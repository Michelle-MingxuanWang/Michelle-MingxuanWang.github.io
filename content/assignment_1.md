title: Assignment 1
date: 09/03/2021
author: Mingxuan Wang

Problem1: sum_square_diff
Using a loop to calculate the sum of the squares of the first one hundred natural numbers and use it to minus the square of the sum of the first one hundred natural numbers. 
Then we have the difference between the sum of the squares of the first one hundred natural numbers and the square of the sum.

Problem2: coin_sums
Using nested loops to traverse every possible combination of the coins. 
If the combination can form to an amount of 2 pounds, the count of the combinations adds 1.
In the "if" clause, the equations is "if a*100+b*50+c*20+d*10+e*5+f*2<n+1" because if the total amount is less than 201, the amount can be added to 200 with any number of 1 pence coins.
Moreover, the count of combinations starts from 1 because it includes the case of making 2 pounds with 200 pence.

Problem3: concealed_square
The minimum value of the integer is 1020304050607080900 and the maximum value of the integer is 19293949596979890.
Therefore, let i, which is the number we need to find, starts from the square root of 10^18 to the square root of 2*10^18, which means it starts from 10^9 to the square root of 2*10^9.
Since the last digit of the integer is 0, the stride in the loop is 10.
Calculate the square of i, and using 'if' clause to constrain the value of some digits of the integer:
Use 100 to divide i and calculate the remainder of the result being divided by 10, make the remainder equals to 9. 
Use 10000 to divide i and calculate the remainder of the result being divided by 10, make the remainder equals to 8. 
Similarly, constrains all the values of the digits according to the problem description.
When we find the integer, we can break the loop, and return the unique positive integer that we need to find.

