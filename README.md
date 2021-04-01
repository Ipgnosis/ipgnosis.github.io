# ipgnosis.github.io

The github pages site of Ipgnosis

## Project 1: Exploring Machine Learning via Tic-Tac-Toe

**This is a work in progress**

This project was inspired by [Google's AlphaZero](https://deepmind.com/blog/article/alphazero-shedding-new-light-grand-games-chess-shogi-and-go). However, AlphaZero's learning process is opaque, and this doesn't expand my knowlege of how software can learn the problem space. This project is a process through which a human can understand the way that computers learn from first principles.

### Sidebar:
Humans don't learn games such as Tic Tac Toe, Chess or Go by doing any of the following:

1. Exhaustively studying rules, strategies and tactics
2. Exhaustively studying all the great games played by past masters

What they actually do is learn enough to start playing the first game, then they play and learn as they go along. During early game play, humans do not:

* Start a game with a proven strategy in mind (e.g. 'Sicilian Defense', 'Ruy Lopez', etc.)
* Conduct an exhaustive, breadth first search of all possible moves (*NB even in Tic Tac Toe, there are 9! or 362,880 possible moves*)
* Calculate win/loss probabilities for any given move
* Explore the history of great games played in the past, looking for similarities

### Goal:

The goal of this project is to get the computer to learn Tic Tac Toe as a child learns: starting with just enough information to play and then learning by experience of play, basing their decisions on their recollection of what worked or didn't work in the past.
