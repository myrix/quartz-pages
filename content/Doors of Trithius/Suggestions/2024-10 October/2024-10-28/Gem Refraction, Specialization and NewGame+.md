#DoorsOfTrithius #Suggestion #GemRefraction #Ability #DarkArts #Skill #SkillSpecialization #DarkShadow #NewGamePlus #Balance #Metaprogression 

# Discord context

> Geneticlover — 10/26/2024 2:09 AM
> 
> mmm skeleton army
> another suggestion, dunno if planned but i feel like the ggame needs some things that are specializations to the skill trees
> for instance, some specializations in botany that you canNOT get all of.  you have to choose only one.
> would give a lot of replayability
> like for cooking, you could have a spec that grants ability to make any recipe that requires 2 of something with 1 instead
> thrifty cook or some shit
> 
> Geneticlover — 10/26/2024 2:16 AM
> 
> and other specs that just make your food better or access to special recipes maybe like exotic cooking
> so you'd have to choose between having food more easily with less ingredients or more exotic foods, or just better foods
> 
> October 27, 2024
> 
> Geneticlover — Yesterday at 4:22 AM
> 
> gem refracting skill or whatever it is from reading skill  seems mega busted.  1 max hp and energy for every emerald and ruby in inventory.  easy to farm in any mountain tile from snake rocks.  no cap.  seems like there should be a maximum cap to the skill?

# Notes

point for replayability? --- steam discussion on experience abilities in weapon masteries

# Write-up

A sort of comment on recent Geneticlover's suggestions.

## 1. Gem Refraction

Hard restrictions and limits can reduce fun and induce frustration, especially if it's a nerf.

I personally don't see much need to balance Gem Refraction, cause for any additional +1 hp / energy player has to work, to do things.

Yet, if there would be a need to balance its effect to some extent, could do it with a raisable cap, e.g. in a following way:

1. Make Gem refraction an unbounded series of abilities, level 1 cost as it is now 6 Mysticism, allows up to +25 max hp and +25 max energy from gems.

2. Each subsequent level costs 1 Mysticism, 1 Worldlore and 1 Knowledge and raises the cap by 5.
   
	Alternatively, for even bigger supression, could raise the costs by 1 for each additional level, so Gem Refraction level 3 would cost 2 Mysticism, 2 Worldlore and 2 Knowledge and so on.
	
	Though in that case I would also introduce unbounded generic books as in one of my previous suggestions, to at least give the player a possibility of raising as high as possible if they would feel like putting the work in for that.

Possible justification: the book only gives so much info, unexpected side effects and difficulties crop up when using too many, and you need to conduct your own research and experiments to push further.

### 1.1. Additional possible Dark Arts abilities

While talking about Dark Arts abilities, I have a suggestion for another two:

**a) Kindle the Black Flame**

Can get like the Gem Refraction through a book, or a quest, or in whatever way.

Toggle ability, cooldown 100 turns. On toggle on, gives player the status *Black Flame* of level 1.

Status *Black Flame* level N:

1. -N hp per turn, +4\*N energy per turn.
2. If *Kindle the Black Flame* ability is on, increase level to N+1.
3. If *Kindle the Black Flame* ability is off, decrease level to N-1 when N > 1 or go away if N <= 1.

It's useful, but it burns hp, and if you're not careful, it or the status winding down will kill you --- status level N would consume N\*(N+1)/2 additional hp after ability is toggled off.

**b) Dark Sacrifice**

Also can get through a book, quest, or whatever way; but perhaps could make even more involved, after a quest chain and maybe only at specific locations / with specific map features.

1. Use a consumable (food, potion etc.) you haven't used with the ability before and add a copy of consumable's effects as permanent ability.

	E.g. if a food gives +x hp/turn and +y energy/turn, you now have a passive *Dark Sacrifice: the food* giving +x hp/turn and +y energy/turn permanently.

2. Permanently reduce max hp by 100 + 25\*N where N is the number of *Dark Sacrifice: ...* passives you already have.

	So e.g. first use would give -100 max hp permanently, 2nd use would give additional -125 max hp permanently for -225 total, and so on.
	
	If the max xp (intrinsic, not counting bonuses from items like e.g. Decay Orbs or from Gem Refraction) goes to <= 0, character dies by dark sacrifice.

3. Give *Was that wise?* status of value `GetNextLevelXp(current char level)`:

	No positive hp regen and no energy positive regen except from consumables --- including from *Dark Sacrifice: ...* passives, so you can't even use benefits of that kind immediately --- until the status goes away.
	
	Any wisdom player earns goes into the status, reducing it's value; if the value is reduced to 0, the status goes away.

### 1.2. Dark Shadow ability discussed previously

Previously discussed it as a passive which would replace Athletic's Shadow Mirage with a darker version which would fight back; could make it more engaging and fun by instead using a slightly different version with more depth.

As before, could get it from a book or quest or whatever proper way, this is not changed.

Could be named *Reverted Mirage*.

It's a toggle ability with no cost. It has cooldown of 25 turns, like Shadow Mirage. Upon activation it grants *Shadow Avidity* status, which goes away if the ability is turned off.

The status has a meter, which is filled by any damage player directly inflicts with melee attacks, minus any lifesteal that goes to the player.

When the status is present, actions that normally trigger Shadow Mirage trigger instead Dark Mirage, which in contrast to shadow mirage also attacks enemies and stays present for max of 3 + floor(the meter / 10) turns.

Triggering dark mirage toggles ability off and removes the status. Toggling ability off before mirage is triggered removes the status, while the meter stays in the background and decays at a rate of 1 per turn; if the ability is toggled again before the meter reaches 0, the meter is reused with it's non-zero value.

