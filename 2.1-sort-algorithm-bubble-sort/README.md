# Bubble Sort Algorithm

Bubble Sort is a simple sorting algorithm that repeatedly steps through the list to be sorted, compares each pair of adjacent items, and swaps them if they are in the wrong order. The process is repeated until no swaps are needed, indicating that the list is sorted.

## How It Works

1. **Start at the Beginning**: Begin with the first element in the array.

2. **Compare and Swap**:
    - Compare the first two elements.
    - If the first is greater than the second, swap them.

3. **Move Through the Array**:
    - Move to the next pair and repeat the comparison and swap if necessary.
    - Continue this process until the end of the array.

4. **Largest Element at the End**:
    - After the first pass, the largest element will have moved (or 'bubbled up') to the end of the array.

5. **Repeat Minus the Sorted Part**:
    - Repeat the process for the remaining array (excluding the last, sorted element).
    - Each pass can ignore the last sorted element from the previous pass.

6. **Finish When No Swaps Needed**:
    - The algorithm stops when a pass completes without any swaps, meaning the array is sorted.

### Example

Consider the array `[5, 3, 8, 4, 2]`. The sorting process would involve several passes:

- **First Pass**: Compare and swap where necessary, resulting in the largest element (8) at the end.
- **Subsequent Passes**: Repeat, excluding the last sorted elements.

### Characteristics

- **Time Complexity**: O(n²) in average and worst-case scenarios. O(n) in the best-case scenario.
- **Space Complexity**: O(1), as it only requires a single additional memory space.
- **Stability**: Maintains the relative order of equal elements.
- **Adaptivity**: Can be optimized to stop early if no swaps are made in a pass.

Although Bubble Sort is intuitive and easy to implement, it is less efficient for large datasets compared to more advanced sorting algorithms like QuickSort or MergeSort.

