# Rules:

## Defintions

Throughout the document the following terms have the corresponding definitions:
- Gamer: An entity that has participated, is participating, or is willing to participate in the game.
- Player: A gamer who has submitted in the current round.
- Action: The act of doing something related to the game state. Discussion is not an action unless otherwise specified by a rule.

"Somebody", "nobody" and "everybody" are shorthand for "some gamer", "no gamer" and "every gamer" respectively.


## Game Adminstrator

The Game Adminstrator is the gamer running the game and interpreting the rules text. The Game Adminstrator has the final word on all issues regarding the interpretation of the rules text and on issues for which the rules text does not specify a resolution.

The Game Adminstrator may, at any point, appoint another gamer to become the new Game Adminstrator, as long as that gamer is willing. After doing so they stop being the Game Adminstrator and the appointed gamer becomes the Game Adminstrator.

The Game Adminstrator may NOT become a player, nor appoint a player as the new Game Adminstrator.


## Silly

This is a silly game. Gamers must not stress too much about unforeseen consequences of their actions, for those are what make the game fun.

the rules shall always be displayed rotated by however many points this submission gets (1), expressed as radians.

## Rounds

The game is played as a sequence of rounds. There can be at most one round going on at any given time.
Each round consists of multiple stages. Each stage takes place in numerical order and after the previous one has ended. 

Unless otherwise specified in the rules, game state other than the rulebook's text resets between rounds.

The durations of stages, happenings of undefined length, and the time gaps between rounds are entirely determined by the Game Adminstrator.
The Game Adminstrator may issue time extensions without the need to specify a reason for the extension.


## Stages

### Stage 1 (Submissions stage)

During the duration of stage 1, any gamer can make a "submission" by sending it to the Game Adminstrator through a direct message. From this point on, they are considered a player of the round. A player can only have 1 submission.

The submission must consist of a description of an alteration they wish to make to the rules text, described in any sufficiently easy to understand format.

