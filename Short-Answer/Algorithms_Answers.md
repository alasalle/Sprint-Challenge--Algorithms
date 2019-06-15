Add your answers to the Algorithms exercises here.
## Exercise I

a) The time complexity of this snippet is O(n) because the amount of times the while loop will run is directly proportional to the size of n.

b) O(n * (n-1) * (n-2) * 10) = O(n^3)

c) The time complexity of this snippet is o(n) because the recursion will run as many times as there are bunnies.

## Exercise II

I think the optimal strategy to minimize dropped eggs in this problem would be a binary search. The time complexity of a binary search is O(log n).

1. Create list of floors composed of a range up to _n_.
2. Find midpoint of list by adding low point and high point and dividing by 2
3. Separate list into 2 halves, low to mid and mid+1 to high
4. Drop egg from midpoint and check if it broke
5. If it did, repeat steps 2 - 5 on the low to mid list. If not, repeat steps 2 - 5 on the mid + 1 to high list.
6. Once you find the floor where it does break but it didn't on the floor before it, you've found _f_.