# Word Finder Challenge

## Introduction
This repo contains different algorithms to find a list of words in a 2D char matrix.
The algorithms count all the occurrences of each word in the matrix and return a list of the words found in the matrix (from the original list), ordered by their frequency in the matrix.

The algorithms only search words horizontally or vertically.

The solution contains 2 algorithms (so far):
  - A **slower** one which does a secquential search (checks if each word is in the matrix by iterating through all the columns and rows)
  - A **faster** algorithm which implements a "Trie" structure and a Depth-First Search

The solution also contains some tests to check each algorithm and how much time each one takes when using a 64x64 matrix and long words (the challenge mentions the matrices would be 64x64 at most).

More tests will be added in the future...

### Why use two algorithms?
Being that the **secquential search** algorithm is more efficient in terms of <ins>memory usage<ins> (but requires more processing time) and the **DFS** one is more efficient in <ins>CPU usage</ins> (but requires more memory to allocate the different structures), and given that I have not been able to make an algorithm that uses little CPU and memory at the same time (and think it would be difficult to do it), I think it is nice to have several options that have different pros/cons to be able to choose the right one for each case. 


## Folder Structure
The "Docs" folder contains the original challenge description and a document explaining assumptions (based on the given description) and ideas used to develop the algorithms

The "src" folder contains the C# classes that contain the algorithms (it was developed using a strategy pattern).