The Game Adminstrator must NOT give any suggestions to the players in private (though they're free to do so in public).
The Game Adminstrator is allowed to say how they're planning to interpret the players' submission drafts, both in public and in private.

#### Rounds of Restriction

Every third round is a themed round, which has some contrived restriction or theme upon submissions.

The previous winner of a themed round agrees with the Game Adminstrator on what this will be.

### Stage 2 (Guessing stage)

At the beginning of stage 2, the submissions given during stage 1 are shuffled, assigned numbers and made public. The players are now tasked with determining which submission was submitted by which player.

These "guesses" are represented as partial bijections, meaning that each submission is paired with at most 1 unique player and each player is paired with at most 1 unique submission.

The first time you guess, you learn how many entries you correctly guessed. (You may then change your guess by guessing again.)

During stage 2 of any round, any player may spend 10 marbles (which disappear) and in return get 1 added to their score during the scoring stage of that round only.

During stage 2, players may challenge the Game Adminstrator to a game of tak.  If they win their marble gain during stage 3 is doubled, if they draw or lose their marble gain during stage 3 is 0.

### Stage 3 (Scoring stage)

After stage 2, each player receives 1 point for each player they guessed, and loses 1 point for each player that guessed them.
The players with the most points are the winners of the round.

The rules alternations submitted by each of the winning players are all enacted by the Game Adminstrator, and go into effect after the end of the round.

While enacting the submissions, the Game Adminstrator is free to edit the rulebook's formatting and paragraph order.

After stage 3 ends the round is over, and a new one may begin.

### Endorsements

At the end of each round, after guesses are finalized and scores are calculated, but before identities or guesses or scores are announced or any new rules are enacted, each player is given (in private) the choice to either Endorse any individual player, or not.

Next, for every player P, compute P's Endorsement Score as 1 + (the sum of the Endorsement Scores of every player that Endorsed P). To keep this well defined, disregard every player that is part of a cycle in the directed graph of Endorsements: those players' Endorsement Scores are effectively zero.

If the rules define a role of "President", then replace 1 in the above equation with 3 when P is the President.

Then, the player(s) with the greatest Endorsement Scores have their rule submission enacted, the same as if they had won through guessing.

The information about who Endorsed whom is revealed by the Game Adminstrator along with everything else at the end of the round.

### Limbo

Between rounds, the game is still ongoing unless the Game Adminstrator announces otherwise. Game actions may still be taken and the rules still apply.


## Contract law

A contract is a document that specifies obligations under certain conditions, interpreted and enforced by the Game Adminstrator.

An obligation is a restriction on the actions that a gamer may take as part of the game.  Such restrictions may be positive, requiring a party to take a certain action, or negative, forbidding them from doing so.

A party to a contract is a gamer who has signed it.  A signature is any proof that a party has accepted the contract that the Game Adminstrator is willing to accept.

The Game Adminstrator must refuse a signature if it cannot be proven that the obligations of the contract would be feasible or possible for the gamer signing to do without the contract.

Once somebody becomes party to a contract, they are bound by the contract's obligations for as long as the contract lasts.  Even if a party does not explicitly take obligated actions, the game proceeds as if they had.

Contracts persist across rounds. A contract may specify a period of time for which it lasts; if not, it lasts until the end of a round.

Contracts may specify circumstances under which parties may unsign that contract.  If not, then it is not possible to unsign the contract while it lasts.

Contracts may be made in public or private.  The Game Adminstrator must list other parties to a signed contract on request, and signatures to public contracts are always available.

All contracts must have a unique title.


## Daemons

Any gamer may summon a daemon by specifying the terms of a contract.

The daemon is then bound by that contract, and exists as long as the contract remains in force.

A daemon may participate in the game as if it were a gamer, but may not become a player (and thus may not submit submissions in rounds).
In particular daemons may own marbles and sign other contracts.

It is acceptable to refer to daemons using any string that matches the regex `^d[aeiou]+mon$`.


## Admitdiot Bugger-Up

If it is discovered the outcome of the game is undecidable, the Game Adminstrator must repent for permitting such circumstances to occur, and then arbitration is entered.


## Marbles

Each gamer has a number of marbles that carry on into future rounds. This amount is public information.

Every gamer starts with zero marbles, and earns one marble for each correct guess they make during the guessing phase.

If a gamer tries to do an action that would result in somebody having fewer than zero marbles, that action fails, with the gamer being told "you have lost your marbles".

The following actions can be made using marbles:
1. Rolling a marble - gives one of your marbles to a specified gamer
2. Shooting a marble - uses one of your marbles to remove one marble from a specified gamer


## Itums

Itums have a name and description. Optionally they can have a little drawing too. There can not exist identical itums.
If an Itum does not have a little drawing, any gamer may give it one.

When an Itum is held by some gamer, that gamer is affected by the Itum's description, as interpreted by the Game Adminstrator.

Itum descriptions may cause changes to game state, and grant exemptions from the rules, but not change the rules text.

Itums require pompous names paired with deadpan effect descriptions.

The Game Adminstrator names minimum bid amounts for all wagon Itums, and may change them at will.
This minimum bid consists of some amount of marbles, which may be negative.


### The Swindler and their Wagon

The Swindler is an esteemed role, an important member of the community who supplies itums to those most in need.
Their Wagon is a persistent collection of itums and prices.

The Swindler may do each of the following, at most once each per instance of being the Swindler:
- discard a chosen Itum from the wagon
- create a new Itum in the Wagon, by providing to the GA its name, description, and optionally its little drawing
- sellout, choosing another gamer or the GA to become the Swindler. Each gamer may be Swindler at most once per round.

If who's the Swindler is unclear, or if they have not taken any of the above actions for half a Pluto-day (~3 Earth-days), the GA may choose a new Swindler, as if the current Swindler had sold out.

### Till

When a gamer moves to buy an itum, the itum is taken from the Wagon and an auction is started.
Any gamer may bid a number of marbles, not less than the minimum bid for that itum, and does so privately.
Bids are rejected if they cannot be proven payable.
The gamer who caused the auction to start must bid on it. If they are unable to do so, the auction is cancelled.

When bidding ends, the gamer with the highest bid gets the itum, and they pay the second highest bid, or the minimum bid if they're the only bidder.
In case of a tie the winner is chosen randomly and the highest bid is the same as the second highest bid.

No auction may be started on an Itum that lacks a little drawing.

### The farmers market

The farmers market is a place where a gamer can sell their carrots, potatos, onions, and other itums to other gamers. The market is open during limbo and the submission phase. The gamer selling the itum may set the price and method of sale, for example first come first serve or an auction. Once the transaction has been confirmed, the price and itums are transferred as appropriate.


## Winning

Winning is the achievement of complete control over the game.

A record of the number of times each gamer has won so far is to be kept forevermore. This record is not to be changed under any circumstances.

Submissions that attempt to change or nullify this section of the rules are invalid.


## Insert Tits Here

The Game Adminstrator may choose to give gamers Tit(le)s, to slack off on work.

Tit(le)s must be amusingly named, if they are found not they are instantly revoked.

There is only one of each Tit(le), and the Game Adminstrator may grant and revoke them.

A Tit(le) grants the holder the Game Adminstrator's abilities from a selection of the rules text. That is, the Game Adminstrator picks a subset of the rules text (not necessarily contiguous), and a gamer - this selection of the rules text now applies as though instances of "the Game Adminstrator" (et sim.) were replaced with the gamer's name.


## Meow Meowing
 
Gamers may meow, bark, or produce other such cute animal sounds.  These actions will be collectively referred to as “meowing”.  Meowing is classified as a game action.
 
The gamer which has proven they have meowed second most this round is the Meow Meower Subordinate.
 

## The Bored
The Bored is an 8x8 grid of square tiles. Tiles are indexed with letters and numbers from a1 to h8.
A Piece is any entity with a defined position on the bored.
Any number of pieces may share a square.
A visualization should be made available showing the positions of every piece.

Every piece has the moveset of a particular piece from chess, shogi, xiangqi, or chaturanga.
If such a moveset depends on directionality, then the piece has an associated direction on the bored, corresponding to the forward direction in its source moveset.

Every piece has a natural number of shoes, starting at 0. A piece may spend 1 shoe to make 1 move
according to its moveset. This is the only allowable way for pieces to move.
Shoe-holding entities may freely exchange shoes between themselves, if they so choose.

Every non-daemon gamer is a piece, moving like the queen from chess, and initially positioned on square a1.
At the end of each round, each player of that round recieves 5 shoes.
Once per round a player may change the kind of piece they move like (and associated direction), to any other permissible option.

Daemons may become pieces if their binding contracts specify so. The daemon's contract must then
specify which kind of piece it moves like, as well as its starting position and direction.

### Buildings
Buildings are Pieces with a description.
Buildings may or may not be able to move. If they can, their description must specify how and under what circumstances. In either case the description must specify the building's initial position.
A building may affect entities that share a bored square with it, according to its description.
This works exactly the same as how an itum affects its holder: buildings may alter game state
and grant exemptions from the rules, but not alter the rules text.

Any gamer may build a building by providing a description to the GA, who in turn specifies a build cost in marbles.
If that gamer is able and willing, they may pay this cost, in which case the building gets built.


## Presidential Selections

A presidential selection takes place every odd numbered round, during which the following happens:

During stage 1 any gamer may submit a presidential ticket, consisting of a contract text yet unsigned.
In stage 2 these tickets are revealed publicly, including who wrote each; subsequently, players may vote for any subset of the set of candidates.
In stage 3 the candidate who appeared in the most voters’ subsets (with ties broken by lowest marble count) wins the selection, becomes the President, and is immediately bound by the text of their submitted ticket contract for as long as they are President.
If lowest marble count fails to break the tie, the Game Adminstrator must arrange a fair and reasonable alternative tiebreaker.

As soon as reasonable after the selection, the President (new or reselected) must choose a cabinet, assigning each governmental office to some gamer.
For each office, the President may not choose themselves or anybody who doesn't want to be chosen.
A government officer may resign at any point, in which case the President must choose a replacement, subject to the same rule above.


## The Treasurer

The Treasurer is a government office. 
The Treasure is a marble balance, separate from that of any gamer, which the Treasurer may roll marbles from as if it were their own.
Marbles may be rolled to the Treasure, but not shot at it.

When a gamer is taxed n marbles, it means that n of their marbles are forcibly rolled to the Treasure.
A gamer may not take an action if they can't pay all taxes associated with that action.
At the beginning of each round, each gamer is taxed the smallest of {0 marbles} and half their marble count rounded down.
When a gamer pays for an item at the farmers market, they are taxed {whatever you think is fair no lying allowed}.
When a gamer pays for an item at the swindler's wagon, they are taxed {1 marble if you've had a non-zero amount of marbles for at least a whole round, 10³⁸ marbles otherwise}.

