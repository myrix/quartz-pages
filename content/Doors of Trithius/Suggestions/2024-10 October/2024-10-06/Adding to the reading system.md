---
created: 2024-11-10 18:02:51+03:00
assigned datetime: 2024-10-06 14:59:00+03:00
tags:
 - DoorsOfTrithius
 - Suggestion
 - Reading
 - Ability
 - GenericBooks
---

Isn't meant to affect the game significantly, just add more content and things to engage for the player with.

Specific values are off the cuff and if accepted should be checked and tweaked where required.

# Additional passives

Infinite series of passives: Polymath 1, 2, ....

Polymath N requires N worldlore, N mysticism, N philosophy, requires and replaces Polymath N-1 and gives +N% wisdom. (So to overall to get +N% wisdom from it would need N(N+1)/2 worldlore, mysticism, philosophy points.)

Knowledge is Power series of passives:

+1% weapon mastery xp for each available not spent philosophy knowledge point, costs 5 philosophy.
+1% general skill xp for each available not spent worldlore knowledge point, costs 5 worldlore.
+1% magic skill xp for each available not spent mysticism knowledge point, costs 5 mysticism.

Gives nice tradeoff, do you spend your knowledge points (e.g. on Polymath), or do you keep them for increased passive bonuses?
 
## Possible additional Knowledge is Power passives

Each possibly needing a book study as a basis.

for each available worldlore point, +1% to haggling, costs 5 worldlore.
for each available worldlore point, +1 travel fortitude, costs 5 worldlore.
for each available worldlore point, +1% chance to create a potent/superb food/medicine/alchemy, +1% chance to duplicate a food, including foods with less than 3 ingredients and single-ingredient foods, costs 5 worldlore.

for each available mysticism point, +1% to health & energy regen, costs 5 mysticism.
for each available mysticism point, +1% to magic, mental, physical warding, costs 5 mysticism.
for each available mysticism point, -1% to magic generalist magic skill xp reduction, costs 5 mysticism.

for each available philosophy point, +1% crit damage, +0.5% crit chance, costs 5 philosophy.
for each available philosophy point, +1% protection, +0.5% damage resistance, +0.5% wound resistance, costs 5 philosophy.
for each available philosophy point, +1% light, +1% view distance, costs 5 philosophy.

Dying Light (possibly requires base life steal >0% from any other source to be active?), for each point of min(available worldlore, available mysticism, available philosophy) gain +0.5% life steal, costs 5 worldlore, 5 mysticism, 5 philosophy.

Rage against the Night, for each point of min(available worldlore, available mysticism, available philosophy) gain -0.5% all abilities cost reduction, costs 5 worldlore, 5 mysticism, 5 philosophy.
 
# Generic books

T is total number of all non-generic books available in the game, R is number of books the player had studied.

After R/T exceeds alpha (from 0 to 1), start adding generic books to the book pool, to be possible found in loot and shops, keeping total number of unread books as (1 - alpha)T.

Finding new books would still be a diminishing return prospect, as with random distribution in loot and shops the chance to get an unread book, equal the fraction of unread books to total books, would be (1 - alpha)T / (R + (1 - alpha)T), decreasing with R.

When alpha is 0, players might see generic books right after their 1st study. It may be undesirable, so can choose alpha > 0, maybe 0.15, 0.25, 0.35? The higher alpha is, the less chance to find unread books would be.

Wouldn't unbalance Reading, cause reading xp income is inversely proportional to R number of read books, and then reading levels are further decreased by quadratic or near-quadratic xp curve.

Generic books are generated as (Beginner/Intermediate/Advanced) (Skill/Worldlore/Philosophy/Mysticism) 1, 2, ..., for more variety. Numbers are purely to differentiate books, don't mean anything, can be generated in order. Could generate in batches by numbers to keep distribution balanced, adding all from the N batch whenever need to grow the pool of available unread books.

Beginner books require Reading 7 (or Skill 5 for skill books), give 80 reading xp (+60 skill xp for skill books / +3 knowledge points for knowledge books).
Intermediate books require Reading 11 (or Skill 7 for skill books), give 120 reading xp (+80 skill xp for skill books / +6 knowledge points for knowledge books).
Advanced books require Reading 17 (or Skill 11 for skill books), give 180 reading xp (+120 skill xp for skill books / +9 knowledge points for knowledge books).