# GuessQuest

## Overview
GuessQuest is a simple betting guessing game where the player starts with a certain amount of money and attempts to guess a randomly generated number between 0 and 100. The game provides feedback on whether the guess is correct, and deducts money for incorrect guesses. The game ends when the player guesses the correct number or runs out of money.

## How to Play
1. **Start the Game**: The game begins with an initial amount of 1000 money units.
2. **Make Guesses**: You have up to 10 chances to guess the correct number.
3. **Enter a Guess**: For each guess, input a random number between 0 and 100.
4. **Check Result**: 
   - If your guess is correct, you win the game.
   - If your guess is incorrect, you lose 100 money units and the game prompts you to guess again.
5. **End Game**: 
   - If you guess the correct number, you will be asked if you want to view all your guesses.
   - If you run out of money, the game ends and reveals the target number.

## Game Flow
1. **Initialization**: The game initializes with 1000 money units and generates a random target number between 0 and 100.
2. **Gameplay Loop**:
   - Display the current amount of money.
   - Prompt the player to enter a guess.
   - Check if the guess is correct.
     - If correct, display a win message and optionally show all guesses.
     - If incorrect, deduct 100 money units and display an invalid guess message.
3. **End Conditions**:
   - If the correct number is guessed, the player wins.
   - If the money runs out, the player loses and the target number is revealed.

## Key Functions
- **Game() Constructor**: Initializes the game with a starting amount of money and generates a random target number.
- **getTarget()**: Returns the target number.
- **play()**: Manages the main game loop where the player makes guesses.
- **checkWin(int guess)**: Checks if the player's guess is correct and updates the money accordingly.
- **winPrompt()**: Displays the win message and prompts the player to view all guesses.
- **losePrompt()**: Displays the lose message and reveals the target number.
- **printGuesses()**: Prints all the guesses made by the player.

## Example
Game started!  
Current Money: 1000  
Enter random number between 0-100: 50  
Invalid guess!  
  
Current Money: 200  
Enter random number between 0-100: 75  
You guessed the right number!! You win!!  

Would you like to view all your guesses? [Y/N]: Y  

Guesses: 8  
50  
30  
60  
70  
80  
55  
65  
75  
  
Enjoy playing GuessQuest and test your luck and guessing skills!