The Treasurer may freely edit text contained in curly brackets in the above paragraph, as long as the replacement text:
- resolves to some number of marbles
- does not have any side effects (aka. does not cause changes to the game),
- does not itself contain any curly brackets.

Such changes must be announced publicly when they occur.


## The Herstorian

The Herstorian is a government office. The Herstorian is responsible for documenting interesting things that happen during their term, and compiling this account into a document called the Herstory, which is publicly available. The Herstorian may also, at their discretion, compile introductory resources, summaries of the rules, etc, for the benefit of new or returning players.


## Hats

Hats are a badge of honor. Hats come with a name and optionally a picture. The President can give any number of hats to any number of players they wish to reward for their actions. Gamers can refuse a hat that the President is trying to give them. Any gamer may give one of their hats to another gamer as an action if that gamer's willing to accept it.

Gamers can choose which of their hats they're currently wearing. A gamer can wear at most one hat a time.

## The Octahedron

The Octahedron is supreme.  No infintesimal may come to be above it.  The Octrahedron cannot begone.  A chain of events does not lead to the Octahedron's non-existence, for a lack of existence of the Octahedron necessitates those events do not exist.  You cannot not have what permits to have.
 
- The Octahedron exists iff the Game continues.
 
-# *Our product proposes a unification of this existential existence's extermination, providing a centralised solution to the destruction of all, and hereby obviating any from the need to spend time considering why they exist: it's as simple as not using the unified destructor.*
 
