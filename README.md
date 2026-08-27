# ECE 2112 - Experiment 1: Introduction to Python Programming

Balagtas, Jacob T.

2ECE-B

8/27/2026

## Objective of this Activity

The objective of this experiment is to hone and develop basic python skills through different activities. In these activities we would use basic python functions, operators, string operations. Additionally, it manipulates strings by slicing, indexing, and built-in string methods. The activities below are: Word Rotation Problem, Username Builder Problem, Bookend Swap Problem.

## A. Word Rotation Problem

**Goal:** Create a function **rotate_word(text)** that moves the first character of the word to the end of the word itself.

### Code:

    def rotate_word(text):
      return text[1: ] + text[0]

This code defines the **rotate_word** function, which has the ability using a string to take the first character of the word to the end of it. For **text[1: ]**, the method used here is string slicing which extracts the index ‘1’ from the word to the end of the string. On the other hand, **for text[0]**, instead of string slicing, it uses string indexing to get the first character of the word. Next, the operation **+** combines the sliced string and the first character from the first two functions. Lastly, the **return** function produces the results.

Example:

    def rotate_word(text):
      return text[1: ] + text[0]
      print(rotate_word(“Cellphone”))

Using this code, it will transfer the chapter “C” which is the first character to the place of the last character. This will result in the newly arranged word, **ellphoneC**.

## B. Username Builder Problem

**Goal:** Create a function **make_username(first_name, last_name):** that combines both names with a “.” in between to create a username.

### Code:

    def make_username(first_name, last_name):
        first_name = first_name.lower().replace (“ “,””)
        last_name = last_name.lower().replace (“ “,””)
        return first_name + “.” + last_name

This code defines the **make_username** function that combines the first name and last name with a period in between to create a username. The function **.lower()** converts all the characters of both the first and last names into lowercase and the **return** function will show the results.

Example:

    print(make_username(“Jacob”, “Balagtas”))

Using this code with the given code above, this will result in **jacob.balagtas**.

## C. Bookend Swap Problem

**Goal:** Create a function **swap_bookend(items):** that swaps the positions of the first and last characters of the list while keeping the elements in the middle in place.

### Code: 

    def swap_bookends(items):
        first, *middle, last = items
        return [last] + middle + [first]

This code defines the **swap_bookends** function that takes a list and “swaps” or exchanges the positions of the first and last elements while keeping the middle elements intact.

Example:

    print(swap_bookends([1, 2, 3, 4, 5, 6]))

Result:

    [6, 2, 3, 4, 5, 1]

Notice the first and last element, which is 1 and 6, respectively. The second line in the code shows their original positions, while the last line in the code with the **return** function shows that the first and last swapped places but the middle stayed in its place.
