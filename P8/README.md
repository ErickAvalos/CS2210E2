8 - Perfect Squares

    1. For this problem we first need to ddtermine which numbers are perfect squares.  This can be determined with by multiplying a variable times itself and storing it, then increment the variable (e.g., x = 2, x * x = 4, store 4, increment x).  Then we can perform modolus operation on the given integer n with a predetermined perfect square value. If the result is 0, we can then determine how many of this square number it takes to add up to n by dividing n by the perfect square. Repeat the process with the following square number.

    2. We need to store the perfect square numbers in an array (we store the numbers that are <= n). We also need to store the result of the divison in a variable and change it everytime the result is lower 
    (e.g., n = 100, 100/4 = 25, it would take 25 fours to add up to n.  But then 100/25 = 4, we can replace 25 with 4).

    3. IDEAL
    The problem we need to solve is how to determine how many repetitions of a perfect square number it takes to add up to our given n value.  The goal is to find the lowest possible amount of perfect squares that add up to n. It is possible to anticipate a given n which might not have a sum of perfect squares, such as n = 13.

    DUKE's 7
    A small instance of this problem is to determine how high the number of perfect squares we need to store in the array (we don't need to store perfect squares greater than n). I think it can be tricky which perfect square value takes less amounts to add up to n.  Some test cases to test would be n = 0 or even negative numbers.


