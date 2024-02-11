# Mersenne-primes
This repo is all about mersenne primes numbers annd contains source code for the primality test for Mersenne numbers.
Mersenne numbers are a class of numbers defined by the formula 2^p - 1, where "p" is a positive integer. The general form is 2^p - 1.
Mersenne numbers are not necessarily prime.
But Mersenne primes are a subset of Mersenne numbers that are also prime. They follow the form 2^p - 1, where both "p" and 2^p - 1 are prime numbers.
Mersenne primes are special because they have unique properties and are of particular interest in number theory.

The lucas_lehmer method is an implementation of the Lucas-Lehmer primality test for Mersenne numbers.
Here's a brief overview of how the Lucas-Lehmer primality test works:

Parameters:
p: This is the exponent in the Mersenne number 2^p - 1 that we want to test for primality.
Initialization:

s is initially set to 4.
m is calculated as 2^p - 1, which is the Mersenne number being tested.

Loop:
The code enters a loop starting from 2 up to p - 1.
In each iteration, s is updated using the Lucas-Lehmer recurrence relation: s = (s^2 - 2) % m.

Check:
After completing the loop, the method checks if the final value of s is equal to 0.

Return:
The method returns True if the final s is 0, indicating that 2^p - 1 is a Mersenne prime. If s is not 0, it returns False, indicating that 2^p - 1 is not a Mersenne prime.