### The Oct
 
Those that hold a face are collectively known the Oct.
 
When there is a disagreement over how the game should continue, a contradiction in the rules, a vote is started.  All allocated faces of the Oct must participate.
 
Instant Runoff Voting is used:  Each participant ranks the proposed paths from one to N.  If every participant's 1st is the same, it happens from source of the Octahedron.  Otherwise the paths with the least 1sts are eliminated, the gaps in each ranking shifted up, and loop recounting the 1st.
 
When three faces gather, they may agree to re-allocate any faces to and from any Gamer, except those necessitated by the rules.
 
The following must have a face:
- The Game Administator
- The Attorney Specifc, which is a Governmental Office.
- The daemon “Two wolves and a lamb deciding what to eat for lunch.”, if such a daemon exists.
- The Meow Meower Subordinate.
 
-# *All forgets.  Since time unrememerable, each face has been separated in space.  However, for all to exist the Octahedron must be, so it is presumed there is a fourth dimension - linking all together.*

-# *SUB WOOF WOOFER*

## Appendagealism

Going around the most recent player list, each player may append a word and optional punctuation mark to the end of the rulebook. They must be able to know the contents if desired (such as being public, or sent to them). When reaching the end of the player list, repeat.

Appended edits are inserted into the rulebook just like winning submissions, and thus go into effect only at the end of the round.

Edits made by appending aren't considered rules until completed by appropriate punctuation.

<sub>“Appendagealism – A rare term referring to a philosophy or view that emphasizes the importance of attachments or secondary elements in a system.”—ChatGPT</sub>


### Appendage

when the impostor is REQUIRED to submit, they leak their entry's first syllable publicly. This impostor is the second kinkmaster to president in one election. Elections erect loudly when you squeeze your hat (cost: your innate hnngnm marble blaster).

