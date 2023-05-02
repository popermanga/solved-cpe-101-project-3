Download Link: https://assignmentchef.com/product/solved-cpe-101-project-3
<br>
Tic-Tac-Toe Simulator




Your code must pass all of the tests to get any credit. Your grade will be based on the date which your code passes all the tests. To get 100% credit for this project, you must submit in PolyLearn by 11:00PM on 5/9/18. Code that does not pass all of our tests will not get any credit.




Monday      (5/9) – 100% @ 11:00PM

Tuesday      (5/10) – 80%  @ 11:00PM

Wednesday (5/11) – 60%  @ 11:00PM




<strong>Objectives: </strong>




<ul>

 <li>Practice on List</li>

 <li>More practice on writing loops in python.</li>

 <li>More practice on writing and calling functions that you have written.</li>

 <li>Practice testing your code.</li>

 <li>To appreciate the benefits of modular development.</li>

</ul>




<strong>Required File Header:</strong>

All students are required to have the following header comment at the top of their source files. Note that the stuff to the right of the colon in red is information for an imaginary example student. (Please put YOUR appropriate information. Also, your header comment is not expected to have red text.) All program files require this header.




# Project 3 – Tic-Tac-Toe Simulator

# Name: Your Name

# Instructor: S. Einakian

# Section: Your Section

<strong> </strong>

<strong>Resources: </strong>

<ul>

 <li>Your instructor, via office hours, email, etc.</li>

 <li>Free tutoring Sunday-Thursday, 7-9 PM, 14-302</li>

 <li>Your TA</li>

</ul>




<strong>Program Description: </strong>

For this program, you will be writing a simulation for the game, Tic-Tac-Toe. Two people play Tic

Tac Toe with paper and pencil. One player is X and the other player is O. Players take turns placing their X or O. If a player gets three of their marks on the board in a row, column or one of the two diagonals, they win. When the board fills up with neither player winning, the game ends in a draw.

<strong>This program has two parts: </strong>

<ol>

 <li>Two Players</li>

 <li>Play with Computer</li>

</ol>

<strong>Part One: Two Players </strong>

<ul>

 <li>Take user input (for two players)</li>

 <li>Store user inputs into a 3×3 Tic-Tac-Toe board</li>

 <li>Check for validity of inputs (no overriding, proper cell value, etc.)</li>

 <li>Check for a win every turn</li>

 <li>Print the board every turn</li>

</ul>




<strong>Part Two: With Computer </strong>

<ul>

 <li>Randomly pick a player (you or computer)</li>

 <li>Take input (for one players)</li>

 <li>Computer or you will generate the next</li>

 <li>Store user inputs into a 3×3 Tic-Tac-Toe board</li>

 <li>Check for validity of inputs (no overriding, proper cell value, etc.)</li>

 <li>Check for a win every turn</li>

 <li>Print the board every turn</li>

</ul>




<strong>Getting Player Input: </strong>

<ul>

 <li>Each player will input a number (1-9) which corresponds to the following cells.</li>

</ul>

<table width="109">

 <tbody>

  <tr>

   <td width="36">1</td>

   <td width="36">2</td>

   <td width="36">3</td>

  </tr>

  <tr>

   <td width="36">4</td>

   <td width="36">5</td>

   <td width="36">6</td>

  </tr>

  <tr>

   <td width="36">7</td>

   <td width="36">8</td>

   <td width="36">9</td>

  </tr>

 </tbody>

</table>




<ul>

 <li>Location 0 in list corresponds with number 1</li>

 <li>Players’ input will be stored in a list.</li>

 <li>Players will take turns.</li>

</ul>




<strong>Checking For a Win: </strong>

<ul>

 <li>A player wins if there is a sequence of 3 of the same letter in the same row, column, or diagonal.</li>

</ul>




<strong>Printing Output: </strong>

<ul>

 <li>You should use for loops to output a 3×3 board.</li>

</ul>

<strong> </strong>

<strong>General Notes: </strong>

<ul>

 <li>You should implement your functions in a file, <strong>py </strong> Checking for a win requires multiple operations.</li>

</ul>




<strong> </strong>

<strong>Functions: </strong>

<ol>

 <li>Welcome

  <ol>

   <li>Welcomes user to the game and explain the game rules.</li>

   <li>You will provide your own Welcome information</li>

   <li>Ask user to decide if playing with computer (pass 1) or another player (pass 2)</li>

   <li>No parameter to pass</li>

   <li>Return 1 if play with computer and 2 if plays with another player</li>

  </ol></li>

