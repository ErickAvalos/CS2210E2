3 - Arithmetic Slices

    1. For this problem we have to traverse through the given sequence in order. We can call a function and send it the sequence and a variable n, starting with the first index. We then have to check for the diffrence between the values at n and n+1. Once we have the difference of the first two values, we can keep calling the function while incrementing n as long as the condition of the same diffrence is met.

    2. The solution to store is the number of slices in the sequence.  We can do this with a count and increment each time our difference matches the original difference. This can be stored in a variable.

    3. IDEAL
    The problem identified is how to compare the differences between consecutive values. The goal is to check for the diffrence of all the values in the sequence, but we can stop when we find a non match.  The only solution I can see is to first grab the difference of the first two values and then start traversing the whole sequence (as needed) and ensure the difference always stays the same. Possible outcomes to anticipate are sequences with less than three numbers or empty sequences.

    DUKE's 7
    A small instance of this problem is determining the original difference to check for throughout the sequence. The tricky part is how to ensure we stop traversing the array when the differences don't match.
    Two test cases would be to test two different sequences with known results to ensure the correct answer. It can get tricky to debug index out of bounds errors.
