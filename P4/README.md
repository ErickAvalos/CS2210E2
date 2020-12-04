4 - Minimus ASCII DElete Sum for Two Strings

    1. To start this problem we first find the ASCII sum of the two given strings. If the sums don't originally add up, we can take the (step A)first sum and substract the value of the first char. Then we recursively call a function with n = 0 which would substract the character at n from the second sum of the second string. We can them compare the two sums and if they add up we can stop, else increment n and compare sums again. If at the end of the first traversion of the second string we don't have a match between sums, we can return to step A but substract the value of the next char.

    2. We need to store the two sums of the given strings in variables.  We also need to temp store the value of the char we are deleting from the sums.

    3. IDEAL
    The problem identified is how to make sure that two strings can have the same ASCCI value if we are able to delete some chars. The goal is to find the two substrings that have the same ASCCI value. A possible strategy is two find all possible substrings and their sums and find the two with the greates matching sum. A possible outcome to anticipate is what if there doesn't exist any two substrings with the same sum.

    DUKE's 7
    The first small instance of this problem is finding the ASCCI sum of the two original strings. It can get tricky trying to traverse the second string while maintaing track of the sum.  A possible pattern would be that the two substrings with the same chars also have the same sum. 