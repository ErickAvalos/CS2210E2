2 - Palindromic Substrings

    1. First we need to break down the original string by characters.  We count how many characters and add the count to total count. Recursively, we want to be
    able to keep track of the total number of palindromes that meet our conditions by forming every substring possible and checking it agains our conditions.

    2. We can start forming a new string by combining the characters.  As long as the new string is still palindrome, we can continue and add +1 to the count
    everytime.  Once we find a non palindrome, we can move on to the next character and start the process over again.

    3. IDEAL
    The problem is whether or not a substring should count as palindrome. The ultimate goal is to count how many palindrome substrings exist in a given string. A
    possible strategy is two form two strings out of the chars and compare them against each other.
    One anticipated outcome is what if we have an even or odd string.

    DUKE's 7
    One small instance of the problem is breaking down a string to individual characters. One tricky part is how to decide if a substring is palindrome. But
    determining patterns can help with this issue by seeing if the characters repeat in order. 
