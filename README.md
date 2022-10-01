# alt_wordle

Project #1 for General Assembly software dev course 

[Wordle Project](https://ultimatebbqribs.github.io/alt_wordle/)


# Wordle breakdown

# Actions

- Render initial view state
    - Function to set 5x6 grid /
    - Header & default page css, background color, max width
    - Set keyboard
        - HTML div’s in a span for each line
        - ID is corresponding letter
        - two classes, keyboard and keyboard row(top, middle, bottom)
        
- Computer Picks Word
    - Create array from list of common words
    - Global variable for computer word set with empty string
    - Function to choose computer word
        - Random number generator picks number
        - Number used to pick array item
        - loop over word variable to create array of individual letters and push to computer word variable as uppercase
        
- User enters guess
    - Function to listen for button and keyboard inputs
        - event ID is stored as variable for user guess
        - keyboard input is lower cased, then stored in user guess variable
        - Event ID, aka chosen letter, is printed in grid as user guess
        - Special keys backspace to pop() array, and enter to submit answer
        
- Guess checked against computer word - change css on tile and keyboard for result
    - function check result
        - Conditional logic for if match true/false
        - if exact match green
        - if partial match use yellow - or a better color blind colour
        - else no match change nothing

- Repeat until win or lose state
    - function win
    - conditional check using 5x AND statements
- Render win/lose state
