# algorithmic-efficiency-optimisation
Keyboard path optimisation algorithm.


Algorithmic Efficiency Optimisation System


Overview

This project develops an algorithmic solution to determine the minimum sequence of operations required to type a given string across multiple keyboard configurations.
The program evaluates alternative input strategies and dynamically selects the most efficient path to minimise total operations.


Comparative evaluation of multiple keyboard layouts
-Decision-making logic to optimise operation count
-Algorithmic minimisation of user actions
-Performance-focused structured implementation


Programming Language Used: Python


Learning Outcomes

This project enhanced my ability to design optimisation algorithms, analyse performance trade-offs, and implement structured decision-making logic.

-------------------------------------------------------------------------------------------
-------------------------------------------------------------------------------------------

Steps followed for this project in detail:

This program asks the user to input a string, and then the robot will choose a keyboard and plan its own actions to type the string using the selected keyboard. 


The robot starts at the top left position (a) and can take the following actions:

u - go up
d - go down
l - go left
r - go right
p - press the key


After pressing a key, the robot stays on that key. This means:

-it can immediately press the same key again
-to go to another key, the robot will start from the last key it moved to.

Furthermore, the robot will always move horizontally (left/right) before moving vertically (up/down) when moving to a key it needs to press.


For a given input string:

- If there is a single keyboard on which in can be typed, then Robbie picks that one.
- If it can be typed on multiple keyboards, the robot picks a single keyboard as follows:
---- The one that requires the fewest moves, or, if there is a tie, 
---- The first best keyboard configuration (in the order they are given).
- Finally, there may not be a keyboard that can type that string.



