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
