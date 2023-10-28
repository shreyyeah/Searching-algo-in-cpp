# Linear-search-and-binary-search-in-cpp
Linear search and binary search are two common searching algorithms used to find a specific element within a list or array in C++. 
Linear search-An easy-to-understand searching method is linear search. It repeatedly goes through each element in an array one at a time until it either locates the desired element or runs out of space. For unsorted lists, it works well.

Binary Search- A more effective searching technique is binary search, although it needs the list to be sorted beforehand. Until the target element is located or it is determined that the element is not in the array, it continually splits the sorted array in half and narrows the search space.

Though,Binary search is significantly faster than linear search for large sorted arrays, as it reduces the search space by half in each step. However, it requires the list to be sorted, which may not be suitable for all scenarios.

To work with linear search-
-Start from the first element (index 0) of the array.

-Compare the current element with the target element.

-If they are equal, return the index of the current element.

-If not, move to the next element (increment the index by 1) and repeat steps 2 and 3.

-Continue this process until the target element is found or the end of the array is reached.

-If the end of the array is reached and the target element is not found, return -1 to indicate that the element is not in the array. 

And with binary search:

-Initialize two pointers, left and right, to the first and last indices of the array, respectively.

-Repeat the following steps until left is less than or equal to right:
a. Calculate the middle index mid as (left + right) / 2.
b. Compare the element at index mid with the target element.
c. If they are equal, return mid as the index of the target element.
d. If the element at index mid is less than the target element, update left to mid + 1 to search the right half of the array.
e. If the element at index mid is greater than the target element, update right to mid - 1 to search the left half of the array.

-If the target element is not found after the loop, return -1 to indicate that the element is not in the array.
