Hangman Game

Welcome to the Hangman Game! This project is a classic word-guessing game implemented in Python, where players attempt to guess a hidden word one letter at a time before running out of attempts.

Project Structure

The project consists of the following files:

hangman.py: The main script that runs the game logic. It handles player input, game progression, and outputs the current state of the game.

hangman_words.py: A Python module containing a list of potential words that the game will choose from.

hangman_art.py: A module that provides the ASCII art for the hangman stages and a logo for the game.

How to Run the Game

Ensure that you have Python installed on your system (Python 3.x recommended).

Clone or download this repository to your local machine.

Run the game by executing the hangman.py script:

python hangman.py

Follow the on-screen instructions to play the game by guessing letters.

Gameplay Overview

The game randomly selects a word from the word_list in hangman_words.py.

The player is shown blanks representing the letters in the word.

The player guesses one letter at a time.

Correct guesses reveal the position of the letter in the word.

Incorrect guesses reduce the player's number of lives and display a progressively complete hangman ASCII art.

The game ends when the player either guesses all the letters correctly (win) or exhausts all attempts (lose).

Features

Word List: A curated list of unique and challenging words in hangman_words.py.

ASCII Art: Visual representation of the hangman stages, providing an engaging user experience (hangman_art.py).

Logo: A simple logo to display at the start of the game for a polished look.

Sample Code Snippets

Choosing a Word

import random
from hangman_words import word_list

chosen_word = random.choice(word_list)
word_length = len(chosen_word)

Checking Player Input

if guess in display:
    print(f"You've already guessed {guess}")

if guess not in chosen_word:
    print(f"You guessed {guess}, that's not in the word. You lose a life.")
    lives -= 1

Displaying Game State

from hangman_art import stages, logo

print(logo)
print(stages[lives])


Enjoy playing Hangman and challenge yourself to guess the word before the hangman completes!

