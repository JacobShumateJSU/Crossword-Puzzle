# Crossword-Puzzle
#### This is a crossword puzzle game written in python. When you run the program there are three options:(G) Guess Word, (C) Show Clue, (R) Show Grid, (Q) Quit. Guess word allows you to guess a word on the grid. Show clue allows you to receive a hint for any word on the grid. Show Grid allows the player to view the grid, and Quit will exit the game. There are 84 words to guess and they are imported through a .csv file and then displayed onto the crossword grid. The grid is composed of ASCII characters and each character in a word that has not yet been guessed is hidden. The objective is that of a standard crossword puzzle, guess as many words as you can. 

# Running the Crossword puzzle

###### *In order to run this program, you must have python 3 installed.*

### Installing Python 3
* Linux
  * Open up terminal 
  * Type the command: "sudo apt-get install python3.6" replace "apt-get" with your distro's package manager
* Mac OS X 
  * Open up terminal
  * If you have homebrew package manager just type "brew install python".
* Windows
  * Download the latest release of python from https://www.python.org/downloads/windows/
  * During installation, make sure to select option "Add Python to PATH"

#### Once the previous steps are complete, open your command line and make sure you're in the same directory as puzzle.csv and CrossWordPuzzle.py and simply run the command `python CrossWordPuzzle.py`

# Functions Documentation
###### *This program uses 6 separate functions.*
Function | Purpose
------------ | -------------
main() | Initializes core variables, prompts user for input, and then evaluates what to do depending on what the user entered.
createGrid() | Enumerates through a for loop to populate a grid of 15x15 ascii characters. Initializes the grid.
findWord() | Function parameters are user input. Searches grid to see if the word that the user entered exists.
readPuzzle() | Reads the data from puzzle.csv and stores them into a dictionary 
addWordtoGrid() | Populates the grid with words that were read from the puzzle.csv file
printGrid() | Executed when user input is R or Show Grid. This function displays the grid to the user.

# Important Variables 
Variable Name | Value
------------ | -------------
guessedwords | keeps track of how many words the user has correctly guessed
puzzle | Input from puzzle.csv file
grid | The grid itself composed of strings
userinput | Stores user input from keyboard which determines which function to execute
word | Stores the user's guessed word in order to search for its' existence

# Python Libraries Used 
   * sys
   * csv