</ol>




<ol start="2">

 <li>createBoard

  <ol>

   <li>You will use a list to store the data</li>

   <li>List has 9 items starting from index 0 to 9 which holds the values (X or O)</li>

   <li>This function has no parameter to pass and it return a list</li>

   <li>Your game board at first should look like the following:</li>

  </ol></li>

</ol>




1   |   2  |   3

—————

4   |   5  |   6

————— 7   |   8  |   9




<ol start="3">

 <li>printBoard

  <ol>

   <li>The printBoard function will print the game. Remember that the board is represented as a list of nine strings, where the string at index 0 is the mark on space 1 on the Tic Tac Toe board, and so on.</li>

   <li>Passing a list as the board to the function.</li>

   <li>The first call to the print will show an empty board game:</li>

  </ol></li>

</ol>




|      |

—————

|      |

—————

|      |




<ol start="4">

 <li>pickLetter

  <ol>

   <li>This function ask user to pick ‘X’ or ‘O’</li>

   <li>No parameter to pass</li>

   <li>This will return the letter of player’s choice</li>

   <li>If user enters the wrong letter you need to ask user to reenter the letter</li>

   <li>This function return letter</li>

  </ol></li>

</ol>




<ol start="5">

 <li>getInput

  <ol>

   <li>This function takes the letter and board as parameters</li>

   <li>Ask user to enter the letter of his/her choice in the one of the locations (1-9) on the board

    <ol>

     <li>Where do you like to place your letter (pick in range of 1-9)</li>

     <li>If user repeat the location or pass value outside range (1-9) for placing the letter:</li>

     <li>Send a message:</li>

     <li>Invalid move! Location is already taken. Please try again.</li>

    </ol></li>

   <li>This function will return the board after entering the letter</li>

  </ol></li>

</ol>




<ol start="6">

 <li>checkRows

  <ol>

   <li>takes the board as parameter</li>

   <li>returns True and the letter if a row is filled with the same Letter</li>

  </ol></li>

</ol>




<ol start="7">

 <li>checkCols

  <ol>

   <li>takes the board as parameter</li>

   <li>returns True and the letter if a column is filled with the same Letter</li>

  </ol></li>

</ol>




<ol start="8">

 <li>checkDiags

  <ol>

   <li>takes the board as parameter</li>

   <li>returns True and the letter if any of diagonals are filled with the same Letter</li>

  </ol></li>

</ol>




<ol start="9">

 <li>boardFull

  <ol>

   <li>takes the board as parameter</li>

   <li>returns True if the board is full</li>

  </ol></li>

</ol>




<ol start="10">

 <li>checkWin

  <ol>

   <li>takes the board</li>

   <li>if any of checking (rows, columns, diagonals ) returns True</li>

   <li>announce the winner</li>

   <li>if board is filled and no winner announce draw!</li>

  </ol></li>

</ol>




<ol start="11">

 <li>turnCount</li>

</ol>

Use this function to show, which turns the game is. Example:          It’s Player 2’s (O’ )turn!




<ol>

 <li>takes count of turns</li>

 <li>increment counter</li>

 <li>return counter</li>

</ol>
















<strong>Resources: </strong>

<strong> </strong>

You can download the following files from PolyLearn:

<ul>

 <li>py, at least 2 test cases for each function</li>

 <li>py</li>

 <li>incol (test file for two player)</li>

 <li>inrow (test file for two player)</li>

 <li>india (test file for two player)</li>

</ul>

For testing your program with these files:

python3 tictactoe.py &lt; incol        python3 tictactoe.py &lt; inrow

python3 tictactoe.py &lt; india







<strong>Note:</strong>

You can add any extra functions you need. You have freedom on how you format your messages. Make sure to follow the steps. The sample screenshot is given.

<strong>USE EXACTLY THE SAME FUNCTIONS’ NAME. </strong>




<strong>Submission: </strong>

<ul>

 <li>py (test all your functions- at least two tests for each function)</li>

 <li>py</li>

 <li>py</li>

</ul>




<strong>Rubric: </strong>

<ul>

 <li>py (implement all functions) 5 Points</li>

 <li>py (call all necessary functions) 5 Points</li>

 <li>py (two test for each function) 10 Points</li>

 <li>pass 7 tests                                                 70 Points</li>

 <li>comments                                                 10 Points</li>

</ul>








