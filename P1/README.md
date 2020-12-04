1 - Minimimum Falling Path Sum

1. For this problem we need to traverse the 2d array while forming a new sub array.  We can set i to the index of the first value we grab from the first row. Then
we can grab the values of all the rows with the same index value. This forms one subarray and we can save the sum of it in another variable.  Then we can call the
function again with increased index to grab the next value and restart.  Once we have the sum of the new array, we can decide whether to store it if it's lower than
our previously stored sum.  Then we return the lowest sum.

2. We can store subarrays in a temp array (temp because once we have the sum we can move on to the next one) and store its sum in a variable with the return of the
recursive call as its value.

3. IDEAL
The problem identified is how to divide the array into subarrays. The goal is to find the lowest sum of the subarrays. A possible solution is to manually store
every subarray into its own array. A possible outcome might be that two or more subarrays have the same sum value.

DUKE's 7
A small instance is forming the subarrays.  There is a pattern in what values are stored in the subarray, being only able to go at most one index away from the
previous row. Some test cases to consider were empty arrays or subarrays that have the same sum.  The hardest part to debug is how to make sure to stay in bounds of
the array.
