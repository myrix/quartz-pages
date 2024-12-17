---
created: 2024-11-06 06:29:07+03:00
publish: true
tags:
 - DoorsOfTrithius
 - Suggestion
 - Unbounded
 - Scaling
 - Ability
 - Discovery
---

Suggestions for Sineso on unbounded scaling abilities with some additional things.

Tried to write this as less as possible as just suggestions and as much as possible as analytics, considering alternatives as close to as possible on their merits.

# Unbounded scaling abilities

## Necessity

In our discussions I expressed sentiment that we need scaling abilities so that skill levels don't feel useless after everything in the skills is unlocked.

Other players express complementary sentiment of exactly the same kind about the need for focus points to not feel useless.

From relatively recent [Steam discussion](https://steamcommunity.com/app/1519490/discussions/0/4700160645243044861/) by *Bambinator the deer*:

> \<snip\>
> You gain 1 focus point by gaining a level by mastery (weapons) or by skill level. But at some point the focus point becomes useless (I said the focus point which is useless, not the level itself which is useful because you gain a point charge point per level no matter what). For example I am level 53 in the skill quatermastery with 29 focus points, and I have nothing more to unlock.... Maybe make a talent point that can be maxed infinitely with the extra focus points.
> \<snip\>

Note explicit support for both scaling abilities which scale simply off the skill level (ibid.: "not the level itself which is useful because you gain a point charge point per level no matter what") and scaling abilities which scale off the invested focus points.

Player *black_Leviathan* evidently [shares this sentiment](https://steamcommunity.com/app/1519490/discussions/0/4700160645246990397/#c4700160645247213355) in Steam discussion started by *Bambinator the deer* on the topic of extra focus points:

> To my knowlegde they are sadly useless at the moment.

And that's broadly in line with the general sentiment reached at least for one moment in our discord discussion about the need for continued progression, [succinctly exemplified by](https://discord.com/channels/@me/1266914098101223505/1292870625773490298):

> Sineso — 10/07/2024 6:26 PM
> 
> \<snip\>
> Something I have made a note of actually from this conversation, is to consider for skill trees how I can add scaling unlocks mid to late game for continued progression.
> \<snip\>

So, aggregating all that and expanding with obvious balancing considerations:

1. Players express preference for, and the game better have unbounded scaling abilities.
    
    Both abilities that scale with just skill level and that scale with spent focus points, so that earned skill levels and focus points never feel useless, decreasing fun and appeal of the game.
    
2. Such abilities should in some way fit into skill trees.
    
3. Such abilities should be balanced, preferably in a general way so that there's less need to balance each individually.

While this probably isn't a core feature, it's something that can enhance the game, polish it, the kind of thing that takes game from good to very good and from very good to great — so all other things being equal, better have it if possible.

Thinking about it, this is actually a specific instance of a general principle of catering to player's satisfaction.

### Player's satisfaction

Games are, among other things, engines of satisfaction. While for any game player's satisfaction per se and its maximization is not the main thing about the game, cause it's general and the game is specifically about what the game is about, it's important, could even say obviously important.

From developer's perspective, could outline at least two specific somewhat related motivations of importance:

1. Players deriving satisfaction from the game is one measure of the game's value to the players, and making a product of as high as possible value to as many as possible people is an intrinsic reward.

2. The more satisfactory the game is, the more it is popular, the higher it is rated, the more it is successful in general and from the monetary perspective in particular.

So whenever possible, leaving other important aspects of the game uncompromised, we should try to tune it to more satisfaction — should aim to establish avenues of satisfaction and should strive to prevent avenues of frustration. And conversely, should strive to prevent disappearance of satisfaction and should aim to encourage disappearance of frustration.

How it applies to this specific instance of scaling abilities is rather obvious, we should try to provide to the players avenues of getting satisfaction from skill levels and from spending focus points regardless of how high a skill level player reaches, precluding frustration of acquired skill levels and focus points losing effect and becoming useless. And, while doing so, we should be careful not to introduce additional frustration or break existing satisfaction due to balancing effects or other concerns.

It's better for as many as possible aspects of the game to be tuned and polished for more satisfaction and smoothed for less frustration due to the psychological halo effect, which enhances positive impressions and buttresses negative impressions of unrelated parts of the game due to satisfactory experience with other parts of the game.

How satisfaction tuning relates to the general principle of aiming to design the set of player's inputs and the game's state space with how its state changes depending on and how it responds to player's inputs? Feels like it would be most accurate to say it's one specific concern of the general design process.

## Kinds of possible unbounded scaling abilities

Already in the game for some skills:

1. Scaling from skill level, the simplest kind.
    
    E.g. Swords' standard Sword Finesse, +1% damage with swords per level of Swords weapon mastery. 

New proposed ability kinds:

2. Scaling from linear spent focus points, +1 ability level per 1 spent focus point.
    
    E.g. hypothetical Swords passive ability giving +1 accuracy with swords for each ability level, so effectively +1 accuracy per 1 spent focus point:
    
    ability level 1 (+1 accuracy) for 1 fp
    ability level 2 (+2 accuracy) for 1 fp
    ability level 3 (+3 accuracy) for 1 fp
    …
    
3. Scaling from quadratic spent focus points, Nth ability level for N spend focus point.
    
    E.g. hypothetical Swords passive ability giving +2 dodge with swords per ability level:
    
    ability level 1 (+2 dodge) for 1 fp (1 fp total, +2 dodge/fp)
    ability level 2 (+4 dodge) for 2 fp (3 fp total, +1⅓ dodge/fp)
    ability level 3 (+6 dodge) for 3 fp (6 fp total, +1 dodge/fp)
    …
    
    Can use this kind of abilities when we need a sort of soft-cap-like behaviour, first levels are easy to get, but then the steadily increasing fp costs make additional ability levels relatively ineffective.
    
4. Scaling from unspent focus points, +X effect per 1 unspent focus point.
    
    E.g. following hypothetical Swords passive abilities:
    
    +1 attack speed for each unspent focus point
    +1% crit chance for each unspent focus point
    +1% crit resist for each unspent focus point
    
    Same type of abilities, scaling off unspent points, as some of the reading knowledge points abilities suggested some type ago, but now with focus points. 
    
    This kind of abilities create an interesting dynamic decision landscape for the player to engage and have fun with, e.g. with two abilities of such kind being unlocked each unspent focus point now has two beneficial effects. So cost/benefit of keeping focus points unspent for abilities of the 4th kind vs. spending them on the abilities of the 2nd and 3rd kind also depends on how many abilities of the 4th kind are in the skill and how many and which of them are unlocked.
    
    Such abilities can be justified as sort of unapplied, general skill knowledge and experience, as opposed to focused, directed application that is abilities of the 2nd and 3rd kind, but still somewhat slightly more focused than totally general abilities of the 4th kind. Though main appeal of them is that they mechanically add beneficial variety — I remember you mentioning research on how additional choice affects satisfaction and its inflection point, this is exactly the kind of additional 2nd/3rd choice still increasing satisfaction.

Rationale for the kinds:

1st kind makes skill levels not useless.

2nd kind makes focus points not useless.

3rd kind makes focus points not useless, allows working with effects we might want less unbounded scaling for.

4th kind makes focus points not useless and complements 2nd and 3rd kind by adding a new way to use and look at focus points.

Each skill in general — weapon masteries, general skills and magic skils — should have scaling abilities for making both skill levels and focus points not useless, so at least one ability of the 1st kind and one ability of one of the 2nd, 3rd or 4th kind.

### General considerations depending on ability kind

First consideration, need to note that a skill having just a single ability of the 2nd kind with no abilities of the 3rd or 4th kind would be bad design due to player's wasted effort.

E.g. if player would see just an ability giving +1 accuracy for each spent focus point, they would rightly be annoyed, "why do you make me manually click unlock for each ability level when you could just given me the same effect with no clicking required from a simple +1 accuracy per skill level ability?".

So if a skill is to have an ability of the 2nd kind, there should be at least one other ability of the 2nd, 3rd or 4th kind to introduce alternative focus point uses and make unlocks mean something.

Second consideration, a skill having just a single ability of the 4th kind with no abilities of the 2nd or 3rd kind would be not so good design due to another issue, there would be no clicking required but it would feel like inventing focus point use just for the sake of it.

E.g. if player would see just an ability giving +1 attack speed for each unspent focus point, it would give perception of artificial introduction of a focus point sink to pave over useless focus point issue, as the same effect is achieved with less complexity and hassle just by a simple +1 attack per skill level ability.

So if a skill is to have an ability of the 4th kind, there should be at least one another ability of the 2nd or 3rd kind to introduce alternative focus point uses.

Finally, if possible, a little bit more choice with abilities abilities of the 2nd and 3rd kind would make player's experience better, and abilities 4th kind shine best when there's at least two of them, so ideally each skill better have several additional scaling abilities.

Naturally a question arises, how could all these abilities fit with skills trees?

## Additional skill abilities acquireable mid-playthrough

In general can't fit all scaling abilities we better have neither in existing skill trees nor in upcoming ones, even if there might be place for one or two additional ability in some skill trees. So, additional abilities should be added during playthrough, separately from sources other than initial skill trees. But then, how to arrange them with the trees?

This point doesn't only concern proposed scaling abilities, in the game there are already skill abilities player can aqcuire mid-playthrough from scrolls of technique, e.g. Mordhau Bash for Swords, though all of such abilities as far as I'm aware are currently in weapon masteries which are not trees.

Even if currently there are not that many abilities and they can be folded into the upcoming trees for masteries, I also suggest introducing more standard, non-scaling abilities acquireable mid-playthrough. Could invent new, could re-use any previously removed, after some tweaking if required.

So overall, I suggest for each skill to have around from 4 up to 10 (or even more if there would be more good ideas that would fit) additional abilities acquireable mid-playthrough after skill acquisition, scaling and non-scaling.

Though, please take note, if it would be decided to add such abilities, they by their nature don't have to be added all at once in a single update or any definite number of updates, can spread them out over any updates in any order that would be suitable.

Possible ways to acquire abilities could include from scrolls, books, quests, events, items, skill reaching required level, perhaps with cross-dependencies on other skill, e.g. need to reach a certain level in the skill and another level in another skill. 

Another possible source is some form of discovery mechanic, as with alchemy/cooking/medicine recipes, which could be better than just a skill reaching required level; see [[#Possible implementation of discovery mechanic]] subsection for exactly what is says.

And of course a variety of types of sources is better than a single source type or a just a few types of sources.

How would that make the game better?

1. Scaling abilities would make skill levels and focus points never useless.

2. It could be one of those secret-like things giving amazement, sense of wonder for the player to discover mentioned in our discussions.
    
    Like player would acquire and additional skill ability and go, "whoa, there's actually more to the skill? does it have even more abilities? does other skills also have more like this?".
    
3. And it would be an additional beautiful complexity which, when properly fitted, increases player's satisfication by just being in the game — it makes the game richer, greater, better looking, better feeling, better for playing.

4. And functionality of additional abilities would provide more space for tactical and strategic decisions and for expression of player agency, more things to play with, to have more fun with — would make game more interesting and give players more avenues for getting satisfaction.

To illustrate this principle of additional beautiful fitting complexity working check out concept scene art for towns (from the discord) and leafborn villages (from scenes in media package) side by side with how towns and leafborn villages look in the game.

Towns:

![[scene_town_more.png]]

![[scene_town.png]]

Leafborn villages:

![[scene_leafborn_more.png]]

![[scene_leafborn.png]]

Also in the same vein an applicable point I had raised earlier by itself, the logo with a gradient is better than the flat logo, exactly due to the same principle of additional beautiful fitting complexity:

![[Doors of Trithius/Suggestions/2024-10 October/2024-10-29/October suggestions/Text - Unbounded scaling abilities/logo_gradient.png]]

![[Doors of Trithius/Suggestions/2024-10 October/2024-10-29/October suggestions/Text - Unbounded scaling abilities/logo_flat.png]]

Just as the game would be better if towns and leafborn villages would look more like concept scenes, less sparse, more filled out, livelier, and just as the logo with the gradient looks and feels better, livelier than the flat logo, the game would be better for having additional acquirable/unlockable skill abilities beyond ones that are currently in the skills in the game and are flat full accessible on skill unlock.

Main example of beautiful rich fitted complexity is actually in the game, it's the combat with all its variety and combinations of different weapons and active abilities. Now that is not to say that each and every aspect should be as complex as combat, but complex greatly put together combat is good, so if we can get some of that goodness of put together complexity in other places, like in unbounded scaling abilities acquirable mid-playthrough, it would be good.

And it's not actually tautological, combat is about abilities you have at the start of the game, while unbounded scaling abilities are about continuing progression in late game and beyond.

Now of course we should be careful with additional complexity that requires to be parsed by the player, like skill abilities, as opposed to additional complexity that's more for looking beautiful and taking in — though should note that as far as I can see in towns and villages example additions are not just for looking pretty, there are some functionality affects like wells, workstations, containers, items etc.

So with additional skill abilities we should take care lest we risk overwhelming the player, but that would not be a problem for additional skill abilities player can acquire mid-playthrough as they would be introduced one-by-one or in small groups and not that frequently just by the nature of their unlock conditions.

And of course fitting, together and with other parts of the game, active functionality that abilities are is more work than fitting mostly passive decorations, but it's worth it for the fun and satisfaction it would bring players.

Next, if we'd decide to have additional skill abilities acquirable mid-playthrough, back to the question we deviated from, how to arrange such abilities with the skill trees?

## Skill pane expansion

The answer to the question of how to arrange acquirable abilities with the skill trees is simple, expand skill panes when a condition for additional abilities is satisfied. Could expand mostly horizontally but some vertical expansion could be good too.

There's a relevant question, is there hard skill pane height limit, perhaps exposed in a default game window size which gives 1270x740 px playing area? Why such, I would call it unround, default size? Why not more common sizes and ratios, e.g. 1280x720 (16:9) or 1280x800 (16:10)?

If there is a hard height limit due to default window size, it's already too hard cause for some skills it squeezes too much, e.g. can't have a more detailed description in Athletics like you have in Medicine, there's just no space:

![[pane_athletics.png]] ![[pane_medicine.png]]

Why not increase skill pane height limit, increasing default window size to e.g. 1280x800 (16:10) or 1440x900 (16:10) or even 1280x960 (4:3) or 1440x960 (3:2)?

Going back to the question of arranging additional abilities with the skill tress, consider placement in expanded skill panels guided by a metaphor 'the tree upon the earth and the stars in the sky' metaphor, which neatly aligns with the pairing of the beginning for a beginner (initial skill tree) and the mastery for the master (additional discoverable abilities later), with red squares marking possible placement locations for additional abilities:

![[extended_taller.png]]

With a little more space, can even arrange the stars into constellations if needed, grouping additional abilities when it makes sense into groups, even maybe connected if required:

![[extended_taller_group.png]]

If the height limit is absolutely absolute and still need to be as narrow as possible, can still achieve this kind of placement, even if it would be a little bit crampier:

![[extended_base.png]]

![[extended_base_group.png]]

Could also make more space to the sides even if need to absolutely preserve height, this would allow more freedom in placement and grouping.

Can place additional abilities as we please, and while where they are placed in relation to other additional abilities and initial skills abilities matter to a certain extent, we can be freer with placement as players would uncover such additional abilities one by one and there would be little place for confusion, it's not like we should optimize for clarity and transparency as with initial skill trees.

So yeah, this would achieve us possibility to add abilities to skills mid-playthrough, which a) would allow us to give players scaling abilities, and b) would be one of those secret things players would go "whoa!" about when they see it.

### Unevenness in skill tree clarity?

Just an aside based on observations of trees of Dreadheart, Chilvalry, Athletics, Warrapt and Survival, in order of decreasing clarity and increasing difficulty of parsing:

![[tree_dreadheart.png]] ![[tree_chivalry.png]] ![[tree_athletics.png]] ![[tree_warrapt.png]] ![[tree_survival.png]]

Contrast is undeniable, Dreadheart offers more clarity and guidance to the player than Survival.

Survival in particular looks rather like a forest than a tree, and even if it's thematically appropriate for the skill :) don't think it's either intentional or desirable for player's clarity of understanding.

If the goal of the trees is to guide and to help players, in particular new players, with a) understanding how skill abilities relate to each other, and b) choosing which abilities acquire in which order, it might help to slightly rearrange more convoluted trees into more parseable shapes.

