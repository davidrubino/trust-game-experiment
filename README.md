# trust-game-experiment
Implementation of an experiment to simulate trust between users

The experiment follows this protocol: a group of users are paired with one another in teams of 2. Each team exchanges a certain amount of money,
that is multiplied during each turn. For each round, each user has the choice to send back the amount he received, send more money, or send nothing.
In the latter, the game ends.

At the end of a game, each user is given a score. The score doesn't match the money received, but it is a trust factor that determines if a user is trustworthy of not
(typically if the user decides to keep all the money he has a low score whether the user who sends more money will have a higher score).

During the next round, each user will see the score of his opponent. The goal of the experiment is to determine whether a trust score will influence users into making decisions of sending more or less money.
Also, two players will not play together consecutively.

There are two implementations of this experience:
- a Java/JavaFX client-server application based on the RMI API
- a ZTree application (a software created by the University of Zurich in order to implement trust and financial experiments)
