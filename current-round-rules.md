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

The holder of an itum is affected by its description. Interpretation of what each itum actually does is up the the Game Adminstrator.

Itums have the ability to make changes to game state but not change the rules text. If an itum's description conflicts with the rules, the rules take precedence. In particular, if an itum grants an exemption from the rules and the rules don't account for that, then that itum does nothing.

### The Swindler's Wagon

The Swindler is an esteemed role, an important member of the community who supplies itums to those most in need.

Their Wagon is a persistent collection of itums and prices.

The Swindler may optionally:
- discard a chosen itum from the wagon
- provide a description and so on of an itum to stock into the wagon
- recall or change the submission that was submitted by the previous Swindler to the next round if there is one
- submit a rule to the next round. This rule is only allowed to activate when the Itum's description would, and may specify any departures from the text of the rules the Itum is allowed to make. The Swindler then plays as a player in the round, under the title "*as swindled*". The Swindler is considered a distinct player in the round, and whoever is the current Swindler may play as their real identity at the same time; when doing so, they must clarify to the GA the identity they are using for any game action.

Then they sellout, choosing another gamer or the Game Adminstrator to become the Swindler. Each gamer may be Swindler only once per round.

The Game Adminstrator names minimum bids for all wagon itums (which may be negative), and may change them at will. The minimum bid consist of some amount marbles.

If who's the Swindler is unclear, or the they have not taken an action for half a Pluto-day (~3 Earth-days), the Game Adminstrator may take their role.

### Till

When a gamer moves to buy an itum, the itum is taken from the Wagon and an auction is started. Any gamer may bid, and does so privately. All bids must have at least the counts in the asking price or higher, and may not include things not in the price. Bids are rejected if they cannot be proven payable.
The gamer who caused the auction to start must bid on it. If they are unable to do so, the auction is cancelled.

When bidding ends, the gamer with the highest bid gets the itum, and they pay the second highest bid, or the minimum bid if they're the only bidder. In case of a tie the winner is chosen randomly and the highest bid is the same as the second highest bid.

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


## Meowing

Gamers may meow, bark, or produce other such cute animal sounds. These actions will be collectively referred to as “meowing”.
Meowing is classified as a game action.


## The Map

The map is an 8x8 grid of square tiles.
An object is any entity with a defined position on this grid. The map should be made available as a visualization showing the positions of every object.

Daemons may have associated positions on the map, in which case their associated contract specifies how and when they move as well as their initial position.

The Game Adminstrator may veto contracts whose obligations relate to movement, if they deem these obligations may be too complicated to keep track of in practice.


## Buildings

Buildings are objects with a description. 

Buildings may or may not be able to move. If they can, their description must specify how; in any case, their initial position must be described.

Buildings may confer special abilities not covered by the rules, similar to an itum. The building's description must specify this.

Any gamer may build a building by giving a description to the Game Adminstrator, who in turn specifies a build cost in marbles. If the gamer is able and willing, they may pay this cost, in which case the building gets built.


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
When a gamer pays for an item at the swindler's wagon, they are taxed {whatever you think is fair no lying allowed}.

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


## Appendagealism

Going around the most recent player list, each player may append a word and optional punctuation mark to the end of the rulebook. They must be able to know the contents if desired (such as being public, or sent to them). When reaching the end of the player list, repeat.

Appended edits are inserted into the rulebook just like winning submissions, and thus go into effect only at the end of the round.

Edits made by appending aren't considered rules until completed by appropriate punctuation.

<sub>“Appendagealism – A rare term referring to a philosophy or view that emphasizes the importance of attachments or secondary elements in a system.”—ChatGPT</sub>


### Appendage

when the impostor is REQUIRED to submit, they leak their entry's first syllable publicly. This impostor is the second kinkmaster to president in one election. Elections erect loudly when you squeeze your hat (cost: your innate hnngnm marble blaster).

