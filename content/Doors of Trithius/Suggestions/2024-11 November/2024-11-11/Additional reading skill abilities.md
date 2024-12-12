---
created: 2024-11-11 04:09:32+03:00
tags:
 - DoorsOfTrithius
 - Suggestion
 - Reading
 - Skill
 - Ability
 - Progression/Continuing
---

Two new Reading skill abilities, to
a) fill it out a little bit more, and
b) enable continuing progression, and answer to the question "what to do when everything (or near everything) is done?".

**1. Neverending Journey passive ability**

Can be an ultimate ability at the top of the Reading skill tree.

+(Reading skill level)% to rewards from books, allows re-reading a read book if would have gotten more rewards from it now than what you'd got when you read it.

Re-reading takes the same amount of time as reading.

Re-reading gives only the delta between what you've already got from the book and what you can get now.

Sources of reward increase: Reader's Insight ability, higher Reading level through Neverending Journey, and the 2nd proposed ability, Scattered Interests.

Can re-read books unlimited amount of time as long as you have reading reward increase.

The bonus should also apply to skill xp and knowledge rewards from books; for that could make knowledge meters decimal and increase the scale, so what now gives 1 knowledge point would give e.g. 100 knowledge points, and what now costs 1 knowledge point would cost 100 knowledge points.

This would also give more flexibility in setting knowledge prices, could have something cost e.g. 75 or 150 knowledge points, so like 0.75 or 1.5 knowledge points are they are now.

**1.1. No possibility of imbalance from compounding returns**

Could it be that re-reading books would give additional Reading levels, allowing to re-read books again and so on in a cycle?

No danger of that, let me demonstrate.

With the ability at reading level R re-read increases reading experience you can extract from books by a factor (1 + R/100). Skill level is bounded above by sqrt(skill xp) with some additional constant factor, so increasing xp by a factor of (1 + R/100) would increase reading skill level by a factor of sqrt(1 + R/100).

Then next re-reading iteration would give overall (1 + R/100 * sqrt(1 + R/100)) xp increase and sqrt(1 + R/100 * sqrt(1 + R/100)) skill level increase, and so on, and overall it would come to the increase factor we can define as the limit

x = sqrt(1 + R/100 * sqrt(1 + R/100 * sqrt(1 + R/100 * sqrt(…))))

That's easy to solve with a well-known trick, it's self-recursive so can do a substitution

x = sqrt(1 + R/100 * x)

which rearranges to quadratic equation and gives

x^2 - R / 100 * x - 1 = 0
x = R / 200 + sqrt(1 + (R/200)^2)

Expanding sqrt with a general binomial formula we get for R < 200

x = 1 + R / 200 + 1/2 * (R / 200)^2 + O((R / 200)^4)

That means that re-reading is never a source of infinite reading xp and levels, it's always finitely bounded, and more over, it's only a slow linear increase of levels until about the base reading level of 200, which is effectively beyond a soft cap, and a little bit less slow but still a linear increase of levels beyond that, with factor of about x = 1 + R / 100.

Just don't have enough books in the game to level 200, and even with generic books from a separate suggestion if would require and exponential amount of time — generic book incidence rate over time is proportional to 1/N, N being number of read books, so overall xp rate over time is proportional to integral of that, ln(T), so would need to spend exponentially more and more play time for more and more reading xp.

If a player actually achieves base Reading level of 200, so actually more than level 400 with Neverending Journey bonus baked in, e.g. through skill points from char levelling, I say give this mad dude all the reading xp forever, they earned it.

**2. Scattered Interests passive ability**

Ability would give bonus reading rewards depending on a number of books read, as +floor(sqrt(N))% with N being number of books read. So +1% at 1 read book, +2% at 4 read books and so on.

The bonus should also apply to skill xp rewards and knowledge rewards.

Don't need to communicate exact formula to the player, just need to give a short description with relevant info, like this:

"Increases reading rewards depending on a number of books read, currently by 2%. Would need to read 9 books for 3% increase."

This ability is mostly for filling out Reading skill tree, and as additional source of reading reward increases for more re-read opportunities with Neverending Journey ability.