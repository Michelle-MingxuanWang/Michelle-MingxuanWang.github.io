Title: Assignment 2 Description
Date: 09/19/2021
Slug: Assignment 2 Description
Author: Mingxuan Wang
Category: Assignment 2

Write a function called 'pi_expan()'using evalf to convert the input number to to a floating-point approximation with n digits after the decimal point, then multiplies $10^n$, truncate the integer part and convert it to a string.

Then write a function called 'sliding_window()' to generate a list with slinding windows. Using for loops to continuously truncate numbers of length k from the input number, and store the truncated number in the list.

Then write a function called 'is_prime()' to decide whether the number is prime or not:

Using Sieve of Eratosthenes, we can output all the prime numbers under the number we inputted.
The algorithm works as follows:
denote the number we inputted as 'num'. Creating a list of length 'num' to store boolean values represent whether the index of the boolean value is prime or not.
At first, let all the boolean values in the list to be True. Change the boolean values of index '0' and '1' to be False.
Using for loop to enumerate boolean values in the list starts from index 2. If the boolean value is True, change the boolean value of the square of the index i to be false (because the multiple of a prime is not a prime). Loop the list with a constant stride (the index i).
When the loop is finished, using np.nonzero to filter the indexes with a True boolean value in the list. Then the primes under num are outputted.

In the specific question assigned, we need to decide whether the numbers with 10 digits are prime or not. 
Since there are 10000000000 numbers with 10 digits, they are too many to be stored in a list, I outputted the prime numbers under the square root of the number assigned and devided number assigned by all the primes under the square root of it. 
If it is not divisible by all prime numbers under its square root, it is a prime.

Then, write a final function 'find_prime()' to combine the functions. Generating an arbitary large expansion using the 'pi_expan()' function, and use the output as the parameter of the 'sliding_window()' function to generate a list of truncated k digit numbers. Using a for loop to decide whether numbers in the list is prime or not by calling 'is_prime()' function.

For testing the functions, write unique test for all the four functions. Folve the given problem by calling the final function 'find_prime()' with $17\pi$, 100, 10 as the parameters.