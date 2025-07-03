
# players (shuffled)

- jetison
- rebecca
- makefile
- umnikos


# 1

remove the clause that causes contracts to be uneditable.

# 2

during stage 2, players may challenge the Game Adminstrator to a game of tak. if they win their marble gain during stage 3 is doubled, if they draw or lose their marble gain during stage 3 is 0

# 3

```diff
- Itums have the ability to make changes to game state but not change the rules text. They may also grant specific exemptions from the rules.
+ Itums have the ability to make changes to game state but not change the rules text. If an itum's description conflicts with the rules, the rules take precedence. In particular, if an itum grants an exemption from the rules and the rules don't account for that, then that itum does nothing.
---
  The Swindler may optionally:
  - discard a chosen itum from the wagon
  - provide a description and so on of an itum to stock into 
the wagon
+ - recall or change the submission that was submitted by the previous Swindler to the next round if there is one
+ - submit a rule to the next round. This rule is only allowed to activate when the Itum's description would, and may specify any departures from the text of the rules the Itum is allowed to make. The Swindler then plays as a player in the round, under the title "*as swindled*". The Swindler is considered a distinct player in the round, and whoever is the current Swindler may play as their real identity at the same time; when doing so, they must clarify to the GA the identity they are using for any game action.
```

# 4

## the Herstorian
 
The Herstorian is a government office. The Herstorian is responsible for documenting interesting things that happen during their term, and compiling this account into a document called the Herstory, which is publicly available. The Herstorian may also, at their discretion, compile introductory resources, summaries of the rules, etc, for the benefit of new or returning players.



