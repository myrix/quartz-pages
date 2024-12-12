
# Useful Insights

What you do is reinforced in your behaviour.

Are you chasing dopamine high?

Get the process going, one thing to do after another.

## Additional Insights

Go away to another place, like kitchen, to remove extraneous attractions and to switch mental track.

Disable all distractions and all contact, Telegram / Discord / Whatsapp etc., if need to do tasks.

If have pressure due to expectations of doing better, especially if in something you're not that good, temporarily switch, or almost switch, to another track of work, like ISP work.

Fail again. All fail until they don't.

# In Progress

*What you do is reinforced in your behaviour.*
*Are you chasing dopamine high?*
*Get the process going, one thing to do after another.*

Always need at least one current meaningfully useful terminal task:

```tasks
(tag includes #DoorsOfTrithius) OR ((tag includes #ISP) AND (tag does not include Support))
status.type is in_progress
```

General tasks:

```tasks
tag does not include #DoorsOfTrithius 
(tag does not include #ISP) OR (tag includes Support)
status.type is in_progress
```

# Today & General

Today & General:

%% Set created date serves as a soft of general signifier, as opposed to today. %%

```tasks
tag does not include #DoorsOfTrithius 
(tag does not include #ISP) OR (tag includes Support)
not done
NOT (scheduled after today)
no created date
```

```tasks
tag does not include #DoorsOfTrithius 
(tag does not include #ISP) OR (tag includes Support)
not done
(scheduled after today) OR (has created date)
```

Done today:

```tasks
tag does not include #DoorsOfTrithius 
(tag does not include #ISP) OR (tag includes Support)
done today
```

Done yesterday:

```tasks
tag does not include #DoorsOfTrithius 
(tag does not include #ISP) OR (tag includes Support)
done yesterday
```

[[Task Archive#Today & General]]

# Doors of Trithius

Doors of Trithius:

```tasks
tag includes #DoorsOfTrithius
not done
```

Done today:

```tasks
tag includes #DoorsOfTrithius
done today
```

Done yesterday:

```tasks
tag includes #DoorsOfTrithius
done yesterday
```

[[Task Archive#Doors of Trithius]]

# ISP

ISP:

```tasks
tag includes #ISP
tag does not include Support
not done
```

Done today:

```tasks
tag includes #ISP
tag does not include Support
done today
```

Done yesterday:

```tasks
tag includes #ISP
tag does not include Support
done yesterday
```

[[Task Archive#ISP]]