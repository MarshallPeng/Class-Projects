# Marshall Peng
## Class Projects

## Tiny Search Engine - C - CS50

A Search engine that consists of three parts: a Crawler, Indexer, and Querier. 

* A crawler is the first of three subsystems of the Tiny Search Engine. The crawler crawls a website and fetches URLS that are found in it, then crawls the pages found using those URLs until the crawler has reached a certain maxdepth.
* The Indexer is the second sub-system of the TSE. The job of the indexer is to read files produced by crawler. Then build an inverted index mapping from words to documents, and write that index to a file.
* The Querier is the third sub-system of the TSE. The querier reads the index file produced by the TSE Indexer, and page files produced by the TSE Querier, and answers search queries submitted through stdin.

## Parts of Speech Tagger - Java - CS10

Sudi is a parts of speech tagger that, given training sentences and tags, labels each word in a sentence with its part of speech (noun, verb, etc.) I use a statistical approach to solve this problem since a word can have different parts of speech in different contexts. To implement this, I used the Viterbi Algorithm on Hidden Markov Models.

## Kevin Bacon Game - Java - CS10

Given data files containing actors, movies, and actors-to-movies information, this program finds an actor's "Bacon number." An actor's Bacon number is found in the following way. Starting with an actor, see if the actor has been in a movie with someone who has been in a movie with someone...who has been in a movie with Kevin Bacon. The number of degrees of separation is the Kevin Bacon number. To implement this game, I used breadth-first search to find the Kevin Bacon number.

## Collaborative Graphics Editor - Java - CS10

A graphical editor that has a similar ability as Google Docs, where multiple people can edit one document. So one person can draw a rectangle, and another person can edit, recolor, move, etc. that same rectangle. Each client editor has a thread for talking to the sketch server, along with a main thread for user interaction (previously, getting console input; now, handling the drawing). The server has a main thread to get the incoming requests to join the shared sketch, along with separate threads for communicating with the clients. The client tells the server about its user's drawing actions. The server then tells all the clients about all the drawing actions of each of them.