If current convolutedness is due to maximum height of skill pane due to default window size and the additional need to fit the recipes, that's another argument for expanding default window size, e.g. as stated above, to 1280x800 (16:10) or 1440x900 (16:10) or even 1280x960 (4:3) or 1440x960 (3:2). This would allow more space for rearranging offending trees and making them more understandable.

I would advocate for this approach.

Otherwise, if the height limit is absolute, there's a theoretical option of removing some skill abilities and changing them into abilities that can be acquired mid-playthrough, which also would give more space that could be used for rearranging, but this option has severe drawbacks: a) would need to rebalance affected skills, b) that's taking from the players what they already have, that's frustrating.

I would advocate against this approach, list it here just for theoretical completeness.

## Balancing unbounded scaling abilities

Even if we wouldn't have additional abilities acquirable mid-playthrough, we still need to tackle a question of how to balance unbounded scaling abilities due to abilities unboundedly scaling off skill level which are already in the game.

And if we are to have many new unbounded scaling abilities for many skills, it would be good to have a general way to balance them, to save as much balancing headache as possible, and I would like to suggest a possible way to do exactly that or almost exactly that.

Almost, because abilities would still need to be individually balanced up to a standard cutoff of skill level 50, then consistency checked at skill level 100, and then you can let the proposed general balance technique do its work.

To see how unbounded scaling abilities can be balanced, let's look at an example of an ability that is perfectly balanced, or at least balanced very good — Swords' Sword Finesse, +1% damage with swords per Swords level, or of course any other such standard weapon mastery +1% damage/level ability.

It's balanced good because with all else being equal it increases outgoing attacking capabilities of the player linearly with skill levels, with factor of (1 + 0.01 L), which means that difficulty of overcoming a given outside struggle, e.g. an enemy or a group of enemies with given hp, decreases inversely proportional, with factor of 1/(1 + 0.01 L).

Graphical representation of capabilities and difficulty changing with increasing skill levels:

![[attack_capability.png]]

Closer look at how difficulty changes with increasing skill levels:

![[attack_difficulty.png]]

Can see two very good properties due to how slowly it decreases, global and local:

1. Globally, slow decrease of the difficulty means that there's still enough difficulty at any skill level, no matter how high.
    
    The combat does not feel too easy on any skill level, and the challenge from the difficulty and satisfaction from overcoming the challenge would never go away.

2. Locally, the difference in difficulty at two near enough skill levels is quite small.
    
    Mathematically, difference in difficulty at skills levels $L$ and $L+k$ is inversely proportional to the square of the level and decreases quite quickly:
    $$
    \frac{1}{1 + 0.01 L} - \frac{1}{1 + 0.01 (L + k)} =
    \frac{k}{(100 + L) (100 + L + k)}
    $$
    
    That actually has two separate beneficial effects.
    
    First, skill level jumps large enough to give evidently higher damage numbers and gain satisfaction from increased capability are still close enough that decrease in difficulty is almost unnoticeable, and there's no loss of satisfaction from the challenge.
    
    Second, as with increase of the skill level time to get to the next skill level generally rises, there's a sort of slow-boiling effect.
    
    Player is accustomed to the recent difficulty though prolonged exposure, at higher skills levels compares current decreased difficulty not to the original difficulty at initial skill levels but to more recent, which is lower and less different — e.g. difficulty at skill levels around 100 (≈0.5) is perceived in comparison not to the difficulty of when skill level in the single digits (≈1), but to the difficulty of skill levels in the 50s (≈0.66).
    
    And that gives impression of even more slowly decreasing challenge, almost or I would say completely removing loss of satisfaction from decreasing challenge.

So, speaking generally, scaling ability scales, skill levels and focus points are never useless, skill xp always matters, the player consistently gets satisfaction from each skill level increase and looks forward to even more increases in the future.

Each skill level increase has meaningful consequence of further increasing character capabilities, delivering satisfaction, and while the difficulty decreases a little bit, the change is never qualitative, there is always and forever challenge and it decreases slowly enough that there is no loss of satisfaction due to the loss of the challenge — this aspect of the game is never broken, no regime change.

And that actually is valuable on it's own because it allows maintaining player's anticipation for more and more satisfaction from this avenue, and anticipation enhances satisfaction by adding an independent satisfaction from anticipation itself, or at least that's what I got from skimming what I managed to google on consumer anticipation in marketing psychology.

### Mathematical aside on 1/n difficulty

This is by no means any formal definite proof, by it can shed additional light on conclusions we just reached, or at least I thought it would be neat to show this here.

It's actually interesting how mathematical properties of difficulty, and therefore challenge, decreasing proportionally to 1/L due to capability growing proportionally to L show how ~1/L scaling sits on a sort of best middle ground between fast and slow decrease.

For our difficulty $\sim\!1/L$ we have
$$
\sum_{L=1}^\infty \frac{1}{L} = \infty,
$$
which we can take to mean that in such a regime there's always challenge to be found, and that out satisfaction avenue never breaks due to loss of satisfaction from loss of challenge and, separately, from loss of anticipation of future satisfaction.

If we restrict consideration to difficulty rates of the form $\sim\!1/L^\alpha$, for any difficulty rate with $\alpha > 1$ which decreases faster than our base difficulty rate $\sim\!1/L$ we have a total challenge which is bounded above by finite quantity,
$$
\sum_{L=1}^\infty \frac{1}{L^\alpha} < M, \quad \alpha > 1,
$$
which a) directly means that there's a loss of satisfaction from anticipation of future satisfaction from challenge, cause there's just not enough challenge, only a finite amount, and b) indirectly means that there will be loss of challenge satisfaction by itself, the challenge would just be decreasing too quickly.

Conversely, while with $0 < \alpha < 1$ we would have always still enough challenge,
$$
\sum_{L=1}^\infty \frac{1}{L^\alpha} = \infty, \quad 0 < \alpha < 1,
$$
that would mean that the capability, inversely proportional to difficulty, would grow only sublinearly as $\sim\!L^\alpha$, $0 < \alpha < 1$, which could (for at least main direct damage capability multiplier) lead to loss of satisfaction from slow down of capability growth at higher skill levels.

So it seems that at least for attacking capabilities we would like to have scaling that leads to linear capability growth and inverse difficulty decrease.

And perhaps with some attacking capabilities it would make sense for capability to grow sublinear with difficulty decreasing even slower, but only if it would not lead to loss of direct satisfaction and anticipation satisfaction due to perceived slowness of capability growth.

### Skills, abilities, stats and capabilities

So far all the analysis considered only a situation with a single ability simply linearly scaling off the level of a single skill and linearly affecting a single stat directly translating into an attacking capability, such that overall the capability would scale linearly off the level of the skill — e.g. foundational Swords' passive Sword Finesse, +1% damage per Swords level, affecting +% damage stat which directly goes into direct damage attacking capability, with direct damage growing linearly with Swords' level.

That's not always the case, and even with the direct damage, simplest attacking capability, there are at least two simply scaling abilities that could simultaneously affect +% damage stat, the other being Warrapt's foundational passive Martial Focus giving +0.25% damage per Warrapt level.

Does that change our analysis, and if it does, how? What are exactly our required assumptions and how they could change?

Going from the final effect back, we look at an attacking capability growing linearly, or at least linearly in average over time, with a stat it depend on — direct damage capability and +% damage stat in our analysis so far. In actuality an attacking capability could grow linearly from multiple stats, e.g. our direct damage capability grows linearly with following stats: +% damage, crit chance, crit bonus, repeat attack chance, multi-attack chance, +min/max damage bonus.

Then the stat grows linearly with a level of a skill — in our analysis, +% damage stat and Swords skill. Actually a stat could grow linearly depending on a number of skills, perhaps with different rate per skill, e.g. our +% damage stat grows linearly with both used weapon's weapon mastery skill and Warrapt.

This, however, doesn't change the conclusions of our analysis.

For multiple skills feeding the same stat, desired asymptotic behaviour is the same for any combination of skills separately or jointly, as with skill levels rising the situation sooner or later equilibrates to the state where there's roughly the same work required to add additional parcel of stat increase from an additional level of any of the skills.

And as for a non-asymptotic behaviour, for skill levels roughly up to 50, it is anyway to be balanced more manually with more close consideration and is already balanced in the game.

For multiple stats increasing the same capability, the same arguments apply, base balancing up to stat values from skill levels up to 50 is to be balanced by hand and should be balanced in the game already, and analysis of the asymptotic behaviour in regards to difficulty and challenge also hold, with one caveat though.

The caveat is that if attacking capability depends on a number of stats multiplicatively, we might want to control this multiplicative compounding effect. E.g. our direct damage attacking capability depends on our stats +% damage, crit chance, crit bonus damage, repeat attack chance, multi-attack chance, +min/max damage bonus multiplicatively — if we raise the damage factor depending on +% damage stat by X by raising +% damage stat sufficiently, and we raise average damage factor depending on crit chance by X by raising crit chance sufficiently, and we raise average damage factor depending on repeat attack chance by X, and so on, for K stats, we would raise overall damage capability by X^K.

