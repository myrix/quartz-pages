---
created: 2024-10-29 06:11:00+03:00
---

An aggregate of a number of specific suggestions, some connected, some not.

I'm writing analytics, or trying to, to the extent it's possible analyzing things as they are.

Things worth doing are worth doing imperfectly.

Just because something of that might be helpful for the development of the game.

Unless want to go do set up IDE and work on a feature?

# Notes

## Scaling abilities

based on Steam discussion, see about fp

as Sineso said, need a scaling ability in each skill

+experience in generalist weapon masteries
+damage in specialist weapon masteries

Athletics: see square paper note.

athletics:
+0.5 dodge per athletics level
+0.5 dodge for each point of total bonus move speed above 50

accuracy?
+0.5 accuracy per swords level after swords level 25

swords, unbounded fp sink:
+1 dodge per level with swords

for resistance:
+max(current energy + level - 100, 0) percent

## Balancing unbounded progression

attack capabilities
defense capabilities

linear for attack, leading to 1/(V + N) scaling
for defense --- capping to 100

capped at 100% - ceil(X% / 50)

with total resistance capped at 100% 

possible info for players:
gives 1% bonus per level

Gives 1% bonus <stat_name> per level, discounted after 50% (see <stat_name> tooltip in Stats).
OR
Gives 1% bonus <stat_name> per level, with diminishing returns after 50% (see <stat_name> tooltip in Stats).

gives 1% per level, with diminishing returns after 50% (currently X% total, +)

## Skill Tree extention

after fp and scaling abilities, cause where can we place it?

could be one of those secret-type things you talked about, bam, player realises there's whole another tier to a skill! awesome! hey, could there be the same for other skills?

Dreadheart / Athletics / Survival comparison, adding/unloading and how?

like you said, a sort of guide for a new player

Rejected abilities for skill tree extension, like +dodge from movement after 150 from Athletics, or +%xp from weapon masteries.

## Solution to capping and ESL

after scaling abilities, cause if scaling some we'd need to cap

as in education, better to first get simple concept and then elaborate on it to a more complex understanding

then fail when trying to get more complex understanding immediately

e.g. atom model, first planetary with electrons rotating, and then electrons as probability clouds (and there's next step when it's actually underlying wavefunction, etc.)

example from \#questions channel of user IOIOI --- compare explanation of that and a better, shorter one for ESL

## Travel Weariness

see 

Make into a full-fledged system, along with:
1. Hunger.
2. Combat.
3. Questing.

challenge -> player acts -> win or lose

storytelling triad: self, environment, other people

## Ways of Polling

See on mobile messages.

# Write-up text v. 1 (obsolete)

