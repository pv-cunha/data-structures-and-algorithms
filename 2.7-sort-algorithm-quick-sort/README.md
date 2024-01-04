# Quick Sort Algorithm

Quick Sort is a highly efficient, comparison-based sorting algorithm that uses the divide-and-conquer principle. It's particularly known for its superior performance with large datasets.

## How Quick Sort Works

### Overview

1. **Divide and Conquer**: Quick Sort partitions the array into two halves, then sorts each half independently.

2. **Pivot Selection**: The algorithm selects a 'pivot' element and moves all elements smaller than the pivot to its left and larger elements to its right.

3. **Partitioning**: The array is rearranged so that elements less than the pivot are on one side, and elements greater than the pivot are on the other.

4. **Recursive Sorting**: Quick Sort is then applied recursively to the two partitions.

5. **Base Case**: The recursion ends when the sub-array has one or no elements.

### Process

1. **Choose a Pivot**: Select an element as the pivot from the array.

2. **Partitioning**: Rearrange the array so that elements less than the pivot are placed before it, and elements greater than the pivot are placed after it.

3. **Apply Recursion**: Recursively apply Quick Sort to the sub-arrays of elements on either side of the pivot.

### Example

Consider the array `[3, 6, 8, 10, 1, 2, 1]`:

- **Select Pivot**: For instance, `6`.
- **Partition**: Arrange the array into `[3, 1, 2, 1, 6, 8, 10]`.
- **Recursive Sort**: Independently sort `[3, 1, 2, 1]` and `[8, 10]`.

### Characteristics

- **Time Complexity**: O(n log n) on average, O(n²) in the worst case.
- **Space Complexity**: O(log n) typically, O(n) in the worst case.
- **Not Stable**: The relative order of equal elements is not maintained.
- **In-Place**: Sorts the array without requiring additional storage space.

### Ideal Use Cases

Quick Sort is ideal for large datasets where its average-case efficiency is beneficial. While it has a higher worst-case complexity, its average performance and space efficiency make it a popular choice in many practical scenarios.