So we might pay attention to that and for capabilities that depend on a number of stats multiplicatively additionally adjust how these stats scale from skill level jointly, more on that later in [[#Joint and thematic scaling]].

And we should to note that if we are to adjust how capabilities ultimately scale off the skill levels, the best way to do this is at the stat level by adjusting how stats scale off aggregated stat contributions from separate skills which depend on skill levels — it's already done and it works good for move speed and attack speed, but if we think on explicit argument as to why, it might be that:

1. Stats are explicit first-class entities in the game with established means of conveying information to the player through the stat values and tooltips, while capabilities are only implicit aspects of the gameplay and are perceived by the player as aggregated vague gameplay impressions ("combat getting easier/harder").

2. In other direction, stats are actually the mechanical basis of the gameplay as opposed to skill levels and individual stat contributions from skills, so it obviously makes sense to control scaling of the gameplay variable here in one place just before it is used as opposed to in multiple places at the variable's sources.

### Inversely scaling attacking abilities

That's all and good, but all this so far actually holds if an attacking capability actually linearly depends on a stat.

And that is not true for some of the stats, in particular it's wrong for the melee ability cost reduction stat which e.g. can be raised by contributions from the recently mentioned Warrapt foundational passive scaling off Warrapt level.

In fact, if we have $s$ fraction of the ability cost reduced, meaning the ability costs are now by a factor of $1-s$ less, we can use abilities $1/(1-s)$ times more frequently, and our attacking capability is in general larger by the same factor of $1/(1-s)$.

Obviously, this gets out of hand quickly as soon as $s$ is sufficiently close to $1$ and breaks down at $s = 1$:

![[inverse.png]]

And if we are placing a hard limit on ability cost reduction, as it seemingly is now, we are making additional skill levels providing ability cost reduction less useful and losing satisfaction from these additional skill levels.

Fortunately, we can fix this by changing the way military ability cost reduction stat $s$ is computed from the total $x$ of raw melee ability cost reduction contributions from all relevant abilities of all relevant skills and other sources, from a 1-to-1 computation $s = x$ to some suitable transformation $s = f(x)$.

To achieve the desirable regime established above, with capability rising linearly as $\sim\!x$ and difficulty decreasing reciprocally, with constant satisfaction from capability increase and without satisfaction loss from loss of challenge, with additional second-order satisfaction from anticipation, we would need:
$$
\begin{align*}
\frac{1}{1-s} &\sim x \\
\frac{1}{1-f(x)} &\sim x \\
1-f(x) &\sim \frac{1}{x} \\
f(x) &\sim 1 - \frac{1}{x}
\end{align*}
$$

Condition of the form $1 - f(x) \sim 1/x$ might be more useful cause we would strongly like our stat transformation $f(x)$ have additional obvious natural properties, like starting close to 1-to-1 linear relation at the origin, $f(0) = 0$, $f'(0) = 1$, and then gradually decreasing, $f''(x) \le 0$.

To give an idea how that looks like, transformation 
$$
\begin{align*}
f(x)
&= \frac{x}{x + 1} \\
&= 1 - \frac{1}{1 + x}
\end{align*}
$$
alike to current move speed bonus and attack speed bonus transforms satisfies these requirements — though it might not be the best, we'll consider other possibilities a little later.

Can see exactly how the difference $1-f(x)$ decreases with required asymptotic rate $\sim\!1/x$ with increasing $x$ for $f(x) = 1 - 1/(1+x)$:

![[inverse_1.png]]

This general scaling $1 - f(x) \sim 1/x$ was somewhat unexpected for me, that means that my suggestions of the general shape $f(x) \sim 1 - 2^{-x}$ with exponential attenuation I had been making previously for ability cost reduction stats quite a time ago are actually not that good, not optimal — as just like when we previously considered direct attacking capabilites with their preferred direct linear scaling, our desired stat scaling $1 - f(x) \sim 1/x$ sits right in the optimal middle.

If the attenuation $1 - f(x)$ would decrease faster than $1/x$, e.g. exponentially as $2^{-x}$, attacking capability would still be increasing too high, superlinearly, and difficulty would be decreasing too fast, which would lead to satisfaction loss from loss of challenge. On the other hand, if the attenuation  $1 - f(x)$ would decrease slower than $1/x$, that would mean the stat value itself $s = f(x)$ would grow too slowly, with $1 - f(x) \sim 1/x$ it already grows too slow, and making it even slower would lead to loss of satisfaction from stat growth.

Which $f(x)$ exactly would be the best?

Let's consider three candidates, all satisfying already stated requirements of $1 - f(x) \sim 1/x$, $f(0) = 0$, $f'(0) = 1$ and $f''(x) \le 0$.

1. Simplest, already mentioned
    $$
    f(x) = 1 - \frac{1}{1 + x}
    $$
    which is alike to current move speed bonus and attack speed bonus transforms.
    
2. Of the same general shape, but with piece-wise linear growth:
    $$
    f(x) = 1 - \frac{1}{\lfloor 2x + 1 \rfloor} + 2 \, (x \bmod ½) \left[ \frac{1}{\lfloor 2x + 1 \rfloor} - \frac{1}{\lfloor 2x + 2 \rfloor} \right]
    $$
    Is slightly faster growing, which I feel is better, and has additional beneficial properties.
    
    Can be computed with one-liner:
    
    `=1 - 1/FLOOR(2*X+1) + 2*MOD(X,0.5)*(1/FLOOR(2*X+1) - 1/FLOOR(2*X+2))`
    
3. Also continuous, as the simplest one, but constructed so that its rate of growth is closer to the piece-wise linear one:
    $$
    f(x) = (1 - \tanh x) \cdot \left[ 1 - \frac{1}{1 + x} \right] + \tanh x \left[ 1 - \frac{1}{1 + 2x} \right]
    $$

![[inverse_123.png]]

I believe that the 2nd, piece-wise linear, is the best choice, due to considerations of a) balancing, b) satisfaction from stat growth, c) player information. Otherwise the 3rd one, faster continuous, is the second best, and the 1st one, the simplest one, is the last in suitability.

First, balancing.

All three transforms are 1-to-1 or close to 1-to-1 near origin, which preserves current balance for low levels of raw total incoming melee cost reduction and means that there's no need to spend time and work on rebalance.

Piece-wise linear transform, the 2nd one, does it best with 1-to-1 correspondence all the way to 50%, the 3rd, the slightly faster increasing continuous, is second best with this, and the 1st, the simple continuous, is the least good, it deviates from 1-to-1 correspondence the fastest.

Second, satisfaction from stat growth.

While overall suitability from satisfaction is optimal for all three candidates due to required asymptotic behaviour $1 - f(x) \sim 1/x$, as was shown above, we can still compare specifics; and it feels that the 1st, the simple continuous, grows too slow, giving stat value $s = f(x)$ of 50% only at 100% raw total incoming value $x$.

Meanwhile, the 2nd, the piece-wise linear, gives 50% stat at exactly 50% of incoming raw total, and this feels right, while the 3rd, the slightly faster continuous, is not as slow as the 1st but not as fast as the 2nd, and again the 2nd is the best while the 3rd is the second-best.