Upon appearance of dark mirage the meter is transferred from the status to it; if the value of the meter < 10, the player suffers damage of (10 - meter value) hp and the meter is set to 10.

The mirage's attacks continue to fill the meter; the meter is distinct from mirage's hp, mirage taking damage does not affect the meter. (Visual effect: the more meter is filled, the more it's solid and non-transparent.)

If the meter reaches the value of the player's hp (as of the moment when the ability was turned on), the dark mirage incarnates fully and would no longer despawn by itself after any number of turns. It gains ability to move and to use any of the player's abilities (as of the moment when the ability was turned on), and starts attacking everyone indiscriminately until it's destroyed.

If the meter is filled from the player's melee attacks to the value of the player's hp (as of the moment when the ability was turned on) while the ability and the status is still on, the abillity is turned off, the status goes away, and a dark mirage immediately fully incarnates in a closest free tile near the player and starts behaving as described above, attacking everyone indiscriminately.

### 1.3. Possible additional modification for Gem Refraction

Before the gems can be used with Gem Refraction, they could be have to be attuned to in some way, gem after gem. And the ability would only count attuned gems.

E.g. it can be that attuning to a gem gives -1 hp per turn (or -1 energy per turn for the other kind) for 100 turns, can't attune to more than one gem at at time.

Or attuning to a gem would require killing an enemy with a melee attack while the gem is selected for attunement.

## 2. Skill specialization for replayability

As said before, hard limits and telling player No can feel arbitrary and unpleasant, reducing fun.

And we can introduce skill specialization decisions for fun decision making and replayability potential without such hardiness.

Consider Cooking, and for example like Geneticlover specified, let it have two ability groups or branches, A dealing with more esoteric cooking, and B with some of the usual cooking we have now.

#DoorsOfTrithius #Suggestion #Skill #Cooking #Ingredient #Recipe

* As an aside, A can be a suggestion on its own right, e.g. new kind of ingredients in addition to current ones, with perhaps such esoteric ingredients available at a kind of travelling merchant or available for harvesting if you have Hunting skill and high levels of Botany.
	
	Possible new kinds of ingredients: beer liver, wyrm heart, beetle glands, ogre marrow, desert worm rumen, bee venom sacks, ice flesh, fire flesh, thunder flesh, white death mushroom, black death mushroom, fairy cucumber, storm apples.
	
	Esoteric foods also could have new kinds of effects, e.g. +X map hp / +Y max energy for 500 turns.
	
	Esoteric recipes could have chance of failure to prepare (in general perhaps corresponding to the number of ingredients?), which would reduced by cooking and would affect the superb chance.
	
	E.g. with base chance of failure of 35% could have chance of failure of (35 - 2 \* cooking level)% and chance to get superb variant of (2 \* cooking level - 35)%.
	
	Esoteric foods could also have more potent negative effects, e.g. -X hp or -Y energy per turn in addition to their positive ones, and they could be mitigated depending on the cooking level, e.g. -(2 \* cooking level)% to negative effect potency. This could be a separate ability maybe?

A and B start as exclusive to each other, if you choose anything in A you can't choose anything in B and vice versa, except until the condition is fulfilled.

The condition:
1. chosen ability group if fully unlocked, and
2. the skill reaches a preset high level threshold, and
3. an additional passive ability is unlocked.

Could have such additional passive ability in the tree from the start or could let the player acquire it from a book, a quest or in whatever other way.

Justification from realism:

You can't (or it would be horrendously inefficient) simultaneously learn classical European cuisine and e.g. specialty Japanese fugu cuisine, but you can spend a decade becoming a capable chef and then you can again spend years and years training to safely prepare fugu dishes.

Skill level requirement can be chosen as high as needed to make the decision to pursue A or B effectively permanent for all of early, mid and end-game, giving a replayability potential --- to choose either A or B first and have only it for most of even all of the run, or even to choose to put in the work to specifically get both alternatives earlier.

### 2.1. Additional replayability from NewGame+

Could have introduce even more replayability potential via NewGame+ regime with meta-progression. For example:

After winning, character's traits (and maybe selected passives?) are stored, and can start the game anew with this character with traits selected as usual at character creation *and* these additional stored traits.

Then, if across multiple newgame+ with the same character the character acquires in such a way all the traits available to it (e.g. all combat and all physical for Mercenary, all speed and all combat for Street Urchin, all mental for Druid, etc.), it's marked as trait-complete. Corollary, commoner is marked trait-complete on it's first win.

Trait-complete characters characters can acquire any trait other trait-complete characters have, so e.g. if have trait-complete Knight and trait-complete Druid, on a newgame+ with such a Knight player would be able to select mental traits for the Knight.

With an ironman option enabled, each newgame+ also gives additional level to a *Weight of existense* permanent status, which gives the player +5% incoming damage, -3 accuracy and -3 dodge per its level.

If doing an ironman newgame+, upon the character's death the info of the previous successful run for this character is deleted, so the character is set back a step in a newgame+ chain.

On a non-ironman runs the player would be able to select any level of *Weight of existense* status from 0 to the number of wins in the newgame+ chain for this character, and if the character would die in a non-ironman newgame+ there is no setback to the chain.

Overall, this would give:

1. Completionist goal of finishing the meta-progression of getting all the traits on all the characters.

2. For each character, competitive goal of seeing how high in newgame+ level you can get in an ironman mode, when each newgame+ is harder and character death means restart of a run an a step back in the climb along the newgame+ levels.



