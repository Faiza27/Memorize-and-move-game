# Memorize-and-move-game

## Project Idea:
This is a console game where you (player) will need to start from your starting coordinate and need to reach your ending coordinate.
On your way to the ending coordinate you will find obstacles and advantages.

## Features -
The game has three levels - Easy, Medium and Hard.
Obstacles will reduce your point and Advantages will increase your point. 
You can jump over the obstacles also. But only for fixed times.
In this three leveled game, you will have fixed lives and jumps for each level.
You can see your present position anytime, but for each present position state showing you will lose one of your life or if you go out of the bound you will lose one of your life. So, you need to memorize your last position and walk or jump according to that.

## Implementation:
You will choose any level initially for the game from Easy, Medium and Hard level. Each level has a different obstacle and advantage pattern along with a fixed number of lives and jumps. Which is:

Your initial game state will be shown there. 
  You will see a state with signs, where
  -  ‘*’ shown as obstacles 
  -  ‘+’ shown as advantages 
  -  ‘-’ shown as a blank path
  -  ‘s’ shown as starting point or current coordinate
  -  ‘e’ shown as ending point

  Another state will appear with the coordinates, where 
  -  red colored coordinate numbers mean obstacles
  -  green colored coordinate numbers mean advantages
  -  black colored coordinate numbers mean blank path
  -  blue colored coordinate number means starting point or current coordinate
  -  magenta coordinate number means ending point

You need to use your keyboard for moving your avatar from the starting point to end point. There pressing
-  ‘8’ means going up which will be like (x, y+1) from a (x, y) coordinate
-  ‘2’ means going down which will be like (x, y-1) from a (x, y) coordinate
-  ‘4’ means going left which will be like (x-1, y) from a (x, y) coordinate
-  ‘6’ means going right which will be like (x+1, y) from a (x, y) coordinate
-  ‘5x’ means jump where ‘x’ can be replaced with ‘8’, ‘2’, ‘4’ or ‘6’ which will be like (x, y+2), (x, y-2), (x+2, y) or (x+2, y) from a (x, y) coordinate accordingly.

For touching each obstacle 5 points will be reduced and for touching each advantage you 10 points will be added. If your avatar goes ‘out of bound’ anyhow, then for each of this deed one of your lives will be reduced.

For each jump move one of your jumps will be reduced.

The game will end when the number of lives will be zero or when your avatar will reach the end. If your avatar can’t reach the end, then you will lose it otherwise you win it. Your gained points will be shown with the result. 

## Hint:
For printing your present game state you need to write a function named Game_State() which will take your present (x,y) coordinate as parameters and print the output using two other functions named Game_State_Sign() and Game_Sate_Coordinate() which will take the same parameters as the previous function and print the game state with signs and colored coordinates accordingly. 

For moving your avatar you need to write a function named Move() which will take the past (x,y) coordinates and return your present (x,y) coordinates after doing the move. You will need to write a Jump() function which will be called in case of jumping and will take and return the same values as the previous one. 

For calculating the point you need to write a function named Point() which will take your present (x,y) coordinate as parameters and output will be: only when life is 0 or present coordinate matches with ending point show "Game Over"+"You Won" or "You Lost"+ "with x points" or print a message when your avatar touches any obstacle or advantage or none of these or undo your move when your avatar goes out of bound and reduce number of life by one and return a Game_Denoter variable with specific value which will denote if the game will proceed or not.


## Code Structure: 
https://colab.research.google.com/drive/1moY0ONzsRbySryxRYjyteE1y_9Ix5aWj?usp=sharing

## Marking Criteria:
Your submission will be granted as “Pass” if you complete only 30% of this project. If you can complete 60% that would be graded as “Good” and more than it will be considered as “Splendid”.

30% means: The game works for only the “Easy” level.  There’s no life or out of bound condition or obstacles. One can end the game by pressing any specific value.

60% means: The game works for only the “Easy” level. One can’t go out of bound. For each move it will check the coordinate in the move function and you don’t need to reduce the number of lives for this.

## Bonus:
If you think you are a pro, then try this! Generate the Obstacle_list and Advantage_list for each level using a random number generator and then add that to the dictionary.  Then for each time you run the game a new set of obstacles and advantages will appear and you will enjoy the real “Memorize your move” game!!

## Submission Process:
Open your account on github and follow this link to upload your project:
https://docs.github.com/en/enterprise/2.13/user/articles/creating-a-new-repositor
Share the link of your repository in google classroom.




