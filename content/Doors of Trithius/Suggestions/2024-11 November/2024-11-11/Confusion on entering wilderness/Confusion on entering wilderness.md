---
created: 2024-11-11 13:58:31+03:00
tags:
 - DoorsOfTrithius
 - Suggestion
 - Overworld
 - Wilderness
 - Exploration
 - Tutorial
 - Player/Information
---

**Mitigating possible confusion about entering wilderness tiles**

So today Rigante reported that it's not always clear that you can enter and explore wilderness tiles from the overworld, and at least one other player reported the same, see 1st comment under [*merusalem*'s guide on Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=3349638061):

> One huge thing you mention is the ability to enter map tiles on the over world at any point. I was disappointed thinking it was only random encounters.

In the 2nd case it seems it was one of the issues causing the player to contemplate refund, so it's probably worth looking into.

As far as I was able to check, there's nowhere the player is directly informed they have the ability to enter and explore any wilderness tile at will.

First tutorial after leaving the starting dungeon, on wilderness danger, doesn't actually mention anything about entering and exploring wilderness:
![[tutorial_1.png]]

Then the player probably arrives at the starting town, and they can infer from the town pop-up that they can enter tiles with keyboard E, and that this would also work on wilderness tiles.
![[nerton.png]]

But they also might not, as there's no pop-ups when moving onto wilderness tile in the overworld travel, so clearly these are distinct situations and there's no reason to connect what works in one to another.

Next the player probably gets starting town tutorial, on exit strategy, and it might further reinforce this perceived distinction due to only mentioning towns and dungeons in the context of ability to use escape command:
![[tutorial_2.png]]

This ambiguity, which has possibility to be a source of confusion, can be mitigated by:

1. Adding explicit clarification on wilderness exploration to the Wilderness Danger tutotial, e.g.:
	
	"Any tile can be explored by using \[E\] key. Wilderness can be a source of resources and experience, but it can also be a source of danger depending on it's type and surroundings.
	
	Friendly settlements can be a safe haven, giving respite from the dangers of wilderness and allowing to recover from weariness accrued while travelling."
	
2. Explicitly mentioning wilderness as circumstances for the use of escape \[B\] command in Exit Strategy tutorial.
	
	E.g. by replacing "This command works in towns and dungeons, but only if no enemies are nearby" by:
	
	"This command works in settlements, dungeons and wilderness, but only if no enemies are nearby and you are not in battle."
	
	This also would give additional benefits of a) using 'settlement' instead of 'town' to include farms and villages, and b) mentioning that you can't escape battles, which can be a nasty frustrating surprise otherwise.