There's also a difference in second-order satisfaction from anticipation. To have anticipation, the player needs a concept of how the stat $s = f(x)$ would grow with the growth of incoming raw total $x$; this is a part of the whole question of how to best inform the player on the stat scaling, but that we'll discuss fully in the following subsection [[#Informing players]].

With such changing transforms as our $f(x)$ candidates I don't see any way to better inform the player on how stats $s = f(x)$ would grow with the growth of incoming raw total $x$ than just giving the player a rate of change estimate, something like e.g. "X% melee cost reduction, +d.dd% per additional source %", possible tooltip if there is actuall scaling (again, for more thorough consideration of how it is best to inform the player see the following subsection):

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional source percent point
```

And how much there is anticipation relies on ability to have a mental picture of future depending on current and expected changes — the less you're able to predict the less you have anticipation. And if you're basing your predictions on the rate of change, your ability to predict is worse if reported rate of change itself changes frequently, and is conversely if it doesn't change as often.

And with this, the 2nd candidate $f(x)$, the piece-wise linear, is again slightly better than the continuous 3rd and 1st candidate. Due to lineriality of the piece definitions of the 2nd $f(x)$ its reported rate of change would change quite infrequently, while for the continuous 3rd and 1st transforms reported rate of change would change every time the incoming raw total $x$ would change, making player's idea of possible future behaviour of the stat $s = f(x)$ more uncertain and reducing player's anticipation and possible satisfaction from it.

Third, player information.

### Informing players

What is the optimal way to inform the players on stat transformations? Specifically, in the F4 stat panel and stat tooltips? And in relation to our possible candidate stat transformations $f(x)$? Let's look through the alternatives and see what is the best one.

First, possible levels of information deepness.

1. Minimal approach, employed by some other games, e.g. one quite successful rogue-lite bullet heaven, just north of 1 million copies sold on Steam, is just to specify that there is a transformation and show the final effective stat value.
    
    With our example it would be something like: "Reduction in energy cost for all melee weapon abilities, with diminishing effect at higher values."
    
    Effectively conveys the truth of the situation, without burdening the player with additional info to process.

2. Middle ground approach, the one we've already seen above, specify that there is a transformation, that we explicitly transform the stat to be under 100%, and show the rate of changes.

3. Expanded approach, try to convey even more information on the transformation, as much as possible info on the computation.
    
    Might not work with tooltips, but we'll see.

There's also a question of percentages and points, if we get the final effective stat percentage value by modifying an incoming total, do we need the source values from items, passives, statuses etc. be dimentionless points, like it is with accuracy and dodge?

I surmise we actually do not need that, given that percentage modification is already in the game for quite a long time, when we get Fire/Ice Resist % source from the Physical Resist % and there's absolutely no confusion about that, never seen a player ask for clarification on that; but for completeness' sake we can consider following alternatives:

1. Employ percentage into percentage stat transformation design.

2. Require for percentage stats with transformation that incoming source values are dimentionless (not in the strict sense, just as a label) points.

And of course we should define our criteria for comparison. We are trying to determine the optimal way of informing the players, so that they would get as complete as possible idea of how stats work though as little as possible effort. It's essentially a problem of educational nature, so it seems reasonable to use foundational educational principles:

1. If we would like to unpack a conceptual parcel for the audience to grasp, understand and internalize, we better split it in such a way that the path to understanding is a sequence of conceptually easier, even as easy as possible all other things permitting, steps, even if after some steps audience's understanding would be incomplete or wrong in some aspects.
    
    Illustrative example 1: Basic arithmetic.
    
    Students in primary school start with counting sticks and counting up and down one by one, getting the concept of natural numbers; then there are addition and subtraction, but subtraction is not full-domain, can't subtract larger from smaller; then there are negative numbers, and can subtract larger from smaller; then there's multiplication and division, can't divide just by anything though; then there's division with remainder; then there are fractions and proper division;
    
    so there are multiple paradigm shifts of the form "It's actually not like you thought it was before, it's not so simple, it's actually like this, and the thing we told you you couldn't do is actually possible."
     
    Illustrative example 2: Atom model in physics/chemisty education.
    
    Education starts with a simple planetary model, then changes to electrons as clouds model, and then actually refines to proper mathematical electron wavefunction spherical harmonics model with complex probability amplitudes.
    
    Illustrative example 3: C compilation details in CS education.
    
    When students are presented a C "Hello, world!" program for the first time, we can hear things like "This is the main function, you need it for the program to work" and "This include thing makes possible to use printf here, you can think of it as a sort of analogue of Python's import or, better yet, just something that's required for the printf" and "To run the program, do this";
    
    and only later the students are informed that "this" is actually multi-stage compilation process, involving preprocessing, compilation and linking, that the main function is an entry point and what entry point is and that you can actually specify arbitrary entry point when linking, that include directive is for the preprocessor and it actually just pastes printf function definition into the compilation unit and how the actual printf function in the form of its object code is linked during linking;
    
    and then that there's the whole other pile of matters relating to run-time linking and shared libraries.
    
    Obviously our stat transformation matters are much lighter, but the principle is the same.
    
2. Don't actually make the audience spend attention and mental effort without relevant need.
    
    Somewhat related to the 1st principle, but actually stands and is useful on its own.

And now we can go through our candidate stat transformations $f(x)$, starting with the 2nd, the piece-wise continuous one, as it has previously shown most promise by non-player-information considerations.

Note also the 3rd and 1st candidate $f(x)$ are both continuous and would only differ in presentation in specific values, so with them we could restrict our comparisons to only the 3rd, shown previously to be second best by non-player-information considerations.

#### Piece-wise linear

With our piece-wise linear stat transformation we can immediately notice that, as it's 1-to-1 up to the total incoming source value $x$ of 50%, we actually have the option to delay informing the player of the transformation until the incoming source value would actually exceed the threshold of 50%.

It's in line with the 2nd principle, it's better to not set up the player for spending additional attention and mental effort on engaging stat transformation until it would actually be relevant.

So, with piece-wise linear transform we have additional alternatives:

1. Do not show the transform information until there's an actual transform happening.

2. Show transform information regardless of magnitude of total incoming source value $x$.

And now there's nothing but just go through the variants, through I'll try to order them roughly from more optimal to less optimal based on general considerations according to our criteria.

1\.

Do not show transform until relevant (1.)

Before 50% of total incoming source $x$:

1.1.

Do not show transform until relevant (1.)
Percentage into percentage computation (1.)

Example tooltip:

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%
```

1.2.

Do not show transform until relevant (1.)
Incoming source values are dimensionless (2.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 40

** Cost Reduction **

40%
```

Note that there is a conceptual jump from incoming dimentionless source to the final percentage stat value requiring some measure of player's attention and mental effort, even if it's obvious.

How dimentionless values could look at some source tooltips, partial examples:

```
# Martial Focus #

Each warrapt level gives +0.25% damage and +0.25 melee and ranged ability cost reduction.
```

```
# Efficient Dispatch #

Reduces the energy cost of all melee and ranged abilities by 9.
```

```
# Bludgeon Specialist #

Reduces the energy cost of all melee abilities by 25.
```

Last two look off, not that good, so we'd need to somehow modify this, probably to:

```
# Efficient Dispatch #

+9 melee and ranged ability cost reduction.
```

```
# Bludgeon Specialist #

+25 melee and ranged ability cost reduction.
```

After 50% of total incoming source $x$:

1.1.1.

Do not show transform until relevant (1.)
Percentage into percentage computation (1.)
Expanded information (1.)

Note: two decimals used here are consistent with the same amount in move speed and attack speed tooltips, but if any amount of decimals here and forward is too much for your taste, can always round more and leave less decimals.

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional source percent point

** Computation **

75% =
50% + 25% →
50% + 25% / 3 =
58.33%
```

How this would look at higher values:

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Equipment: 38%
Status Effects: 35%
  Stand Ground: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 8%

Total: 115%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 69.17%

+0.17% per additional source percent point

** Computation **

115% =
50% + 50% + 15% →
50% + 50% / 3 + 15% / 6 =
69.17%
```

Here there's also a conceptual jump involving understanding how the final stat value is computed from the total incoming source value, and how increase in total source value would translate to increase in the stat value, but it's easier than the previously mentioned jump from dimentionless total source to the stat percentage due to explanation explicitly stated in clear text and the explicit demonstration of the computation.

Now a question arises, is there now a need, in situations when the stat's total incoming source is greater than 50%, to somehow note in all of the stat's percentage sources that this source value may not be included in the final stat value in 1-to-1 scale?

No, there is not much need, it would be more trouble than it's worth.

As soon as the player sees and understands the tooltip with with "Modified total source cost reduction…" explanation and computation demonstration, either by chance or by investigating after noticing discrepancy between new added source percentage and apparent stat increase — and that's a good thing, it's uncovering the game's deeper layers and is rewarding — a conceptual separation between source percentages and the final stat percentage is established in the player's mind.

This mental separation is enforced due to:

1. There being two pairs of different values, total source percentage (75% in the example tooltip) and final stat value (58.33%) and a source percent point, 1%, and corresponding final stat value increase (+0.33%) — these are obviously not the same numbers, and so source percentages and final stat value percentages are obviously different kinds.

2. An explicit description stating how one percentage is a product of processing — scaling — of another one; how, one could say, a final stat percentage is prepared from the source percentage in the same conceptual manner as e.g. how food ready for consumption is prepared from its raw kind.

3. An explicit demonstration how the preparation process works and how indeed one percentage is taken apart, worked on and rearranged into another completely different percentage.

And consequently additional explicit tooltip notes to the same effect would only be boring clutter being player's attention sink.

Though for completeness' sake, if it would be needed, it probably could be something like dynamically adding a short text to the tooltips, something like this:

```
# Martial Focus #

Each warrapt level gives +0.25% damage and +0.25% melee and ranged ability cost reduction (with diminishing returns at higher totals).
```

```
# Efficient Dispatch #

Reduces the energy cost of all melee and ranged abilities by 9% (with diminishing returns at higher totals).
```

```
# Bludgeon Specialist #

Reduces the energy cost of all melee abilities by 25% (with diminishing returns at higher totals).
```

1.1.2.

Do not show transform until relevant (1.)
Percentage into percentage computation (1.)
Middle ground information (2.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional source percent point
```

The same argument on conceptual separation and the unneededness of additional notes in source tooltips as in 1.1.1. variant apply. Even if the separation might be not as quick to be established without the explicit demonstration of the computation, it would still be as firm once the understanding is achieved, the understanding would just require maybe several seconds more to be found.

1.1.3.

Do not show transform until relevant (1.)
Percentage into percentage computation (1.)
Minimal information (3.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Diminishing effect at higher values:* 58.33%
```

Here the conceptual separation of the source percentage and the final stat percentage is again made slightly harder to establish, but again it's still explicit due to explicitly shown different numbers, again would just need slightly more time to understand.

1.2.1.

Do not show transform until relevant (1.)
Incoming source values are dimensionless (2.)
Expanded information (1.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35
  Savage Efficiency: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 75

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional source point

** Computation **

75 =
50 + 25 →
50% + 25% / 3 =
58.33%
```

How this would look at higher values:

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Equipment: 38
Status Effects: 35
  Stand Ground: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 8

Total: 115

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 69.17%

+0.17% per additional source point

** Computation **

115 =
50 + 50 + 15 →
50% + 50% / 3 + 15% / 6 =
69.17%
```

Need to note that just as with percentage to percentage computation, there's a conceptual jump in understanding how the final stat value is computed from the total incoming source value.

1.2.2.

Do not show transform until relevant (1.)
Incoming source values are dimensionless (2.)
Middle ground information (2.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35
  Savage Efficiency: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 75

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional point
```

1.2.3.

Incoming source values are dimensionless (2.)
Minimal information (3.)

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35
  Savage Efficiency: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 75

** Cost Reduction **

*Diminishing effect at higher values:* 58.33%
```

Alternatives 2.1.1. — 2.2.3., when we always show transform information, regardless if the total incoming source value $x$ is less or greater than 50%, look the same and have the same conceptual jumps as alternatives 1.1.1. — 1.2.3., with an added drawback of frontloading the transform complexity and therefore being more insistent on player's attention and mental effort.

Also perhaps for alternatives 2.1.3. and 2.2.3 with minimal information better to use "Effect with diminishing returns at higher values: X%" instead of "Diminishing effect at higher values: X%" so that when there is 1-to-1 correspondence with total incoming source value is less than or equal to 50%, there is no confusion cause "Diminishing effect…" sort of implies the diminishment is present, while below 50% there is none.

Let's see summary of the drawbacks of each variant, with following key:

|     | | Expanded | Middle | Minimal |
| --- | --- | -------- | ------ | ------- |
| **Not until relevant** | **Percentage** | C1 | C1+ | C1++ |
| | **Dimensionless** | C2,M | C2+,M | C2++,M |
| **Show regardless** | **Percentage** | C1,F | C1+,F | C1++,F |
| | **Dimensionless** | F,C2,M | F,C2+,M | F,C2++,M |

C1 — conceptual jump for understanding that total source value percentage is computed into a different kind of percentage of the final stat value.

C2 — conceptual jump for understanding that dimentionless total source value is converted to the final percentage stat value.

+, ++ — additional drawbacks due to less information with middle and minimal information options.

M — need to adjust source tooltips for dimentionless values, e.g. "Reduces the energy cost of all melee and ranged abilities by 9." -> "+9 melee and ranged ability cost reduction.".

F — drawback of frontloading transformation info and being more insistent on player's attention and mental effort.

As it was argued above, I take C2 conceptual jump to be no less easy than the C1 conceptual jump.

Well, among all the alternatives with piece-wise linear transform, my preference is probably already obvious, it's 1.1.1. with not showing transformation information until it's relevant, leaving source values as percentages and expanded transformation information.

#### Continuous

As opposed to piece-wise linear transformation, with continuous transformation there's no exact region of 1-to-1 correspondence at all, so we have to always show transformation information.

And with continuous transformations we actually can't really show how computation works in a way that would be fit for a tooltip; maybe it can be placed in a section of more involved in-game help or tutorial, but with unsuitability for tooltips it means we don't have an option of expanded computation information.

So, we actually have only four variants, percentage / dimensionless incoming source values and middle / minimal transformation information.

Here are example tooltips, with stat values computed according to the 3rd candidate stat transform, the slightly faster growing continuous one:

1.1. Percentages, middle information.

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 53.75%

+0.42% for additional source percent point
```

Note subtle difference in stat rate of change report, "for additional source…" instead of "per additional source…", as with continuous transforms rate of change changes with even small total incoming source value changes, as opposed to piece-wise linear transform where it stays constant for large intervals of total incoming source values.

1.2. Percentages, minimal information.

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Effect with diminishing returns at higher values:* 53.75%
```

2.1. Dimensionless, middle information.

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35
  Savage Efficiency: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 75

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 53.75%

+0.42% per additional point
```

2.2. Dimentionless, minimal information.

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35
  Savage Efficiency: 35
Passive Effects: 34
  Bludgeon Specialist: 25
  Efficient Dispatch: 9
Skill Bonus: 6

Total: 75

** Cost Reduction **

*Effect with diminishing returns at higher values:* 53.75%
```

With absolutely the same arguments as for piece-wise linear, here's comparison table:

| | Middle | Minimal |
| --- | ------ | ------- |
| **Percentage** | C1,F | C1+,F |
| **Dimensionless** | F,C2,M | F,C2+,M |

C1 — conceptual jump for understanding that total source value percentage is computed into a different kind of percentage of the final stat value.

C2 — conceptual jump for understanding that dimentionless total source value is converted to the final percentage stat value.

\+ — additional drawback due to less information with minimal information option.

M — need to adjust source tooltips for dimentionless values, e.g. "Reduces the energy cost of all melee and ranged abilities by 9." -> "+9 melee and ranged ability cost reduction.".

F — drawback of frontloading transformation info and being more insistent on player's attention and mental effort.

And again with the same arguments, from the variants available for continuous transformation, it seems the 1.1. with percentages and middle information is the best, though it loses to piece-wise linear 1.1.1. variant.

#### Suggested variant

So, overall, based on criteria of a) balancing, b) satisfaction from stat growth, and c) player information, I would suggest for melee ability cost reduction and other inversely scaling attacking stats, like ranged ability cost reduction and nature magic ability cost reduction, a piece-wise linear stat transformation of the form
$$
f(x) = 1 - \frac{1}{\lfloor 2x + 1 \rfloor} + 2 \, (x \bmod ½) \left[ \frac{1}{\lfloor 2x + 1 \rfloor} - \frac{1}{\lfloor 2x + 2 \rfloor}\right]
$$
giving the stat value $x = f(x)$ from total incoming source value $x$, with conditional showing of the transformation info in the stat tooltip, with expanded transformation info.

While in the 1-to-1 region, with total incoming source value $x \le 50\%$, show the tooltip as it is now, e.g.:

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%
```

When the transformation actually takes place, with total incoming source value $x > 50\%$, show transform info in the tooltip:

```
# Melee Cost Reduction #

Reduction in energy cost for all melee weapon abilities.

** Sources **

Status Effects: 35%
  Savage Efficiency: 35%
Passive Effects: 34%
  Bludgeon Specialist: 25%
  Efficient Dispatch: 9%
Skill Bonus: 6%

Total: 75%

** Cost Reduction **

*Modified total source cost reduction, scaled to under a maximum of 100
%:* 58.33%

+0.33% per additional source percent point

** Computation **

75% =
50% + 25% →
50% + 25% / 3 =
58.33%
```

As per arguments stated above, this is the best variant with the best way to deliver understanding of how stat scaling works to the player.

Though if we would like even more sureness that the player would have clarity and understanding, we could add a tutorial which would appear the first time the total source value if any stat with such a transform would get high enough and the stat transformation would actually take place, but how to go about the optimal way to have tutorials about this and in general is the whole separate question for a separate section.

### Defensive abilities and stats

Now that we mentioned Physical Resist in the previous section as an example of how the game already has percentage to percentage computation, it's a good opportunity to start talking about balancing defensive scaling abilities, like Chivalry's Bravery (+0.25% physical resist per Chivalry level) and defensive stats in general.

For fractional defensive stats, which go from 0% to 100% and which either prevent a portion of an incoming negative effect, like Physical Resist and other damage resists, or give a chance to negate an incoming negative effect, like wound resists or e.g. missile deflection, it's better to also have a scaling stat transform like with inversely scaling attacking abilities like melee cost reduction, though perhaps not of the same general shape.

Better for 2 reasons:

First, it's better for player's satisfaction.

With stat transform any additional skill levels giving slightly more of the source stat value through unbounded scaling abilities would never feel useless, would always give some satisfaction.

And other sources of the stat would also never feel useless or partially useless — like e.g. with Physical Resist which you could pretty easily get to above 100% and e.g. Dreadheart's Dogged Resolve triggered effect suddenly loses some of its value in situations where Fire/Ice Resists are not relevant, the same to a partial extent with Quartermastery's Maintain Uniform, it may feel less useful, and when when you find out an enchanted item you just got has Physical Resist it may take some wind out of your sails, like: "Oh, an enchanted loot, very nice! ... Ah, it's Physical Resist, ok."

When a stat presses against or goes over the hard threshold, it has an adverse effect on satisfaction from every source of the stat, so better not to let the stat to that by introducing a source -> stat transform allowing for unbounded stat source values and letting the stat to approach the threshold asymptotically instead of pressing against it or going over it.

Second, it's better for the balance and feel of the game.

Currently the >100% Physical Resist tank build is the most powerful build, you get it, the game is easy. Yeah, there's armor penetration from crits and from more unusual enemies, and from non-physical damage, but overall it's busted. It would be good to not let it be a perfect defense even in some situations, to make it so that there's always an avenue of damage from even simple physical damage enemies, even if however small, by making the Physical Resist stat only approach 100% asymptotically.

And the same for other proportional defense or chance defense stats, better for the balance and feel of the game to not let them approach 100% defense or 100% chance to defend, better let them approach 100% only asymptotically.

Alright, if we are to have that asymptotic behaviour, at what rate it should go for optimal player satisfaction?

Unlike with attacking abilities, for defensive abilities we don't have to balance satisfaction from stat increase and increased stat effects with possible loss of satisfaction from decrease of the game's challenge.

For defensive stats, any increase of the stat's defensive effect brings satisfaction, and game becoming easier due to that is perceived as desirable and satisfactory, no matter how good the defense becomes, because it's the primary reason of the defensive stats to make game easier. However good they become, there's never a feeling that something is now broken or out of balance — if we restrict our view to the stats themselves of course, and not their sources.

That means that for optimal player satisfaction which would work for any unbounded incoming stat values, allowing extended progression from unbounded scaling abilities with it's associated primary satisfaction and second-order satisfaction from anticipation, we just have to sort of stretch improvement from incoming source stat values in constant-feeling manner all the way to infinity.

Here I don't have a definitive answer, but if you think about it, what is the constant progression of a proportional defensive stat? What does it mean that each additional set quantity of incoming source stat value improves the proportional defense the stat provides by the same amount? And it feels right that for the proportional defense to improve by the same amount means that it reduces incoming negative effect by the same factor.

And so, we arrive at our desired asymptotic behavior for defense stat $s$ computed from a total incoming source value $x$ with a transform $s = f(x)$, the transform $f(x)$ should have an asymptotic exponential attenuation, $1 - f(x) \sim e^{-x}$.

Just like with inversely scaling attacking stats, we also would like for our transform to have additional obvious natural properties, like having 1-to-1 or being close to 1-to-1 linear relation at the origin and to gradually decrease, $f(0) = 0$, $f'(0) = 1$, $f''(x) \le 0$.

And just like with inversely scaling attacking stats, we can look at more than one candidate transform:

1. Simple with required asymptotic behaviour, continuous:
    $$
    f(x) = 1 - e^{-x}
    $$
    
2. Of the same general shape, but with piece-wise linear growth and slightly faster:
    $$
    f(x) = 1 - 2^{-\lfloor 2x \rfloor} + 2 \, (x \bmod ½) \left[ 2^{-\lfloor 2x \rfloor} - 2^{-\lfloor 2x + 1 \rfloor} \right]
    $$
    
    Can be computed with one-liner:
    
    `=1-2^(-FLOOR(2*X))+2*MOD(X,0.5)*(2^(-FLOOR(2*X)) - 2^(-FLOOR(2*X+1)))`
    
3. Also continuous, at the simple one, but with rate of growth closer to the piece-wise linear one, even slightly faster at higher $x$, perhaps faster than necessary:
    $$
    f(x) = \tanh x
    $$

![[defense_123.png]]

And again just as with inversely scaling attacking stats, can compare our candidate transforms on considerations of a) balancing, b) satisfaction from stat growth and c) player information.

And again for the same reasons the piece-wise linear transform seems the best.

#### Suggested variant

So for proportional defensive stats that vary from 0% to 100% I would suggest a piece-wise linear stat transformation of the form
$$
f(x) = 1 - 2^{-\lfloor 2x \rfloor} + 2 \, (x \bmod ½) \left[ 2^{-\lfloor 2x \rfloor} - 2^{-\lfloor 2x + 1 \rfloor} \right]
$$
with conditional showing of transformation info in the stat tooltip, with expanded transformation info.

Within the 1-to-1 region, with total incoming source value $x \le 50\%$, show the tooltip as it is now, e.g.:

```
# Physical Resist #

The percent of physical damage reduced from incoming attacks after taking into account protection

Note, that attacks with armor penetration will directly counteract physical resist.

** Sources **

Equipment: 44%
```

When the transformation actually takes place, with total incoming source value $x > 50\%$, show transform info in the tooltip:

```
# Physical Resist #

The percent of physical damage reduced from incoming attacks after taking into account protection

Note, that attacks with armor penetration will directly counteract physical resist.

** Sources **

Equipment: 162%
Status Effects: 78.5%
  Dogged Resolve: 30%
  Guarded Wait: 25%
  Bravery: 15.5%
  Maintain Uniform: 8%
Passive Effects: 6.87%
  Battle Hardened: 6.87%

Total: 247.37%

** Resist **

*Modified total source resist, scaled to under a maximum of 100
%:* 96.71%

+0.06% per additional source percent point

** Computation **

247.37% =
50% + 50% + 50% + 50% + 47.37% →
50% + 50% / 2 + 50% / 4 + 50% / 8 + 47.37% / 16 =
96.71%
```

There's an additional question of inter-stat scaling, like e.g. when Ice and Fire Resist has a source which scales off the Physical Resist; for such situations the scaling source should scale off the source stat's source total, e.g. with the example above Fire Resist would get a 247.37% / 4 bonus source off Physical Resist and would show the following:

```
# Fire Resist #

The percent of damage reduced from incoming fire damage.

25% of your physical resist is added as bonus fire resist.

** Sources **

Physical Resist: 61.84%

Total: 61.84%

** Resist **

*Modified total source resist, scaled to under a maximum of 100
%:* 55.92%

+0.5% per additional source percent point

** Computation **

61.84% =
50% + 11.84% ->
50% + 11.84% / 2 =
55.92%
```

And as a final note, perhaps the 'defensive' label when talking about scaling transforms for defensive stats is a too restrictive misnomer, the reasoning in this and the previous section applies to all inward-facing fractional stats, which govern player's capabilities to manage incoming effects other things are causing to be aimed at the player.

### Joint and thematic scaling

Going back to our example of the set of stats affecting direct damage capability — +% damage, crit chance, crit bonus damage, repeat attack chance, multi-attack chance, +min/max damage bonus — and how they raise this capability multiplicatively, which gives us a reason to look at the question of if they really all should scale linearly.

And as some of these stats are percentage attacking stats, let's actually engage with this wider question, should percentage attacking stats have scaling transforms, and if they should, what kind? Perhaps, just as with defensive or better say inward-facing stats, the 'attacking' category is not exactly right and it's better to talk of outwardly-facing percentage stats, which govern effects player imposes on other things.

There are two broad categories of outward percentage stats, for some it may make sense to have values of over 100%, for others it is nonsensical. While it may actually be that for some stats it is not a forgone conclusion to which category they belong, and it is for the developers of the game to decide for the stat which category is better, the answer to our current question of whether to use scaling transform and if yes, which, would depend on the category of the stat and therefore each stat should be assigned a category.

Consider the Crit Damage stat, it emphatically makes sense to be possible for it to have values over 100%.

For Multistrike, Repeat Attack Chance and Crit Chance possibility of them having values of 100% also makes sense, but not to the same extent.

If Multistrike has value X% = 100% + x%, it could be that then it's 100% damage attack on a random adjacent target and then an additional x% damage attack on another distinct random adjacent target, if present. If Multistrike is X% = 200% + x%, then it's two 100% damage attacks on distinct random adjacent targets and an additional x% damage attack on another also distinct adjacent target, and so on. Or it could be that if Multistrike is X% > 100% and there are at least two additional adjacent targets, X% is split randomly into two portions as X% = x1% + x2%such that x1, x2 ≤ 100% and two random distinct adjacent targets are dealt attacks of x1% and x2% damage, and if Multistrike is X% > 200% it's split randomly into three portions, and so on. Note, in such cases should update Multistrike description along with its mechanics.

For Multistrike, Repeat Attack Chance and Crit Chance possibility of them having values of 100% also makes sense, but not to the same extent. E.g. if Multistrike has value X% = 100% + x%, it could be that then it's a guaranteed attack on a random adjacent target and an x% chance of an additional attack on another random adjacent target, if present. If Multistrike is X% = 200% + x%, then it's two guaranteed attacks on random adjacent targets and an x% chance of an additional attack, and so on. Note, in that case should change it's description along with its mechanics to something like ""

If Repeat Attack Chance has value X% = 100% + x%, it could be that it's a guaranteed repeat attack and then an x% chance of additional repeat attack. And if Repeat Attack Chance if over 200%, there will be a certainty of two repeat attack and a chance for additional third repeat attack, and so on.

And for Crit Chance, if it's over 100%, it could be that there will be a certainty of it's application, meaning +Crit Damage % of damage and +50% of Armor Penetration, and a chance for it's second application, meaning additional +Crit Damage % of damage and another +50% of Armor Penetration; if Crit Chance if over 200%, two certain applications and a chance for the third and so on.

Or, even though I would advocate against it, for any of these three stats it can be decided that no, it's better to not allow for it to go over 100%. If it's because such over 100% overflow mechanics seems too powerful, there's a possibility of using slightly dampening stat scaling for such stats, stay tuned.

Armor Penetration on the other hand is complete opposite, it emphatically doesn't makes sense for it to have values over 100%, it should be confined into \[0%, 100%) interval.

#### Possible overflow stat scaling

If we'd like to allow a stat to go over 100%, but still would like to limit the overflow somewhat, what can we do?

Easy, just dampen stat growth above 100%.

Given proven track record of piece-wise linear stat transformations, as we've seen with inverse attacking stats and defensive stats, I suggest following piece-wise linear stat transform with logarithm-like asymptotic scaling for stats for which the dampening of the growth above 100% is deemed necessary:
$$
f(x) = \left \lfloor \log_2 (1+x) \right \rfloor + (1 + x) 2^{-\left \lfloor \log_2 (1+x) \right \rfloor} - 1
$$

The transform is 1-to-1 up to 100% and then gradually slows down, see how it compares to the base 2 logarithm:

![[overflow.png]]

I would suggest such overflow dampening for Crit Damage, Crit Chance and Repeat Attack Chance, to limit possible multiplicative effect of joint attacking stat scaling mentioned before. For consistency it could apply also to Multistrike, but there's a possibility of leaving its growth undampened as it's too cool an effect to dampen and, moreover, as it's naturally constrained by the number of adjacent enemies.

Just like with transforms of inverse attacking and defensive stats, there's no need to show transform info if it doesn't actually take place. Before 100% it could look just as it is now:

```
# Multistrike #

The percent of damage dealt to a random adjacent target.

** Sources **

Status Effects: 60%
  Street Sweeper: 60%
```

After 100% it could look just as with inverse attacking and defensive stats, something like this:

```
# Multistrike #

The percent of damage dealt to random adjacent targets.

** Sources **

Equipment: 10%
Status Effects: 198%
  Street Sweeper: 100%
  Prepare for Onslaught: 98%

Total: 208%

** Damage **

*Modified total source damage, with diminishing returns at higher values:* 154%

+0.5% per additional source percent point

** Computation **

208% =
100% + 108% ->
100% + 108% / 2 =
154%
```

As it was already said, such overflow stat scaling could apply to any outward-facing percentage stat for which it would make sense to go over 100%, like e.g. to a chance to collect a Botany flower/mushroom resource, for which it could be that if it's over 100%, you are certain to collect the resource and then have an overflow chance to get an additional resource item.

#### Possible confined stat scaling

As we said, Armor Penetration should be confined to the interval \[0%, 100%). For same arguments as for defensive percentage stats, like Physical Resist, for better player's satisfaction Armor Penetration sources should be allowed unbounded scaling over 100% and beyond, and the stat itself should be derived from sources by a scaling transform.

The question is, what scaling transform $f(x)$? It seems just as with defensive stats, there's no firm justification, but we can say that we would just require a transform which would sort of stretch any values of unboundedly increasing total source value into a constant-feeling improvement of the resulting stat value confined to the interval \[0%, 100%), and that it would be a transform with exponential attenuation, $1 - f(x) \sim e^{-x}$.

And for the same arguments as when we considered possible transforms for defensive stats, the best transform variant would be the piece-wise linear transform chosen for defensive stats:
$$
f(x) = 1 - 2^{-\lfloor 2x \rfloor} + 2 \, (x \bmod ½) \left[ 2^{-\lfloor 2x \rfloor} - 2^{-\lfloor 2x + 1 \rfloor} \right]
$$

And it's information can be relayed to the player in the same way, not actually shown when the total incoming source is up to 50%, and shown with computation details when the total source is greater than 50%.

Of course the same transform can and should be used with other outward-facing percentage stats for which it is sensible to be confined to the interval \[0%, 100%), like e.g. Cooking's chance to create a superb version of the food.

### Ability balancing procedure

And now we can finally return to the initial question, how to balance unbounded scaling abilities in a general way.

Now that we have stat transforms that take care of asymptotic balancing in general, for abilities we only have to, as was already said all the way back, balance them at skill level 50, with consistency check at skill level 100, and then the asymptotic stat transform balancing will do it's work.

As an aside, why skill level 50 specifically? It's because that it's sort of a natural cut-off point for skill, as all of the skills can be completed or almost completed by level 50, and a natural cut-off point for the game contents, based on the assumption that with a normal gameplay player would be able do every unique content of the game before hitting level 50 in character levels or any skill levels.

So if the player get to level 50 and above, that's an additional non-required progression they went for, and therefore should be rewarded that.

And level 100 is because for the unbounded abilities of the 1st kind it's a natural comparison point to the situation at skill level 50, with having twice as much skill levels, and with roughly 50 new focus points available for the abilities of the 2nd, 3rd and 4th kind, just as there were 50 skills levels for the abilities of the 1st kind at skill level 50.

And if the assumption that all the unique content is doable before or by char level 50 and main skill level 50, need just to raise the level of comparison slightly higher, to level 55 or 60 or so on.

As unbounded scaling abilities depend on their skill level, it would also make sense look at how balanced they are not only individually, but as a whole for a particular skill, at least for unbounded abilities of the 2nd, 3rd and 4th kind even if they affect different stats, as abilities of these 3 kinds compete for a single source of the skill's focus points.

For example, let's look at Warrapt.

It already has an unbounded scaling ability of the 1st kind, it's foundational passive Martial Focus: +0.25% damage, +0.25% melee and ranged ability cost reduction per skill level.

Can suggest following additional unbounded scaling abilities to be acquired mid-playthrough — quite a large number, but then the Warrapt is a general combat skill, and there are many facets to combat:

- 1% swap time reduction per unspent fp.

- 1% less time to enter a stance per unspent fp.

- 1% less time to perform all melee and ranged abilities per unspent fp.

- +1% crit prevent chance per unspent fp.

- +1% physical resist per ability level, linear fp scaling.

- +1% multistrike per ability level, linear fp scaling.

- +1% repeat attack chance per ability level, linear fp scaling.

- +1% crit chance per ability level, linear fp scaling.

- +1 protection when using a shield and/or armor, up to the limit of (base protection from shield + base protection from armor / 2), quadratic fp scaling.

Warrapt's full complement of abilities requires 52 focus points to unlock, so we can say with confidence that at skill level 50 any additional unbounded abilities would have only negligible effect, if at all, so can only look at the Martial Focus.

At Warrapt level Martial Focus would give +12.5% damage and +12.5% ability cost reduction, which feels underwhelming compared to the effort required to reach Warrapt level 50 and compared to other bonuses of the same type from other skills.

Reaching Warrapt level 50 requires quite a commitment, consistently using skill points from character level up to prop Warrapt and constantly using Warrapt's xp giving abilities in combat, so seeing only 12.5% ability cost reduction from all this effort compared to e.g. 25% – 35% from a single ability Savage Efficiency from Dreadheart, or 35% from a single ability Stand Ground from Chivalry feels unbalanced. Yeah, these two abilities are situational while Warrapt's bonus is permant and constant, but compare the effort and work required to reach Warrapt level 50 and just get one of these two abilities, there's obvious discrepancy.

The same, though to a lesser extent, is true for the +12.5% damage bonus. Again, Warrapt is general while e.g. Swords specific weapon mastery is, duh, specific, but then if the Swords are your main weapon I would wager you'd reach Swords level 50 no later, and maybe sooner, than Warrapt level 50, and Swords level 50 would give +50% damage compared to the measly +12.5% damage from Warrapt level 50.

So overall, we can buff this scaling ability somewhat, and make it give +0.5% damage, +0.5% melee and ranged ability cost reduction per Warrapt level.

Now let's see how our scaling abilities would work at Warrapt level 100, separately and jointly.

Though before that we'd need to note that getting to Warrapt level 100 from Warrapt level 50 is almost three times as much xp and therefore time and effort as getting to Warrapt level 50.

Abilities at Warrapt level 100, separately:

- +50% damage, +50% ability cost reduction.
    
    Doesn't seem an unbalanced result of reaching Warrapt level 100.

Now all the next abilities require function points, so only one of the following would actually be possible at Warrapt level 100, to the exclusion of everything else. And let's round available focus points from 48 to 50.

- Unspent focus points scaling abilities, the 4th kind, they are active together simultaneously:
    
    50% swap time reduction.
    50% time to enter a stance reduction.
    50% time to perform a melee or ranged ability reduction.
    +50% crit prevent chance.
    
- +50% physical resist.

- +50% multistrike.

- +50% repeat attack chance.

- +50% crit chance.

- +up to 9 protection (9 ability levels from 1 + … + 9 = 45 focus points) when using a shield and/or armor, up to the limit of (base protection from shield + base protection from armor / 2).
    
    Note that as full Adamant armor without shield gives 11 protection, so would get only +5.5 protection from the ability with that.
    
    If we add a shield with 3 protection, the bonus would get to +3 +5.5 -> +8.5, so to fully use the ability need to either use the 4 protection shield or add enchantments to the shield/armor.

Each of the options, remembering the stat scaling, doesn't seem unbalanced as a result of reaching Warrapt level 100.

Now if we would look at Warrapt scaling abilities together, we don't need to re-examine the foundational passive, as it's not affected by focus points, but all the other scaling abilities would share focus points, and with roughly equal distribution we would get something like that, all together:

- 8 unspent focus points:
    
    8% swap time reduction.
    8% time to enter a stance reduction.
    8% time to perform a melee or ranged ability reduction.
    +8% crit prevent chance.
    
- +9% physical resist (9 spent focus points).

- +9% multistrike (9 spent focus points).

- +9% repeat attack chance (9 spent focus points).

- +9% crit chance (9 spent focus points).

- +up to 3 protection (3 ability levels from 1 + 2 + 3 = 6 spent focus points).

Doesn't seem unbalanced as a result of reaching Warrapt level 100.

And so, unless the analysis missed somehting, we can conclude that proposed set of unbounded scaling abilities acquirable mid-playthrough for Warrapt seems like a not bad fit.

Final note, do we need cross-skill balancing, i.e. do we need to check how e.g. unbounded abilities from two skills both at level 50 and/or level 100 work together? In general, no, as above we are relying on assumption that our comparison baseline is level 50 for one main skill, before or at which you can do all the unique content in the game. Again, if the assumption does not hold, could raise single skill comparison level to 55 or 60 or beyond.

## Possible transforms for stats

General procedure for determining if a stat needs a scaling transform:

1. Is the stat outward-facing, attacking?
    
    1. Is the stat inversely scaling, like ability cost reduction?
        
        Transform with hyperbolic attenuation, like suggested for Melee Cost Reduction.
        
    2. Is the stat to be confined to the interval \[0%, 100%)?
        
        Transform with exponential attenuation, like suggested for Physical Resist.
        
    3. Is the stat to have overflow scaling?
        
        Transform with logarithm-like scaling, like demonstrated for Multistrike.
        
    4. Otherwise, no need for a transform.
    
1. The stat is inward-facing, defending.
    
	1. Is the stat percentage-based?
        
        Transform with exponential attenuation, like suggested for Physical Resist.
        
    1. Otherwise, no need for a transform.

And now, even if incomplete, lists of possible scaling transforms for outward-facing and inward-facing stats.

If required, could make the lists complete by considering every stat.

### Outward-facing, attacking

- Accuracy.

That's a bit of a special case, as it already has it's own transform, which for high enough source accuracy is the A>D branch of the accuracy formula, which, taking 100 (accuracy - dodge) points as a unit $x$, is:
$$
f(x) = 0.75 + \frac{x}{((4x)^{1.25} + 1)^{\frac{1}{1.25}}}
$$

Accuracy is an outward-facing, attacking stat with direct relation to capability, the larger accuracy is, the more capable player of dealing damage and the less is difficulty of the combat, so it would be good with either no transform at all or a transform that would give slight logarithm-like dampening at high values.

But, asymptotically for large enough $x$, the accuracy formula transform scales as $f(x) \sim 1 - 1/x^{1.25}$, which is just effectively constant, nowhere to the usual scaling of the usual direct attacking stats; but that's due to the accuracy's special nature.

Probably needs more involved analysis, but at least that means that unbounded scaling abilities of the 1st kind of the form +1 accuracy per skill level, or of the 2nd kind, +1 accuracy per ability level with linear focus point scaling, ability level per spent focus point, or of the 4th kind, +1 accuracy per unspent focus point, are completely fine from player's satisfaction point of view, they would give satisfaction from steadily raising accuracy points and won't lead to loss of satisfaction from the loss of challenge from too fast decreasing difficulty.

- Armor Penetration.

Exponential attenuation.

- Attack Range.

Obviously no transform.

- Attack Speed.

Has it's own hyperbolic-like attenuation transform due to it's nature, the speed of movement over a distance by time, doesn't need any additional transform.

Unbounded scaling abilities of the 1st kind, +1 attack speed per skill level, of the 2nd kind, +1 attack speed per ability level, ability level per 1 spent focus point, or of the 4th kind, +1 attack speed per unspent focus point, are completely fine.

- Bleed Chance.

Straight up attacking ability, with each bleed wound expected to bring some amount of damage, could compute on average but don't remember exact probabilities of healing, so it's just a parcel of damage over time.

Based on that, can have logarithm-like transform, with Bleed Chance over 100% meaning 1 bleed wound for sure and an overflow chance of an additional bleed wound.

Though there's also second-order effects due to some abilities, so might clamp it to the interval \[0%, 100%) with exponential attenuation.

- Botany's harvest chance.

Logarithm-like transform, after you acquire additional Botany ability allowing overflow.

- Crit Chance.

Logarithm-like transform.

- Crit Damage.

Logarithm-like transform.

- Energy Recovery.

Direct attacking ability, no transform necessary.

If there's a concern that additional energy recovery is too powerful, consider this:

a) Obviously need to balance at skills levels 50 and 100 as usual, and this would prevent game regime breakage and any bad balance issues.

