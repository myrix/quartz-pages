- [x] #DoorsOfTrithius #Guide Accuracy-Dodge guide part writeup for Sineso ✅ 2024-10-21

# Discord messages

> Sineso — Today at 11:00 AM
> 
> Would you like to try write a short 1-3 paragraphs describing how this works for the guide?
> I imagine the guide will have advanced section on many of the topics.
> You can click to expand the advanced section. For nerds to see the real stuff.
> And we explain some of the math and the reasoning as clearly and succinctly as we can.
> It doesnt need to be exact explanation, but the general idea
> 
> myrix — Today at 11:05 AM
> 
> the general idea is actually could be said in one-two sentences:
> "Hit chance depends on attacker's accuracy and defender's dodge, hit chance is always between 0% and 100%, is 75% for base accuracy of 75 and 0 dodge, the higher accuracy than the dodge is, the higher the chance is, the lower accuracy than the dodge is, the lower the chance. More bonuses give diminishing returns."
> 
> if with reduction to the mean, can add something like this:
> "The higher both attacker's accuracy and defender's dodge, the less difference matters."
> 
> If to go deeper then this, math would start to appear, like exact functions and requirements including derivative of 1 at the origin.
> 
> Sineso — Today at 11:05 AM
> 
> One step deeper
> "As hit chances approaches 0% or 100%, an increasing amount of accuracy or dodge is needed. "
> "To reach 95% hit chance against a 0 dodge opponent, 100 bonus accuracy is needed. To reach 95% dodge against an opponent with no accuracy bonus, 100 dodge is needed"
> Something like this... explaining the curve or reasoning behind it
> so its not a black box

# Text

Hit chance is determined by attacker's accuracy and defender's dodge, and is always between 0% and 100%. When you are the defender, you can see your dodge chance which is just 100% minus the attacker's hit chance.

For base accuracy of 75 and base dodge of 0 the hit chance is 75%. Attacker's bonus accuracy increases hit chance, defender's bonus dodge decreases it.

For small bonuses the effect is one-to-one or almost one-to-one, 1% per 1 bonus point, but as the bonuses get larger, they start to give diminishing returns, e.g. +5 accuracy bonus against dodge 0 would give 79.6% hit chance, while with +100 accuracy against 0 dodge you'll have 97.0%. For dodge point of diminishing returns is further, +5 dodge bonus against base accuracy 75 would give 70.0% hit chance (30.0% dodge chance), while +100 dodge against the same would have you 5.0% hit chance (95.0% dodge chance).

With large enough and 'equalish' enough accuracy and dodge bonuses you get clash of competencies effect, which drags the hit change close to the middle of 50%. It might slightly hinder or help depending on whether you are the attacker or the defender and what bonus accuracy and dodge values are.

The bonuses need to both close enough in relative magnitude and large enough to make it noticeable; if any bonus is 0, the effect is non-existent. E.g. it attacker has bonus +10 accuracy and defender has bonus +10 dodge you'd have hit chance of 74.0% instead of 75%, while for +100 accuracy and +100 dodge the hit chance would be 65.5% instead of 75%. As with hit chance, when bonuses are already large increasing them even more does not increase the effect as much.

# Good enough

> Sineso — Today at 11:29 AM
> Yeah this is good
> I will reword a bit, but the concepts and structure is solid