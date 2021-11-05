# ipgnosis.github.io

Welcome to the GitHub Pages site of Ipgnosis LLC and, by extension, Russell Bennett. You can see more about me on [LinkedIn here](https://www.linkedin.com/in/russellpbennett).  Here is a quick summary of what I am currently working on (and am able to share).

## Project 1: Exploring Machine Learning via [Tic-Tac-Toe](https://github.com/Ipgnosis/tic_tac_toe)

**This project is a work in progress: see current status in the repo linked above.**

This project was inspired by [Google's AlphaZero](https://deepmind.com/blog/article/alphazero-shedding-new-light-grand-games-chess-shogi-and-go). However, AlphaZero's learning process is opaque, and this doesn't expand my knowlege of how software can learn a problem space. This project is a process through which a human can understand the way that computers learn from first principles.

### Preamble:
Humans don't learn games such as Tic Tac Toe, Chess or Go by doing any of the following:

1. Exhaustively studying rules, strategies and tactics
2. Exhaustively studying all the great games played by past masters

When learning a game, humans typically learn just enough to start playing the first game, then they play and learn as they go along. During game play, humans typically do not:

* Start a game with a proven strategy in mind (e.g. 'Sicilian Defense', 'Ruy Lopez', etc.)
* Conduct an exhaustive search of all possible moves (*NB. even in Tic Tac Toe, there are 9! or 362,880 possible moves*)
* Calculate win/loss probabilities for a move
* Explore the history of great games played in the past, looking for similarities

*However, this is pretty much how all computer versions of board games work.*

What humans actually do is scan the current game state, and make an almost subconscious assessment of risk/reward before selecting the next move most likely to win.  If winning appears less likely, then they are playing for a draw.  This has been confirmed by (former World Chess Champion) Garry Kasparov's book: **'Deep Thinking: Where Machine Intelligence Ends and Human Creativity Begins'**; where he explains how this game intuition is developed through rigorous practice.

### Goal:

The goal of this project is to get the computer to learn Tic Tac Toe as a child learns: through the experience of play, basing their decisions on their recollection of what worked or didn't work in the past.

Once this is working properly, the next step will be to get the program to write the rules it derives in human readable form.

## Project 2: [Analysis of Covid data via Jupyter Notebooks](https://github.com/Ipgnosis/covid_analysis)

**This project is a work in progress: see current status in the repo linked above.**

Like many others, I have been fascinated (and horrified) by the Covid-19 pandemic. I have many questions for which I am unable to find answers: so here is my attempt to find answers for the questions below.

*Note that I switched over from using pandas, because my ultimate goal is to share this data on a website.*

### Hypotheses:
1. Economic strength correlates to high performance in pandemic management
2. Population density correlates to contagion
3. Underlying health has had an effect on infection and death
4. Government policy has affected infection & death rates
5. National culture has an effect on contagion
6. Winter means more cases
7. Islands are better at managing infection?

### Questions:
1. How have counties performed overall?
2. How has country performance changed over time?
3. Has GDP had any effect on performance?
4. Has geography, population density, culture and seasons played a role in contagion?

### Data Source:
Most of the quantitative data is provided by [Our World in Data](https://ourworldindata.org) (see citation in footnote i. below) which is a project based at the Oxford Martin School of the University of Oxford, UK. As described on their [coronavirus pages](https://ourworldindata.org/covid-sources-comparison), this data is based on a range of sources, but particularly from the European Center for Disease Control and Prevention as well as Johns Hopkins University.

(i.) Max Roser, Hannah Ritchie, Esteban Ortiz-Ospina and Joe Hasell (2020) - "Coronavirus Pandemic (COVID-19)". Published online at OurWorldInData.org. Retrieved from: 'https://ourworldindata.org/coronavirus' [Online Resource]


## Project 3: [Python 'Like' function](https://github.com/Ipgnosis/like)

**This project is a work in progress: see current status in the repo linked above.**

A string compare function that analyzes to what extent string A is similar to string B.

### Background

This idea came from working on a different project (see above) where I kept misspelling the country name 'Kazakhstan' as 'Khazakstan'.  I searched for a 'like' function in Python and found none.  This is strange, because this has been implemented in other languages before: there are even 'sounds like' functions (i.e. 'soundex').  So, just for fun, I thought I would give it a shot.  I expect that this will be a lot easier than implementing a spelling checker (or learning how to spell...)

### Ultimate goal

An extension of the string object that adds a 'like' operator to test equivalence.  This will enable 'Khazakstan' to match to 'Kazakhstan'.

**Note that this is not a spelling checker.**

### Implementation

The initial implementation will evaluate some kind of probability function.  As a comparison, I will test against the work of [Damerau-Levenshtein](https://en.wikipedia.org/wiki/Damerau%E2%80%93Levenshtein_distance).

This will be useful for handling 'typos' emanating from keyboarding errors (aka transpositions, e.g. 'typo' vs. 'tyop') that have found their way into data, thereby causing search failures.

This is *particularly useful* when a string contains international characters (that aren't available on all keyboards), for example:

* ñ: the Spanish letter 'eñe'
* ü: the German (etc.) letter u with an umlaut
* ç: the French c-cedilla
* ß: the German letter 'eszett'

(*I suspect that the Cyrillic character set is overly ambitious...*)

Note that the eszett (and maybe others also) is a complication of the general problem in that two letters 'ss' can be substituted for the eszett when the keyboard/character set in use doesn’t contain the eszett.  For example: the German word for 'street' is 'straße' which can also be written 'strasse'.