b) Additional sources are only unbounded scaling abilities acquirable mid-playthough under some conditions, it's not by default, player either discovers it like a secret, and should be rewarded, or spends effort to get this, and should be rewarded.

c) And when player would acquire it, it would be later in the playthrough, when the combat is mostly solved, it would be a reward for perseverance making what player already can do just slightly more convenient.

d) Make it an unbounded ability of the 2nd or 4th kind, requiring spending or keeping unspent focus points, so that it would only begin to scale after about skill level 50, when everything default in the skill is unlocked. And why won't the player start unlock it before some of the default things?

e) Cause benefits would be incomparable, e.g. additional acquirable Athletics ability of +0.1 energy regen per ability level, an ability level per 1 spent focus point, would compete not only with default Athletics abilities, but with other acquirable Athletics abilities.

f) And even then if focused only on this, disregarding other acquirable Athletics abilities, it would give +5 energy regen for the effort of reaching Athletics level 100. Is that an unbalanced reward for this?

There are multiple points here.

First, compare to Athletics' Agile Physique ability giving +5 energy per attack from a single dodge, which with high dodge and multiple opponents gives comparable or even higher amount of energy per turn. Shows that +5 energy regen is not that unbalanced.

Second, to reach Athletics level 100 the player must have explicitly gone for it, explicitly spend all that time and effort, so the reward should be compared in relation to all that time and effort.

