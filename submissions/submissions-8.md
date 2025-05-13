# players (shuffled)

- rebecca
- jetison
- The Right Honorable, The Lord Umnikos
- essaie
- [*as willed.*](<https://github.com/Jetison333/rotg/blob/442ae0a96fc6d22aaeb941bdf76ded6a3e74fad1/current-round-rules.md#the-ghost-of-guessing-past>)

The Right Honorable, The Lord Umnikos drew The Hermit, players who guess him will gain 2 points rather than 1.

## 1

each person can only draw 3 cards per round

## 2

president (v):
- (*intransitive*) To appear; to be present, as in an arrangement.
  - *When I saw him **president** in the lineup, I knew he'd killed my brother.*
- (*transitive*, *dated*) To make exposed.
  - *Dude, she tried to **president** me last night on the tram, and I knew I had to get out of there.*

election (n):
- A casual meetup, get-together, or gathering.
- An ordered collection of names, keywords, titles, or other personal identifiers, usually each associated with a number.
- (*Chiefly UK*, *slang*) Ten trolls' strength 💪, ten trolls' length 😳. One troll can pick it up 😏, but no troll can stand it up 😔.
  - *I tried to save her, having thrown down my **election** and everything. It haunts me to this day.*
- (*computing*, *slang*) A priority queue implemented inelegantly.
  - *trolol d1d u c his **election**/?  roflm4o*

## 3

Itums require pompous names paired with deadpan effect descriptions.

## 4

after the first sentence of the rule titled endorsements insert another sentence or sequence of sentences with the effect of allowing players to pick who they endorse either by naming a player or indicating a submission in which case the author of that submission gets endorsed

also add a new rule that says that round numbers have to be given using roman numerals in all official communication channels

## 5

```diff
From 04a10ec75fae5d5db3453c14dafd4dd8d3447064 Mon Sep 17 00:00:00 2001
From: umnikos <alex.stefanov2@gmail.com>
Date: Sat, 10 May 2025 04:32:34 +0300
Subject: [PATCH] fix stuff

---
 current-round-rules.md | 43 ++++++++++++++++++++++--------------------
 1 file changed, 23 insertions(+), 20 deletions(-)

diff --git a/current-round-rules.md b/current-round-rules.md
index 734b176..8d9b8fe 100644
--- a/current-round-rules.md
+++ b/current-round-rules.md
@@ -1,15 +1,20 @@
 ## Rules:
 
-Each round is played in multiple stages. Stage 2 takes place after stage 1 ends, and the scoring stage takes place after stage 2 ends.
+Each round is played in multiple stages. Each stage takes place in numerical order and after the previous one has ended.
 
-The Game Administrator has the final word on all issues regarding the interpretation of the rules text and on issues for which the rules text does not specify a resolution.
+The Game Adminstrator has the final word on all issues regarding the interpretation of the rules text and on issues for which the rules text does not specify a resolution.
 
 ++/∘++/ = ++/∘++/∗
 
+## Definitions
+In the rest of the document the following terms have the corresponding definitions:
+- Person: An entity capable of playing the game
+- Player: A person who has submitted in the current round
+- Gamer: A person that is or has been a player, or is serving or has served a game-related role (e.g. Game Adminstrator)
+
 ## Stage 1
 During the duration of stage 1, any person on the server can make a "submission" by sending it to the Game Adminstrator through a direct message. 
-From this point on, they are considered a "player" of the round. A player can only have 1 submission.
-“A "person" is anyone the Game Adminstrator acknowledges as having ever taken action within the game.”
+From this point on, they are considered a player of the round. A player can only have 1 submission.
 
 The submission must consist of a description of an alteration they wish to make to the rules text, described in any sufficiently easy to understand format.
 
@@ -23,12 +28,12 @@ The previous winner of a themed round agrees with the Game Admin on what this wi
 
 ## Stage 2
 At the beginning of stage 2, the submissions given during stage 1 are shuffled, assigned numbers and made public.
-The players are now tasked with determining which submission was uploaded by which player.
+The players are now tasked with determining which submission was submitted by which player.
 These "guesses" are represented as partial bijections, meaning that each submission is paired with at most 1 unique player and each player is paired with at most 1 unique submission.
 
 The first time you guess, you learn how many of your neighboring entries have been guessed by you correctly
 
-## Scoring stage
+## Stage 3 (scoring stage)
 After stage 2, each player receives 1 point for each player they guessed, and loses 1 point for each player that guessed them.
 The players with the most points are the winners of the round.
 
@@ -38,13 +43,13 @@ in case of a tie in points, whichever entry has a sha256 hash closer to the sha2
 
 The rules alternations submitted by each of the winning players are all enacted by the Game Adminstrator, and go into effect at the start of the next round.
 
-After the scoring stage ends the round is over, and a new one may begin.
+After stage 3 ends the round is over, and a new one may begin.
 
 ## Marbles
-Each player will now have a number of marbles that carry on into future rounds. This amount is public information. Players will start with zero marbles, and will earn one marble for each correct guess they make during the guessing phase. If a player tries to do an action that would result in some player having fewer than zero marbles, that action fails, with that player being told "you have lost your marbles". Further, each player gets their number of marbles divided by 10 and then rounded down added to their score during the scoring phase. The following actions can be made using marbles:
-1. Rolling a marble - gives one of your marbles to a specified player
-2. Shooting a marble - uses one of your marbles to remove one marble from a specified player
-4. 100 marbles - win the game
+Each person will now have a number of marbles that carry on into future rounds. This amount is public information. People will start with zero marbles, and will earn one marble for each correct guess they make during the guessing phase. If a person tries to do an action that would result in some player having fewer than zero marbles, that action fails, with that person being told "you have lost your marbles". Further, each person gets their number of marbles divided by 10 and then rounded down added to their score during the scoring phase. The following actions can be made using marbles:
+1. Rolling a marble - gives one of your marbles to a specified person
+2. Shooting a marble - uses one of your marbles to remove one marble from a specified person
+4. 100 marbles - if you have at least 100 marbles, win the game
 
 ## The Swindler's Wagon
 
@@ -56,7 +61,7 @@ The Swindler may optionally:
 - discard a chosen itum from the wagon
 - provide a description &c of an itum to stock into the wagon
 
-Then they sellout, choosing another player or the Game Adminstrator to become the Swindler.  Each player may be Swindler only once per round.
+Then they sellout, choosing another gamer or the Game Adminstrator to become the Swindler.  Each person may be Swindler only once per round.
 
 The Game Adminstrator names prices for all wagon itums, and may change them at will.  A price must include some amount marbles or other money, and may include other things too.
 
@@ -64,7 +69,7 @@ If who's the Swindler is unclear, or the they have not taken an action for half
 
 ### Till
 
-When a player moves to buy an itum, the itum is taken from the Wagon and bidding is started.  Players from the past two rounds may bid privately.  All bids must have at least the counts in the asking price or higher, and may not include things not in the price.  Bids are rejected if they cannot be proven payable.
+When a person moves to buy an itum, the itum is taken from the Wagon and bidding is started.  Players from the past two rounds may bid privately.  All bids must have at least the counts in the asking price or higher, and may not include things not in the price.  Bids are rejected if they cannot be proven payable.
 
 When bidding ends, the person with the highest bid gets the itum, and they pay the second highest bid.  Neither the Game Adminstrator nor Swindler receive the payment.
 
@@ -108,16 +113,16 @@ A Tit(le) grants the holder the Game Adminstrator's abilities from a selection o
 
 ## sorry
 
-any player may ohno at the cost of sorry
+any gamer may ohno at the cost of sorry
 
 
 ## Messing with time
 The durations of stages, happenings of undefined length, and the time gaps between rounds are entirely determined by the Game Adminstrator. The Game Adminstrator may issue time extensions without the need to specify a reason for the extension.
 
 # Contract law  
-Players may enter into contracts with other players. In order for a contract to be valid, it must contain obligations and signatures and be submitted to the Game Adminstrator who will enforce the contract's terms. A contract may also contain penalties.   
+People may enter into contracts with other people. In order for a contract to be valid, it must contain obligations and signatures and be submitted to the Game Adminstrator who will enforce the contract's terms. A contract may also contain penalties.   
 ## Obligations  
-Any person who has an obligation is considered a party to a contract. An obligation constraints the future actions of each party to the contract. It may enforce positive action, such as but not limited to submitting a particular rule change submission, or telling a person some information. It may also enforce negative action, such as but not limited to not guessing a submission, or keeping information confidential. Conditions may be specified where an obligation only exists if those conditions are met. Obligations can only be actions that are related to the game, and cannot be things external to the game. If possible the Game Adminstrator should proceed as if obligations are followed, for example if a contract stipulates that a player must make a particular submission, then the game should proceed as if that player made that submission, even if the player attempted to submit something else.   
+Any person who has an obligation is considered a party to a contract. An obligation constraints the future actions of each party to the contract. It may enforce positive action, such as but not limited to submitting a particular rule change submission, or telling a person some information. It may also enforce negative action, such as but not limited to not guessing a submission, or keeping information confidential. Conditions may be specified where an obligation only exists if those conditions are met. Obligations can only be actions that are related to the game, and cannot be things external to the game. If possible the Game Adminstrator should proceed as if obligations are followed, for example if a contract stipulates that a person must make a particular submission, then the game should proceed as if that person made that submission, even if they attempted to submit something else.   
 ## Signature  
 A valid contract must have a signature for every party in a contract. A signature is any proof that a party has accepted the contract that the Game Adminstrator is willing to accept.   
 ## Penalties  
@@ -129,7 +134,7 @@ Players may meow, bark, or produce other such cute animal sounds.  These actions
 Statistics about meowing performed by players, including but not limited to frequency and number of occurrences, are tracked by the Game Adminstrator.  The Game Adminstrator MUST track this information in a privacy-friendly manner, i.e. a manner which does not allow individuals to be identified from their informwation being tracked.  
   
 # Endorsements  
-At the end of each round, after guesses are finalized and scores are calculated, but before identities or guesses or scores are announced or any new rules are enacted, each Player is given (in private) the choice to either Endorse any individual Player, or not. Here a Player is anyone who submitted in the round in question.   
+At the end of each round, after guesses are finalized and scores are calculated, but before identities or guesses or scores are announced or any new rules are enacted, each Player is given (in private) the choice to either Endorse any individual Player, or not.
   
 Next, for every Player P, compute P's Endorsement Score as 1 + (the sum of the Endorsement Scores of every Player that Endorsed P). To keep this well defined, disregard every Player that is part of a cycle in the directed graph of Endorsements: those players' Endorsement Scores are effectively zero.  
   
@@ -142,7 +147,7 @@ The information about who Endorsed whom is revealed by the Game Adminstrator alo
 # Tab 4  
 Each stage, you may visit the Game Adminstrator to learn 2 things in private: 1 is true & 1 is false.
 
-This is a silly game. Participants of all roles must not stress too much about unforeseen consequences of their actions, for those are what make the game fun.
+This is a silly game. Gamers must not stress too much about unforeseen consequences of their actions, for those are what make the game fun.
 
 every new rule applies retroactively, assuming everyone in past rounds would have acted in the same way with the rule as they did without.
 
@@ -165,8 +170,6 @@ At any time one may draw a uniformly random card from the Deck. When a card is d
 
 Effects are not optional. If an effect cannot be resolved, it is not.
 
-Any person may choose that they are only able to draw at most one card per round.
-
 # Appendagealism  
   
 The Appendage is a section of the rules.  
-- 
2.49.0
```

