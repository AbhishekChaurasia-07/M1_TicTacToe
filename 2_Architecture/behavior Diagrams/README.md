# TIC-TAC-TOE GAME DESIGN

When a player makes a move, we need to check if he/she wins the game. A simple solution is to check O(N^2) grid for horizontal, vertical and two diagonals to see if they are all occupied by this player. However, a better solution that has O(1) time would be to trade space for time. That is, we use O(N) space to record the number of each players in each row, column and two diagonals.


![image](https://user-images.githubusercontent.com/101011183/160985644-f86e64ff-a1b8-41b1-a75c-0c4530723ec4.png)

# Tic-Tac-Toe Frame

The TicTacToeFrame (shown in figure 4.2.2) has a menu bar, the BoardPanel, and can open the three dialogs. The final static String values contain the file locations of the help and about HTML files respectively. This class extends java.swing.JFrame.

The getBoard method returns the board variable. The update repaints and performs any necessary update functions to make sure the view represents the current GameState. The openNewGameDialog, openHelpDialog, and openAboutDialog methods open the respective dialogs. The announceEnd announces the end of a game and displays Player p as the winner; if p is null, then this method announces a tie. The askPlayAgain method prompts the user to play again and returns their choice (true for yes).

![image](https://user-images.githubusercontent.com/101011183/160985878-32eb43b8-6efc-46c5-a577-d3232d6b7f74.png)

# The Game theory

The game of Noughts and Crosses or Tic Tac Toe is well known throughout the world and variants are thought to have been played over 2000 years ago in Rome. It’s a very simple game – the first person to get 3 in a row wins. In fact it’s so simple that it has been “solved” – before any move has been played we already know it should result in a draw (as long as the participants play optimal moves).The way to solve Noughts and Crosses is to use combinatorial Game Theory – which is a branch of mathematics that allows us to analyses all different outcomes of an event.

![image](https://user-images.githubusercontent.com/101011183/160985960-270b9c47-6ca8-4d89-ae74-6e2093329add.png)

This is the start of the game tree for Noughts and Crosses. We can expand this game tree to cover every possible outcome for the game. Once this complete tree is drawn, any participant can work through this tree to see what is their optimal move at any one time from any position.An upper bound for the number of positions and number of different games is given by:3 9= 19,683. This is the total number of possible game positions in a 3×3 grid – as every square will either be a O, X or blank.9! = 362,880. This is the total number of ways that positions can be filled on the grid.
# ARCHITECTURE

![image](https://user-images.githubusercontent.com/101011183/160986033-a00ae819-7d45-45c1-87a4-fce743865880.png)