Third, does it in general somehow affect the game's balance particularly negatively? Doesn't seem like it. It will allow to perhaps activate abilities faster, but only up to the limit of their cooldowns. And maybe there will be to some extent more synergetic ability interactions, but I don't see any game-breaking possibilities.

Fourth, even if this just quantitative, not qualitative, change is deemed as taking the gameplay too outside the tailored, developer-designed zone, outside the "as intended"-like experience, it's better to let the player have it. Getting to Athletics level 100 requires commitment and explicit desire to go there, even if it would be different from the standard gameplay to whatever extent, so let the player experience this new slightly different gameplay regime if the player aimed to and done effort to get there.

So overall, there's no need for a stat transform and we can have unbounded scaling +energy regen abilities, probably of the 1st kind, e.g. +0.1 energy regen per ability level, ability level per 1 spent focus, and that would be fine.

- Energy Recovery Efficiency.

No need for transform, same as Energy Recovery.

- First Strike Damage.

No need for transform.

- Health Recovery.

No need for transform.

- Knockback Magnitude.

No need for transform.

- Life Steal.

Tricky case, but generally speaking, it's like inverse scaling attacking abilities, like ability cost reduction, in that the closer Life Steal is to 100%, the more trivial combat becomes, and with Life Steal at 100% it becomes if not infinitely easy, than too easy.

