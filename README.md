# ECE 2112 - Experiment 1: Introduction to Python Programming

Balagtas, Jacob T.

2ECE-B

8/27/2026

## Objective of this Activity

The objective of this experiment is to hone and develop basic python skills through different activities. In these activities we would use basic python functions, operators, string operations. Additionally, it manipulates strings by slicing, indexing, and built-in string methods. The activities below are: Word Rotation Problem, Username Builder Problem, Bookend Swap Problem.

## A. Word Rotation Problem

**Goal:** Create a function **rotate_word(text)** that moves the first character of the word to the end of it.

### Code:

    def rotate_word(text):
    
      return text[1: ] + text[0]

This code defines the **rotate_word** function, which has the ability using a string to take the first character of the word to the end of it. For **text[1: ]**, the method used here is string slicing which extracts the index ‘1’ from the word to the end of the string. On the other hand, **for text[0]**, instead of string slicing, it uses string indexing to get the first character of the word. Next, the operation **+** combines the sliced string and the first character from the first two functions. Lastly, the **return** function produces the results.

Example:

    def rotate_word(text):

      return text[1: ] + text[0]

      print(rotate_word(“Cellphone”))

Using this code, it will transfer the chapter “C” which is the first character to the place of the last character. This will result in the newly arranged word, **ellphoneC**.
