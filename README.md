# MV-TA-Guadalupe-Gomez-Ortiz

ROCK PAPER SCISSORS GAME

randomChoice()
GOAL: Create a randomChoice function that returns a random selection of either "rock", "paper", or "scissors" every time the function is called.

Initialize a function called randomChoice().
Initialize a variable called choice and store the result of Math.random() in the variable.
Multiply Math.random by 3.
Wrap Math.random with Math.floor. Stuck? Click Reveal Content below.
Based on the value stored in choice:
Return the string rock if choice has a value of 0.
Return the string paper if choice has a value of 1.
Return the string scissors if choice has a value of 2.
Call the function and console.log() the result to verify that it works!
Tests 1, 2, and 3 pass at this point

Reveal Content
winner(player1, player2)
GOAL: Create a function called winner that takes two player choices of rock, paper, or scissors. The function should return the winner based on the two player choices.

Declare a function called winner that has two parameters: player1 and player2.
If player1 and player2 have he same value, return the string "It's a tie".
If the value in player1 beats the value stored in player2, return the string "Player 1 Wins!".
E.g. If player1 has a value of rock and player2 has a value of scissors, then the function returns "Player 1 Wins!".
If the value in player2 beats the value stored in player1, return the string "Player 2 Wins!".
E.g. If player1 has a value of paper and player2 has a value of scissors, then the function returns "Player 2 Wins!".
Tests 4, 5, and 6 should be passed here.

Play the Game!
Create a variable called player1 and store the result of randomChoice() in the variable.
Create a variable called player2 and store the result of a separate call of randomChoice() in the variable.
Create a variable called result and call winner with the values stored in player1 and player2.
Log the values of player1, player2, and result to verify your game plays correctly!
Bonus Tasks
Tests have not been written for these, but you can test in your console to verify that it works!

Level 1 Stretch: Rock, Paper, Scissors, Lizard, Spock
Check out the rules here.

Rock Paper Scissors Lizard Spock Rules Visual, text below explains rules.
The rules of the game are:

Lizard eats paper
Lizard poisons Spock
Spock smashes scissors
Spock vaporizes rock
Paper disproves Spock
Paper overs rock
Scissors decapitates lizard
Scissors cuts paper
Rock crushes lizard
Rock crushes scissors
TASK: Update the randomChoice and winner functions to play this version of the game.

Example
let p1 = randomChoice(); // Returns "Spock"
let p2 = randomChoice(); // Returns "paper"
console.log(winner(p1, p2)); // Returns "Player 1 Wins!"
Level 2 Stretch: Create a score Function
Level 3 Stretch: Play Multiple Rounds With a while Loop
TASK: Play 10 rounds of rock, paper, scissors using a while loop.

Go look at Week 2 content on while loops to see how to create counters and repeat code iteratively.
Create a round variable that stores how many rounds have been played.
Initialize round with a value of 0.
Every round should:
Pick a new random value for each player using randomChoice function.
Determine the winner using winner function.
Update the player1score and player2scores variables using the score function.
Play the game for 10 rounds
Output the final score once the game is over
Level 4 Stretch: Build in User Input
TASK: Incorporate user input using the following resources:

Read through this information on creating User Input.
Update your code to incorporate user input.
A few ideas for how to incorporate user input:

Allow the person to input their choice of rock, paper, or scissors. Determine the winner against a random computer choice.
Allow the player to continue playing by prompting them with a question after each round asking them if they want to keep playing. The player can play until they say they are done.
