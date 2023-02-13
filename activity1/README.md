# Activities

## Task 1

- Refer to the following link. Discuss how Merge-sort works:
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/mergesortAV.html

Merge-sort will split array as many times as possible and start sorting from there to put back the array in the sorted order

- Merge-sort Practice. Refer to the following link. Merge the two sub-arrays into the larger array.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/MergesortMergePRO.html

  Done

## Task 2

- Refer to the following link. Discuss how Quick-sort works:  
  https://opendsa-server.cs.vt.edu/OpenDSA/AV/Sorting/quicksortAV.html
  Quick-sort works by pivoting array, partitioning it in 2 halfs and sorting. That is repeated untill full array is sorted.


- Quick-sort Practice. Refer to the following link. Partition the array using quicksort.
  https://opendsa-server.cs.vt.edu/OpenDSA/Exercises/Sorting/QuicksortPartitPRO.html

  Done

## Task 3

- The following snippet is from `./src/quicksort.cpp` lines 32-43. Discuss in groups how the code works:

```cpp
void quickSort(int arr[], int low, int high)
{
    if (low < high)
    {
        //partition the array
        int pivot = partition(arr, low, high);

        //sort the sub arrays independently
        quickSort(arr, low, pivot - 1);
        quickSort(arr, pivot + 1, high);
    }
}
```

- The following snippet is from `./src/quicksort.cpp` line 27. Discuss in groups how ìt works:

```cpp
swap(&arr[i + 1], &arr[high]);
```

## Task 4: Individual (at home)

1. Merge-sort has better worst case performance than quicksort. So why Quick-sort is considered better than Merge-sort? Refer to the following article

Quicksort takes less space.
Quicksort worst case can be brought down to Mergesort with selecting pivot by taking average from 3 elements.
Quicksort is better for virtual memory enviroment cause it's locality.


   https://www.geeksforgeeks.org/quicksort-better-mergesort/
2. Refer to the following article. Analyze the complexity of the Merge-sort algorithm.
   https://www.softwaretestinghelp.com/merge-sort/

Merge-sort

Worst case time complexity	O(n*log n)
Best case time complexity	O(n*log n)
Average time complexity	O(n*log n)
Space complexity	O(n)


3. Refer to the following article. Analyze the complexity of the Quick-sort algorithm.
   https://www.softwaretestinghelp.com/quick-sort/

Quick-sort

Worst case time complexity	O(n 2 )
Best case time complexity	O(n*log n)
Average time complexity	O(n*log n)
Space complexity	O(n*log n)
