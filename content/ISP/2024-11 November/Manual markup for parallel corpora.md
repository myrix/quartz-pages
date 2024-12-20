---
created: 2024-11-24 02:13:56+03:00
tags:
 - ISP
 - ParallelCorpora
 - Markup
 - Manual
---

Мысли по поводу реализации ручной разметки связанных интервалов для параллельных корпусов для Владимира.

> Vladimir Monakhov, 23/11/2024 17:00
> 
> Если Наталья должным образом вольётся и справится, Ты в этом задании принимать участие не будешь?
> 
> Ivan Beloborodov, 23/11/2024 17:01
> 
> думаю да, если прям не нужно будет. также если тебе это поможет могу подумать насчет того как это лучше в бэке реализовать.
> 
> Vladimir Monakhov, 23/11/2024 17:02
> 
> Да, лучше на первых этапах, чтоб было с кем обсудить, потому что по-разному можно представлять решение, а в одиночку можно пойти не тем путём)

# Text

Мысли навскидку, и вполне возможно я что-то пропускаю или будет противоречия с чем-то что выявится в процессе реализации, так что как обычно всегда смотри сам по ситуации и если нужно меняй абсолютно любые вещи.

С одной стороны, это будут разметки текстов, поэтому естественно привязываться к тексту, т.е. к entity в которой текст; с другой стороны, нужна связь с соответствующей разметкой для параллельного текста, в другой сущности.

В простейшем варианте связь это просто какой-либо уникальный идентификатор, типа UUID или порядкового номера, который указан и в той и другой разметке и нигде больше — по тому же принципу как тэги используются для связывания групп когнатов, но проще, т.к. только 2 вещи для связывания.

Возможно, окажется в процессе размышления что будет иметь смысл хранить прямые ссылки или как-то по-другому связывать, и это еще может зависить от того как храним, так что будем иметь в виду на потом.

Нужно будет хранить и несвязанные разметки, хотя бы в процессе создания когда пользователь разметил в одном предложении но еще не разметил в параллельном, так что связь получается опциональная.

В каждой разметке будут собственно данные выделения в виде списка интервалов произвольной ненулевой длины, вида `[[a1, b1], ..., [an, bn]]`, плюс возможно маркировка класса сущности которая была выделена, такие данные произвольного вида естественно хранить как json, типа как `{"selection": [...], "mark": ...}`.

Плюс в разметке должна быть идентификация пользователя, который ее создал.

Мелькала у меня мысль хранить все данные разметок в метаданных сущностей, но нет, это отдельные вещи которые будут у очень малой доли миллионов сущностей, хранящихся в системе, поэтому лучше хранить отдельно в виде отдельных записей БД, плюс это будет хорошо с точки зрения нормализации, значения которые всегда есть лучше выделять в отдельные атрибуты а не хранить в json'е.

В целом, для разметок получается отдельная таблица следующей структуры:

`client_id, object_id` — как обычно, уникальный идентификатор, `client_id` идентифицирует пользователя.

`entity_client_id, entity_object_id` — ссылка на текстовую сущность, в которой эта разметка.

`created_at` — стандарт.

`marked_for_deletion` — чтобы можно было разметки удалять, если они были созданы по ошибке, или были неправильные а правильные уже были сделаны, или вообще по любой другой причине.

`data: jsonb` — собственно данные.

Если для связи разметок используются тэги, то нужно будет поле тэгов, `tag`, допустим типа bigint, и новые уникальные тэги будут браться из отдельной sequence в базе данных, или типа text, и тэги будут генерится рандомно, например как uuid или как текущие тэги для групповых полей, типа когнатов.

При использовании этого поля нужен будет индекс по нему.

Если для связи разметок используются прямые ссылки, то нужно будет просто foreign key поле, ссылающееся на парную разметку через ее client_id, object_id, и оно будет автоматически индексировано; но тут кстати момент, прямые ссылки такого вида будут допускать только парные 1-к-1 связи, в то время как тэггирование будет позволять группы разметок произвольного размера. Задел на будущее с параллельными корпусами с множеством текстов?

Операции для работы над разметками:

1. Создание.

2. Редактирование.

3. Удаление.

4. Связывание/редактирование связей с парными разметками.

Кто может редактировать/удалять/связывать/менять связи? Либо пользователь который создал, либо администратор.

В целом, новая таблица в БД, новый модельный класс в models.py, новый GraphQL-интерфейс в gql_holders.py или новом gql-модуле.

Это все для бэка, про интерфейс не думал, что-то стандартное для ручных разметчиков, можно посмотреть в интернете и даже у нас в нашем родном отделе информационных технологий было общее решение для разметки, можно посмотреть в качестве источника вдохновения. И дальше просто реализация по требованиям.

---

Посмотрел соображения в https://github.com/ispras/lingvodoc-react/issues/1152, вижу думаем в разных направлениях :)

Мне думается, что как отдельные записи в БД лучше, т.к. наколько я знаю разметки результатов парсеров так хранятся потому что это выдача парсера в таком исходном виде, и из-за этого, хранения в html сразу кучи всего, проблемы при работе, редактировании, сохранении, экспорте и извлечении данных, когда мы допустим данные валентностей получаем.

Но опять-таки это твоя работа и твоя реализация, и точно нельзя заложиться на то как будет лучше всего пока не начнется собственно реализация, так что абсолютно на твое усмотрение по ситуации.