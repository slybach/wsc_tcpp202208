Word search challenge from tccpp (2022-08).
Credit to the original problem author.

# Problem description
Here is the program specification:
The program is supposed to read 2 files: a letter grid and a dictionary.
Dictionary is a list of words (less than 16 letters long), no spaces, ASCII only, capital letters only, each word in a new line (file finished with a new line).
Letter grid is a file in a form:

    A A A A A A
    A A A A A A
    A A A A A A

ASCII capital letters delimited by spaces, rows delimited by a new line character (file finished with a new line).

In the letter grid, your task is to find as many occurrences of the words from the dictionary as you can.
The words can be positioned in 8 directions.
The words can overlap each other, one word can appear a multitude of times.

Your program needs to print two numbers on the standard output, in separate lines:
1. The number of occurrences of words from the dictionary in the grid (counting duplicates separately)
2. The number of words from the dictionary that are NOT present in the grid

For simplicity, if a word is a palindrome, you count it two times (one way and the other way).

The limit on the Grid size: 256 letters x 256 letters
The limit on the size of the dictionary: 65'536 words
The words in the dictionary are not sorted and do **not** repeat.

You CAN'T use external libraries. You CAN'T use platform dependent/ platform exclusive functions (conio.h, windows.h, unistd.h)
(you can't vote for your own solution during the voting)


## Addendum:
- There won't be any 1-letter words in the dictionary. At least 2-letter words.
- The path to the dictionary will be passed as the first command line argument ([1]), and the path to the letter grid will be passed as the second command line argument ([2]).
