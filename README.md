# ScalaAssignment

## Peer Review 

### Aakash

#### Question 1: Bucketize the array
1. He first formatted the input number to three decimal using f string interpolation.
2. He then multiplied the formatted number with 1000 to convert to an integer, then he took the modulo of that value with 100 to determine the last two digits. He then subtracted this value from the integer value found before.
3. He then compare the last two digit with 49, if it is less than or equal to 49 than the range is set to ```[(first-two-digit)/1000, (first-two-digit+49)/1000]``` else ```[(first-two-digit+50)/1000, (first-two-digit+99)/1000]```.
4. He then prints the range.

<hr>

#### Question 2: Analyze the players
1. He used case class to for player.
2. He stored all the data of the players in a sequence.
3. He used sortby and negate to order the player objects in descending order according to runs in order to find the player with the highest runs. Using take(1), he took the player with the highest run's object, which was the first. The player's name was then printed by him.
4. Same sortby function for renmaining questions.

<hr>

### Ashish

#### Question 1: Bucketize the array
1. He first formatted the input number to 4 decimal places using the format method.
2. The index of the decimal point is found using the ```indexOf``` method, and the number is split into two parts before and after one place after the decimal point using the ```splitAt``` method.
3. If the second part of the split number is less than 0.49, it is set to "00". Otherwise, it is set to "50".
4. The two parts are concatenated, and the resulting string is stored in a variable named ```newNum```. The starting and ending values of the bucket are calculated by converting newNum to a double and adding 0.049 to it.

<hr>

#### Question 2: Analyze the players
1. He used case class to for player.
2. He stored all the data of the players in a sequence.
3. The highest_run_scored function takes an array of Player objects as input and returns the name of the player who scored the highest runs.
4. The top_5_by_runs_scored function takes an array of Player objects as input and prints the names of the top 5 players who scored the highest runs, sorted in descending order.
5. The top_5_by_wickets_taken function takes an array of Player objects as input and prints the names of the top 5 players who took the maximum number of wickets, sorted in descending order.
6. The rank_players_using_wts function takes an array of Player objects as input and ranks the players based on their total score, which is calculated by multiplying their runs by 5 and adding their wickets multiplied by 0.05.

<hr>
