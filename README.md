# COMP 202 – Assignment 3: Word Search

This repository contains my solutions to COMP 202 Assignment 3 (Winter 2023, McGill University).  
The assignment implements a simplified word search puzzle solver in Python, broken into multiple modular functions.

---

## Description
Given a list of letters and a list of words, the program:
1. Locates each word in the letter list (left-to-right or right-to-left).
2. “Crosses out” found words by replacing their letters with `*`.
3. Collects remaining letters in order to form the hidden magic word.

---

## Implemented Functions
1. **`is_outside_list`** – Checks if an index is outside list bounds.  
2. **`letter_positions`** – Returns all indices where a character occurs.  
3. **`valid_word_pos_direction`** – Validates if a word exists from a position in a given direction.  
4. **`direction_word_given_position`** – Finds all directions a word can be read from a position.  
5. **`position_direction_word`** – Returns all positions/directions where a word occurs.  
6. **`cross_word_position_direction`** – Replaces found word letters with `*` at a given position/direction.  
7. **`cross_word_all_position_direction`** – Crosses out all occurrences of a word.  
8. **`find_magic_word`** – Returns the hidden word from uncrossed letters.  
9. **`word_search`** – Orchestrates finding and crossing all words, returns the magic word.  
10. **`word_search_main`** – Reads puzzle input from a file and outputs the magic word.

---

## Example
Letter list:  
`['C','W','I','K','I','P','E','D','I','A','O','M','M','O','D','N','A','R','P']`  
Words: `['WIKIPEDIA','RANDOM']`  
Magic word:  COMP
