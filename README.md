# stones
Language: Python

Created a game of 16 stones with a two player and AI mode. Player take turns taking 1-4 stones each. Player with 1 stone left loses.

Displays the stones in a grid that is the ceiling value of square root by square root of remaining stones. 

AI takes the optimal amount of stones to win, else takes 1 stone to maximize player error. AI always wins if going second. 
Created strategy by finding losing states (1, 6, 11, 16) based on the remainder of total stones mod max (4) plus min (1) stones that can be taken. 
Because that number is 5, (numbers divisible by 5) + 1 are losing states because no matter what the player takes, 
the AI can take a number to make the remainder 1 (the ultimate losing state).
