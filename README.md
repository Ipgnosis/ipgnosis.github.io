# ipgnosis.github.io

The github pages site of Ipgnosis

## Project 1: Exploring Machine Learning via [Tic-Tac-Toe](https://https://github.com/Ipgnosis/tic_tac_toe)

**This project is a work in progress: see current status in the repo linked above.**


This project was inspired by [Google's AlphaZero](https://deepmind.com/blog/article/alphazero-shedding-new-light-grand-games-chess-shogi-and-go). However, AlphaZero's learning process is opaque, and this doesn't expand my knowlege of how software can learn the problem space. This project is a process through which a human can understand the way that computers learn from first principles.

### Sidebar:
Humans don't learn games such as Tic Tac Toe, Chess or Go by doing any of the following:

1. Exhaustively studying rules, strategies and tactics
2. Exhaustively studying all the great games played by past masters

When learning a game, humans typically learn just enough to start playing the first game, then they play and learn as they go along. During game play, humans typically do not:

* Start a game with a proven strategy in mind (e.g. 'Sicilian Defense', 'Ruy Lopez', etc.)
* Conduct an exhaustive search of all possible moves (*NB even in Tic Tac Toe, there are 9! or 362,880 possible moves*)
* Calculate win/loss probabilities for any given move
* Explore the history of great games played in the past, looking for similarities

What humans actually do is scan the current situation, and make an almost subconscious assessment of risk/reward before selecting the next move most likely to win; if winning is less likely, then they are playing for a draw.  This has been confirmed by Garry Kasparov's book: **'Deep Thinking: Where Machine Intelligence Ends and Human Creativity Begins'**; where he explains how this game intuition is developed through rigorous practice.

### Goal:

The goal of this project is to get the computer to learn Tic Tac Toe as a child learns: through the experience of play, basing their decisions on their recollection of what worked or didn't work in the past.