Was made obsolete after [conversation with Sineso](https://discord.com/channels/@me/1266914098101223505/1308097999469019216), in which the question of possibility of me helping development of the game as programmer / code writer was raised before the suggestions were ready.

## Text proper

Hey Sineso, so here's some rationale and suggestions for unbounded scaling abilities and travel weariness and some other things.

And I would also like to again put forward myself for your consideration as a programmer / code writer for the game, I'll expand on that shortly including your points about large codebase and working in a timely manner you replied with when I first proposed that.

Before everything else, that's not connected to or spurred on by Juki's role change, I conceived these suggestions and proposal in full about a week after v0.5.11 came out, and I learned about the change much later when it apparently happened and you informed me. Not trying to take advantage of or influence or use the situation in any way.

For maximum clarity, I explicitly, unequivocally state that me proposing myself as programmer for the game is not conditional on any kind of attention to my suggestions, and vice versa, you using my coding help for the game does not entail any expectations for my suggestions.

**1. Motivation**

While writing suggestions again noticed how I'm not that good at it. I as always tried to produce good quality, both a) technically, with clear delivery and exposition, solid rationale and logic, and b) in content, so that suggestions are sound and would actually make the game better; but it takes what I feel is much time and effort that could be spend more efficiently on other things helping the game.

Compared to suggestions which I'm not quite good at, I would say I'm so-so at math and actually good at coding, or at least good enough as evidence I would present later would show.

I remember you saying that I can help with beta testing, and occasionally help you with math concepts, and that suggestions are always welcome, but I honestly feel I could help even more with writing code, and that's why I would appreciate for you to consider me helping as a programmer again.

My motivation:

1. Would like for the game to be more complete, done faster, and I would like it to be the best it can be, the best there is. So naturally would like to help with that.
	
	And I'm ready to do any work in priority determined by you from what is best for the game. There are some features I would like more to be ready than others, like hotbar extension, main quest, other magic skills, modding, but that has no bearing on which parts I could work on.
	
2. If you'd consider my contribution sufficient enough, I would be delighted to be in the credits.

3. And of course there's good feeling derived from working on something meaningfully useful I mentioned before.

For clarity, I propose myself to volunteer part-time with no pay as a programmer / code writer.

For completeness, I'm also ready to work for full-time for $3000 USD/month, but a) from cost/benefit standpoint, part-time unpaid volunteering is obviously better, and b) given what you said about https://steam-revenue-calculator.com estimate being in the ballpark, I'm not sure such expenses even make sense for the project, regardless of possible benefits.

**2. Technical expertise**

I graduated from Moscow State University, Russia's top school, in 2011, with specialization in computer science and mathematics; worked as software engineer intermittently since and 2007 and full-time since 2011.

Worked on small and large software written in Java, C/C++, Python, Scala, Javascript.

Recent years I'm working on a Python/SQL/Javascript project, you can see my work if you'd like at https://github.com/ispras/lingvodoc/commits?author=myrix (backend) and https://github.com/ispras/lingvodoc-react/commits/staging?author=myrix (frontend); disregard non-standard branch structure, legacy issues which are unfortunately deemed low priority.

The project is quite large, 100k+ loc in Python and JavaScript total; when I started working on it, I had no problem familiarizing myself with its rather large code base written by others before me, and it wasn't an issue ever since. Interestingly, when I just started working on it the frontend was done via Scala compiled to JavaScript, and I had no problem figuring out how to develop it and write Scala, a language I had no experience with before.

To further illustrate my ability to familiarize myself with and work on large codebases and seemlessly integrate my work into projects written by other people, here's another example, incidentally closer to gamedev. In 2021 – 2022 I'd done a little bit of variety work on OpenMW, an open source engine implementation for Bethesda's The Elder Scrolls III: Morrowind. If you'd like, you can check out issues and associated merge requests and commits:

1. [#6419 Don't grey out topics if they can produce another topic reference](https://gitlab.com/OpenMW/openmw/-/issues/6419) — requested by another player, implemented by me.

2. [#6501 Stuttering in the dialogue menu](https://gitlab.com/OpenMW/openmw/-/issues/6501) — fixing unintended side-effect of the 1st one, significant slowdown apparent when using Morrowind's Russian translation.

3. [#6901 Morrowind.exe soul gem usage discrepancy](https://gitlab.com/OpenMW/openmw/-/issues/6901) — encountered and reported by me, fixed by me.

4. [#6888 Add switch for armor degradation fix](https://gitlab.com/OpenMW/openmw/-/issues/6888) — requested by another player, implemented by me.

Nothing that involved, but each required familiarizing myself with corresponding parts of OpenMW's large codebase, 100k+ loc of C++, and the work was good enough to be in OpenMW's master to this day and get me into OpenMW's credits. Had no need to consult with other OpenMW devs, this work was done in parallel to my own personal modifications of OpenMW I did when playing Morrowind with it, I was able to figure out how OpenMW works and modify it completely on my own.

So, overall, you can be sure I'll be able to work with the game's codebase no problem. You can chuck me into the deep end and give me nothing but a short description of what needs to be done, and I'll do it. Though of course I'm able to work with however detailed task descriptions, with any additional directions on how it should be done, including algorithmic, architectural etc. concerns. And I'm ready to iterate on the result until it satisfies all requirements.

**3. Workflow and timing**

I'm ready to work on any number of tasks and issues as directed and prioritized by you. Small or large, interesting or boring, game mechanics or UI or anything else.

My available free time comes out to about a week each month; my current job is somewhat flexible, so I can spread that week per month as needed, intermittently or or in chunks.

So if there's a time-sensitive task, I could start it and work on it full-time doing nothing else until it's done, the only hurdle is that I will for a time have less free time available afterwards for other tasks.

Or if there's a queue of not so time-sensitive tasks, I could just do them as prioritized by you in a more spread out fashion.

I would also have absolutely no problem, if priorities shake out that way, doing things meant for the future, for next update or the update after the next or even further into the future, and then when their time comes merging them, with adjustment if required, into a main development branch.

And of course throughout all that if I would start volunteering I would ever be available for fixes, support and discussion and won't leave you hanging; if circumstances would change requiring temporary or permanent schedule adjustment or something else, I would notify in advance.

**Separate, somewhat unrelated thing**

Have you considered seeing about the possibility of attempting to invite Juki back to development? Asking cause as far as I understand he had been with the game for years and I assume done much good work, so it would help the game.

Maybe there's some specific issue or issues there's a disagreement on, and it can be tried being talked out? If there are arguments on suggestions, it might be reasonable to try discussing them on merits; if it concerns some of my suggestions, I could offer my participation if it would help. And overall on anything that concerns me I could provide my perspective and hopefully explain my motivation and reasoning and why I do what I do, if it would help.

Perhaps there are some specific things that might motivate Juki to take up development again? It might be worth inquiring and seeing if it's compatible or can be made compatible with the direction of the development of the game you're setting.

# Write-up text v. 2

Here's a design suggestion for unbounded scaling abilities and a possible variant of recipe and ability discovery mechanic: \<link\>

Nothing urgent, so check out when you have time and it's convenient.

Started writing it a while ago and hadn't time to polish it, so if there's any inconsistencies or missing things or whatever, or questions or comments or queries for elaboration, tell me and I'll update.

It's as an HTML export from my Obsidian.md notes, couldn't find a way to export to Google docs, tried exporting as PDF and importing into Google docs, but doesn't work good, some images are missing. Maybe there's a way to convert HTML to Google doc, don't know, if you'd need tell me and I'll try to find a way.

Tried to do this more as an analysis with rationale as opposed to just straight suggestions, more chances that way I hope it will useful for the game, as always if not directly, then as a source of inspiration arguments.

Took a lot of time cause needed to think it through and then write it up, but I still think it's worth it.

**1. Next write-ups**

I'm still going to also write up suggestions of possible things with rationale on a) tutorials and some interface QoL things, b) new game plus, metaprogression and difficulty game modes, and c) travel weariness.

Two reasons I want to do this: 1) if there's a chance my suggestions could influence game design, even if not directly, I would like to take it, cause that's rewarding and feels good, probably even more rewarding then writing code; 2) due to considerations on possible plans to release out of early access.

To elaborate on the 2nd reason, if the game is to be released out of early access, it's foundational systems, like general skill and ability stuff, possible difficulty modes and new game plus and metaprogression, hunger and travel weariness, should be finalized before higher level content, like quests, specific skills, items etc.

Doesn't mean that only foundational systems should be worked on until they're done, it's better to intersperse with higher level content, to give players updates and in the mean time to have attention and focus to thoroughly design foundational stuff portion by portion to the highest quality.

But yeah, have thoughts on this foundational stuff and want to write up on the chance it would be helpful for the game and to crystallize my notions of this systems.

Yeah, I remember you saying that there's travel weariness stuff I don't know and might miss the mark because of it, but it's better for me to work out why I think what I think, and then if/when the discrepancies will become apparent I can take additional info in and update my understanding and notions on how things should be, if required.

Unless of course you, as the ultimate beneficiary, would notify me that there's comparatively little value in my suggestions and rationale; I'd like to use my time efficiently and if writing suggestions is for sure not that useful, I would rather be writing code. So, after perusing my current write-up please notify if it's any useful in any way.

**2. Current plans**

Need to focus on my job for a while, through that's just means would write-up things referred to above not immediately, I'm as before available for discussion/testing, message me any time.

I'm going to at the end of this week, or beginning of the next one, start talking to my team lead on the possibility of me disengaging from my current job; it's not ideal, I really wanted to contribute some code to the game before I would start talking, but there's no time, would be wrong not to give the heads up that I might be leave and stop being available starting some time next year, I'm sure he would appreciate info for planning.

Then back to writing up, maybe with some coding in between.