So it's better for it to have hyperbolic attenuation, like melee ability cost reduction.

- Maximum Damage.

No need for transform.

- Melee Ability Haste.

If it has it's own hyperbolic-like attenuation transform, like attack speed, doesn't need additional transform.

If it doesn't, it should have, as it completely analogous to Attack Speed, or otherwise it should have hyperbolic attenuation, like melee ability cost reduction.

- Minimum Damage.

No need for transform.

- Movement Speed.

Like with attack speed, has it's own hyperbolic-like attenuation transform due to it's nature.

Unbounded scaling abilities of the 1st kind, +1 move speed per skill level, of the 2nd kind, +1 move speed per ability level, ability level per 1 spent focus point, or of the 4th kind, +1 move speed per unspent focus point, are completely fine.

- Multistrike.

Logarithm-like scaling, or no transform to bring out the multistrike coolness.

- Waiting Energy Recovery.

No need for transform, same as Energy Recovery.

### Inward-facing, defending

- Athletics' Dance of Shadow chance.

Exponential attenuation.

- Bleed Resist.

Exponential attenuation.

- Blight Resist.

Exponential attenuation.

- Botany's crit failure chance reduction.

Like Crit Resist, exponential attenuation if it's used as a chance on it's own, which it probably should to never have a perfect defense against crits.

If it's subtracted from the harvestable's crit chance, then no transform, but this is not ideal, if it's high enough it would lead to never ever having harvest crit failures, which is not as interesting.

- Burn Resist.

Exponential attenuation.

- Cripple Resist.

Exponential attenuation.

- Crit Resist.

Exponential attenuation, if it's used as a chance on it's own, which it probably should to never have a perfect defense against crits.

If it's subtracted from attacker's crit chance, then no transform, but the situation is not ideal, if it's high enough it could lead to 100% crit defense for all enemies which is not that good for the same reasons 100% physical resist is not good.

- Decay Resist.

Exponential attenuation.

- Dodge.

Special case, as with accuracy, has it's own transform, which for for high enough source dodge is the D>A branch of the accuracy formula, which, taking 100 (dodge - accuracy) bonus points as a unit $x$ and converting it to a dodge chance, is:
$$
f(x) = 1 - \frac{x}{((4x/3)^4 + 1)^{\frac{1}{4}}}
$$

Dodge is an inward-facing, defending percentage stat, so would be good with asymptotically exponential attenuation, $1 - f(x) \sim e^{-x}$.

The dodge formula though has asymptotics of $1 - f(x) \sim 1/x^4$, which is actually slower then exponential attenuation, so should be fine. But then, compare the dodge formula and our preferred exponential attenuation transform, chance for an attacker to land a hit is going down too fast, that's not optimal:

![[dodge_1.png]]

But then again, it's against an attacker with 0 accuracy; against a hypothetical attacker with e.g. 150 (accuracy - dodge) bonus, from their accuracy and e.g. player's dodge maluses, it looks fine (blue line), against a hypothetical attacker with 100 accuracy bonus it's somewhat fine (green line):

![[dodge_2.png]]

But then, if the issue is that the dodge chance grows too fast after 100 (dodge - accuracy) bonus, why not just fix it?

And that's actually independent of any scaling abilities stuff, we'd probably want slower growing dodge anyway, currently it's 98.87% chance to dodge at 150 (dodge - accuracy) bonus and 99.63% at 200 (dodge - accuracy) bonus, I would say these chances are somewhat too high and could be lower.

So an updated accuracy/dodge function with a new branch for (dodge - accuracy) bonus ≥ 100, smoothly matched to the current one and leaving everything else untouched:

`=if(A >= D, 0.75 + (A-D)/(100*power(power(4*(A-D)/100, 1.25) + 1, 1/1.25)), if(D-A < 100, 0.75 - (D-A)/(100*power(power((D-A)/75, 4) + 1, 0.25)), 0.0498134251268 - 0.168294102565*(D-A-100)/(100*power(power(0.168294102565*(D-A-100)/4.98134251268, 0.7) + 1, 1/0.7))))`

Could use following updated code for it:

```java
private static double getDifferenceBasedHitChance(double accuracy, double dodge) {

    var baseAccuracyBonus = 75.0;
    var baseHitChance = 0.75;
    var scalingFactor = 1.25;

    var difference = (accuracy - baseAccuracyBonus) - dodge;

    if (difference > 0) {
        return baseHitChance + (difference) / (100.0 * Math.pow(Math.pow(4.0 * (difference) / 100.0, scalingFactor) + 1.0, 1.0 / scalingFactor));
    }

	if (difference > -100.0) {
	    // Second branch for smaller negative differences
	    return baseHitChance - (-difference) / (100.0 * Math.pow(Math.pow((-difference) / 75.0, 4) + 1.0, 0.25));
	}
	
	// Otherwise, use the third formula for larger negative differences

	var branchBase = 0.0498134251268;
	var branchSlope = 0.168294102565;    
	
	return branchBase + (difference + 100.0) / (100.0 * Math.pow(Math.pow(-branchSlope * (difference + 100.0) / (branchBase * 100.0), 0.7) + 1), 1.0 / 0.7);
}
```

And with this we have better dodge attenuation, more compatible with the exponential attenuation we prefer for defensive stats (yellow line), green and red line are the dodge chance against enemies with +50 and +100 accuracy correspondingly:

![[dodge_3.png]]

Here's a zoom in to \[95%, 100%) dodge chance interval, can see how now the updated dodge chances are in line with out preferred exponential attenuation for higher dodge bonuses:

![[dodge_4.png]]

Overall, with that it's absolutely fine to have dodge unbounded scaling abilities, perhaps not abilities of the 1st find, scaling of skill levels, but certainly abilities of the 2nd kind, +1 dodge per ability level, ability level per 1 spent focus point, or of the 4th kind, +1 dodge per unspent focus point.

- Fire Resist.

Exponential attenuation.

- Frostbite Resist.

Exponential attenuation.

- Hex Resist.

Exponential attenuation.

- Ice Resist.

Exponential attenuation.

- Knockback Resist.

Exponential attenuation.

- Magic Warding.

Exponential attenuation.

- Mental Warding.

Exponential attenuation.

- Missile Deflection.

Exponential attenuation.

- Physical Resist.

Exponential attenuation.

- Physical Warding.

Exponential attenuation.

- Poison Resist.

Exponential attenuation.

- Stun Resist.

Exponential attenuation.

- Thunder Resist.

Exponential attenuation.

## Possible additional acquirable abilities

Suggestions of abilities player could acquire mid-playthrough from various sources, but scaling abilities and usual ones.

Incomplete, just examples of abilities.

For non-tree skills, marked with an asterisk \*, suggested abilities could also go into trees, if fitting, upon conversion of the skill into a tree.

Abilities are marked with following labels:

- (Non-scaling)

A suggestion of a standard non-scaling ability.

- (Skill-based)

Scaling ability of the 1st kind, which scales off the skill level, i.e. with ability having +X effect per skill level, giving +(X * L) overall effect at skill level L.

- (Linear)

Scaling ability of the 2nd kind, which scales off the linear amount of spent focus points.

Ability has an unbounded number of unlockable ability levels, each additional level costs 1 focus points, so that to get to overall ability level L you need to spend L focus points, and with ability having +X effect per the ability level you'd get +(X * L) effect for the cost of L spent focus points.

- (Quadratic)

Scaling ability of the 3rd kind, which scales off the quadratic amount of spent focus points.

Ability has an unbounded number of unlockable ability levels, Nth level costing N focus points, so that to get to overall ability level L you need to spend L(L+1)/2 focus points, and with ability having +X effect per the ability level you'd get +(X * L) effect for the cost of L(L+1)/2 spent focus points.

- (Unspent)

Scaling ability of the 4th kind, which scales off the number of unspent focus points in the skill, i.e. with ability having +X effect per unspent focus point, giving +(X * K) overall effect when you have K unspent focus points in the skill.

### Athletics

- (Linear) +0.1 energy regen per ability level

- (Linear) +1 dodge per ability level

- (Quadratic) +5 max energy per ability level

### Botany

- (Non-scaling) Show chance of critical failure.

- (Linear) -2% chance of critical failure per ability level.

- (Unspent) +2% faster regrowth of pickables per unspent focus point.

- (Non-scaling) Enable harvest chance overflow, if chance to gather >100%, second chance of (initial chance - 100%) for additional item.

- (Non-scaling) Overworld tile info.

In to any extent explored overworld tiles, in their cards on mouse right-click, show info of botany resources you've seen while exploring the tile, with three levels of ability: 1) show what kind of resources tile has (various plants, mushrooms), 2) also show how many counts of places of each resource in the tile, 3) an estimate with 90% confidence interval how many is available for harvest depending on how long ago visited the tile.

- (Non-scaling) Inner tile info.

While exploring tiles/dungeons, in the portions of the map you've already explored and seen before, show in the fog of war half-transparent greyed-out icons of botany resources in locations you've ever seen them before.

### Dreadheart

- (Non-scaling) +1% melee and ranged cost reduction per 1% of missing health

- (Non-scaling) +1 move speed, +1 attack speed per 1% of missing health

- (Linear) +0.01% chance of Dogged Resolve activation per ability level per 1% of missing health.

- (Quadratic) +0.03% lifesteal per ability level per 1% of missing health.

- (Quadratic) +3 decapitation per ability level.

- (Unspent) +1% crit chance per unspent fp.

- (Unspent) +1% multistrike chance per unspent fp.

- (Unspent) +1% bleed chance per unspent fp.

### Enchanting

- (Skill-based) -1% magnitude to all detrimental enchantment effects per Enchanting level (with exponential attenuation adjustment at higher total).

- (Linear) +1% magnitude to all beneficial enchantment effects per ability level.

- (Unspent) +5% chance per unspent fp to save a crystal, cumulative with Crystal Conservation, minimum cost is still 1 crystal.

- (Non-scaling) Can enchant single item with two enchantments.

Only at enchantment table, crystal cost is (cost1 + cost2 + 1), material costs just add, potency requirement is ceil(max(potency1, 2) * max(potency2, 2)) — e.g. medium accuracy (cost 2, requirement 3) with medium dodging (cost 2, requirement 8) would cost 5 crystals with requirement of 24 Enchanting.

Can add a chance of failure of (2 * potency required - Enchanting level), so e.g. if the potency of enchantment would require 24 Enchanting level, unless Enchanting level is greater than 48, it would have a chance of failure of (48 - Enchanting level)%.

- (Quadratic) -1 potency level requirement per ability level.

- (Non-scaling) Additional potency tier, Apex — 5 crystal enchantment base cost.

### Quartermastery

- (Non-scaling) Unlock 3rd satchel slot.

- (Non-scaling) Gain ability to craft trail food satchel (-25% weight for baked potatoes, boiled eggs, bread, flowery bread, galette, meat pie, roasted haunch)

- (Non-scaling) Enhance items.

Given unenchanted item 1 and item 2 of the same type, e.g. boots, you take them apart and re-assemble together into an item of the same type with the best effects of initial items, i.e. for each common stat bonus of initial items you get the max(bonus1, bonus2), while exclusive bonuses go unchanged.

Repair and bolstering costs are the sum of repair and bolstering costs of initial items, so it's diminishing return.

