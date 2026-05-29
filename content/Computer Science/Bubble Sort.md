---
tags:
  - Computer-Science
  - Algorithms
---

# Definition
A sorting algorithm by floating each value to the top into a sorted state.


## Algorithm
```python
# Optimized Python program for implementation of Bubble Sort
def bubbleSort(arr):
    n = len(arr)
    
    # Traverse through all array elements
    # Look at the ith element
    for i in range(n):
        swapped = False

        # Last i elements are already in place
        # The ith element floats to the top until it's in the sorted position
        for j in range(0, n-i-1):

            # Traverse the array from 0 to n-i-1
            # Swap if the element found is greater
            # than the next element
            if arr[j] > arr[j+1]:
                arr[j], arr[j+1] = arr[j+1], arr[j]
                swapped = True
        if (swapped == False):
            break

# Driver code to test above
if __name__ == "__main__":
    arr = [64, 34, 25, 12, 22, 11, 90]

    bubbleSort(arr)

    print("Sorted array:")
    for i in range(len(arr)):
        print("%d" % arr[i], end=" ")
```

The outer loop will look at n items and the inner loop will look at n-i-1 items.
- The time complexity is $O(n^2)$