Could have a Quartermastery level requirements, like Enchanting requirements, and a chance of failure, like chance of failure for Enchanting two items (see suggestion above in [[#Enchanting]]), based on total items' cost and/or total number and cost of materials you need for bolstering the items.

- (Linear) +1% chance per ability level to get 1 material more (of each type separately, 1 wood / 1 scrap metal / …) when salvaging an item.

- (Unspent) +5% chance per unspent fp to save 1 material (of each type separately, 1 wood / 1 scrap metal / …, with diminishing returns at higher totals) when repairing or bolstering an item, costs are ever minimum 1 material each type.

### Reading*

- (Non-scaling) Slightly nerfed (no +% reward) Neverending Journey ability from a previous suggestion, allows book re-reading to get reward delta if rewards increased since the book was read.

- (Non-scaling) Scattered Interests ability from a previous suggestion, +floor(sqrt(N))% bonus reading rewards with N being number of books read.

- (Linear) +1% reading rewards from books (including skill xp and knowledge) per ability level.

### Survival

- (Skill-based) -1% escape prevention range per Survival level (with diminishing returns at higher totals)

- (Non-scaling) Explicitly show escape prevention range on ability toggle.

- (Quadratic) +1 vision distance per ability level.

- (Quadratic) +0.5 trap vision distance per ability level.

- (Linear) +0.25% energy gain from all sources per ability level.

- (Unspent) +1% trap reaction per unspent fp.

- (Unspent) +1% more loot from outdoor harvestable sources per unspent fp.

- (Non-scaling) Overworld tile info.

In to any extent explored overworld tiles, in their cards on mouse right-click, show info of survival resources you've seen while exploring the tile, with three levels of ability: 1) show what kind of resources tile has (wood, berries, strawberries), 2) also show how many counts of places of each resource in the tile, 3) an estimate with 90% confidence interval how many is available for harvest depending on how long ago visited the tile.

- (Non-scaling) Inner tile info.

While exploring tiles/dungeons, in the portions of the map you've already explored and seen before, show in the fog of war half-transparent greyed-out icons of survival resources in locations you've ever seen them before.

### Swords*

- (Linear) +1% melee cost reduction with swords per ability level.

- (Linear) +1 accuracy with swords per ability level.

- (Linear) +1 attack speed with swords per ability level.

- (Quadratic) +1 min & max damage with swords against full health per ability level.

- (Quadratic) +2 dodge with swords per ability level.

### Travel*

- (Non-scaling) Overworld tile info.

In overworld tile cards on mouse right click, show % of exploration as number of ever viewed area / total area. For dungeons, show aggregated total over all visited floors, and separately a number of visited floors.

### Warrapt

- (Unspent) 1% swap time reduction per unspent fp.

- (Unspent) 1% less time to enter a stance per unspent fp.

- (Unspent) 1% less time to perform all melee and ranged abilities per unspent fp.

- (Unspent) +1% crit prevent chance per unspent fp.

- (Linear) +1% physical resist per ability level.

- (Linear) +1% multistrike per ability level.

- (Linear) +1% repeat attack chance per ability level.

- (Linear) +1% crit chance per ability level.

- (Quadratic) +1 protection per ability level when using a shield and/or armor, up to the limit of (base protection from shield + base protection from armor / 2).

# Possible implementation of discovery mechanic

For alchemy/cooking/medicine recipes and for additional skills acquirable mid-playthrough, or actually any other thing which could be acquired mid-playthrough and depends on skill requirements.

For each discoverable thing with an associated skill we would have a cut-off level of the skill after which discovery becomes possible, and optionally additional requirements. And after the player reaches cut-off skill level, each time another skill level is acquired there would be a chance to discover the thing if optional additional requirements are also satisfied, with the chance getting higher the higher acquired skill level is.

For a recipe required skill level would be a minimal skill level which is required to unlock all abilities recipe requires.

E.g. for Fried Wedges recipe from Cooking required Cooking skill level would be 3 (1 for Peeling, 2 for Pan Frying), and discovering Fried Wedges recipe would be possible starting at reaching Cooking level 3, in case of course when optional additional requirements are satisfied if there are any.

For an ability required skill level would also be the minimal skill level required to unlock the ability, so either the skill level the ability itself requires, or a minimal skill level required to unlock all its prerequisites, whatever is greater.

Obviously nothing prevents from setting required skill levels explicitly to some more suitable value for things for which it would be better.

Additional optional requirements for recipes could be:

1. Actually no additional requirements.
2. Having recipe consumable paper item in the inventory, but not actually knowing the recipe.
3. Having seen each ingredient either in the inventory inventory, loot or a shop at any point in time, separately.
4. Having each ingredient in the inventory at any point in time, separately.
5. Having all of the ingredients in the inventory.
6. Having all required passive abilities unlocked.

It feels that combination of the 2nd one, 3rd one and the 5th one is the most appropriate, so that e.g. to make discovery of Fried Wedges possible you'd need to (had seen both Oil and Raw Potato OR have Fried Wedges Recipe item in the inventory) AND to have Peeling and Pan Frying unlocked in Cooking.

Additional optional requirements for abilities could be any combination of following (or actually of any conceivable conditions that fit):

1. Actually no additional requirements.
2. A separate skill level prerequisites, for the skill of the ability and/or any other skills.
3. Any combination of abilities player already needs to now.
4. A character level prerequisite.
5. Having an item in the inventory at any point in time.
6. Having studied a book.
7. Already having an unlocked mid-playthrough acquirable ability in the skill tree.

7th one feels the most interesting, with it you would first need to sort of breakthrough into this secret / higher skill region with some other source, like book or quest, which would give you your first additional ability for that skill; and then you could discover other additional abilities of the skill on your own during normal skill levelling.

Naturally with the 7th condition don't have to have just one starting ability per skill, could have more than one that are acquirable from external sources like quests or books and can start discovery of other acquirable/discoverable abilities of that skill.

Could of course use combinations of the 7th and others.

Can suggest two ways to determine the chance to discover a thing with its assigned cut-off skill level N when getting another level (N + k) of the skill:

1. k/N.
    
    Less variability, guaranteed discovery by skill level 2N.
    
2. k/(N + k).
    
    More variability, no guaranteed discovery, though still effectively guaranteed by e.g. skill level 2N + 10:
    
    At skill level 2N we have discovery chance of at least N/(N+N) = ½, so non-discovery chance of at most ½, so with 10 additional tries overall chance of non-discovery would be 1/2^10 < 1/1000.

If to choose between this two ways of setting discovery chance, I would advocate for the 2nd.

The 2nd way fits uncertain nature of discovery more, due to more variability it would feel less samey along different playthroughs, and if we would like to give players guarantees of discovery, it's better for them to emerge organically from underlying mechanics of game's reality rather than be imposed by the devs' fiat from above.

On average, for the 1st way expected skill level of discovery is no more than 1.2N + 2, with discovery being made with 95% probability before the 1.3N + 4 skill level.

For the 2nd way expected skill level of discovery is no more than 1.2N + 2.5, with discovery being made with 95% probability before 1.3N + 6 skill level.

See next subsection for graphical visualization and more detailed info.

### Mathematical details

Could skip more involved math and go straight to graphs.

For the 1st way, if chance of discovery at skill level $N+k$ is $k/N$, then a chance of non-discovery is $(N-k)/N$, and overall chance of non-discovery by skill level $N+k$ would be:
$$
\begin{align*}
C_1^*(N, k)
&=
\frac{N-1}{N} \cdot \frac{N-2}{N} \cdot \dots \cdot \frac{N-k}{N}
\\
&=
\frac{(N-1)!}{(N-k-1)! N^k}
\end{align*}
$$

Goes to exactly 0 by k = N.

Keeping things simpler, not using falling / rising factorial / Pochhammer symbol notation.

So then chance of having made the discovery by the skill level $N+k$ would be:
$$
C_1(N, k)
=
1 - \frac{(N-1)!}{(N-k-1)! N^k}
$$

Chance of having made the discovery by the skill level $N+k$ is just the sum of chances to make discovery at each individual level $N+1, N+2, \dots, N+k$, so that would give chance, or better say, probability density of discovery at skill level $N+k$ of
$$
\begin{align*}
P_1(N, k)
&=
C_1(N, k) - C_1(N, k-1)
\\
&=
\left[ 1 - \frac{(N-1)!}{(N-k-1)! N^k} \right] - \left[ 1 - \frac{(N-1)!}{(N-k)! N^{k-1}} \right]
\\
&=
\frac{(N-1)!}{(N-k-1)! N^{k-1}}
\left[ \frac{1}{N-k} - \frac{1}{N}\right]
\\
&=
\frac{(N-1)!}{(N-k-1)! N^{k-1}}
\left[ \frac{1}{N-k} - \frac{1}{N}\right]
\\
&=
\frac{(N-1)!}{(N-k-1)! N^{k-1}}
\cdot
\frac{k}{(N-k) N}
\\
&=
\frac{(N-1)!}{(N-k)! N^{k-1}}
\cdot
\frac{k}{N}
\end{align*}
$$

Intuitively obvious, actually, to discover at exactly skill level $N+k$ is to not get it up to skill level $N+k-1$ and then get it at level $N+k$, so the probability would be a product of probability of non-discovery up to level $N+k-1$
$$
C_1^*(N, k-1) = \frac{(N-1)!}{(N-k)! N^{k-1}}
$$
and specific probability of discovery at level $N+k$ which is $k/N$, exactly what we have here.

Consequently, the probability density is exactly 0 for k > N.

Then we can get average skill level at which discovery would be made as
$$
\begin{align*}
E_1(N)
&=
\sum_{k=0}^N
(N+k) P_1(N,k)
\\
&=
\sum_{k=0}^N
(N+k)
\cdot
\frac{(N-1)!}{(N-k)! N^{k-1}}
\cdot
\frac{k}{N}
\end{align*}
$$

Don't see a closed-form solution, but that's not a problem, can just compute it.

Also can numerically find a 95% probability cutoff, minimal skill level $N+k$ such that it is expected to make discovery by this level with 95% probability.

Here's cumulative probability and probability density for N = 10, 20, 30, with vertical lines at corresponding expected discovery level at 13.66, 25.29 and 36.55 and dotted vertical lines at 95% discovery probability skill levels 16.18, 29.41 and 41.88:

![[discovery_1a.png]]

Here's difference from initial cut-off skill level N to average discovery skill level (point marker), and from initial cut-off skill level to skill level of 95% discovery probability (square marker) for N of 5 to 35, with dotted red lines showing upper bounds of 0.2N + 2 and 0.3N + 4:

![[discovery_1b.png]]

For the 2nd way, with chance of discovery at skill level $N+k$ being $k/(N+k)$ and chance of non-discovery being $N/(N+k)$, overall chance of non-discovery by skill level $N+k$ is:
$$
\begin{align*}
C_2^*(N, k)
&=
\frac{N}{N + 1} \cdot \frac{N}{N + 2} \cdot \dots \cdot \frac{N}{N + k}
\\
&=
\frac{N^k N!}{(N+k)!}
\end{align*}
$$

Notably, never goes to exactly 0 like the chance of non-discovery with the 1st way, just gets smaller and smaller rather quickly.

Chance of having discovery by skill level $N+k$:
$$
C_2(N, k)
=
1 - \frac{N^k N!}{(N+k)!}
$$

Probability density of discovery at skill level $N+k$:
$$
\begin{align*}
P_2(N, k)
&=
C_2(N, k) - C_2(N, k-1)
\\
&=
\left[ 1 - \frac{N^k N!}{(N+k)!} \right] - \left[ 1 - \frac{N^{k-1} N!}{(N+k-1)!} \right]
\\
&=
\frac{N^{k-1} N!}{(N+k-1)!} \left[ 1 - \frac{N}{N+k}\right]
\\
&=
\frac{N^{k-1} N!}{(N+k-1)!} \cdot \frac{k}{N+k}
\end{align*}
$$

Again just as with 1st way, intuitively obvious as the product of probability to not have discovered by skill level $N+k-1$ and probability of specifically discovered at skill level $N+k$.

And just as chance of non-discovery, never goes to exactly 0 like the probability density with the 1st way, just gets smaller and smaller even more quickly.

Average skill level of discovery:
$$
\begin{align*}
E_2(N)
&=
\sum_{k=0}^\infty
(N+k) P_2(N,k)
\\
&=
\sum_{k=0}^\infty
(N+k)
\cdot
\frac{N^{k-1} N!}{(N+k-1)!}
\cdot
\frac{k}{N+k}
\end{align*}
$$

Again can compute it, no upper summation bound is not a problem as it decreases sufficiently fast with increasing $k$, can just take the sum of sufficiently many items.

And just as with the 1st way can numerically find a skill level at which we reach the 95% cumulative discovery probability.

Cumulative probability and probability density for N = 10, 20, 30, with vertical lines at corresponding average discovery level at 14.33, 25.96 and 37.22 and dotted vertical lines at 95% discovery probability skill levels 18.20, 31.42 and 43.88:

![[discovery_2a.png]]

Difference from initial cut-off skill level N to average discovery skill level (point marker), and from initial cut-off skill level to skill level of 95% discovery probability (square marker) for N of 5 to 35, with dotted red lines showing upper bounds of 0.2N + 2.5 and 0.3N + 6:

![[discovery_2b.png]]

Compared to the 1st way, 2nd way has slower rising cumulative chance of discovery, more spread out probability density of discovery, about 0.7 levels higher average skill level of discovery and about 2 levels higher higher 95% discovery probability skill level:

![[discovery_3a.png]]

![[discovery_3b.png]]