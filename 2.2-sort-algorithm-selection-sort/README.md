# Selection Sort Algorithm

Selection Sort is a simple and intuitive sorting algorithm. It works by repeatedly finding the minimum element from the unsorted part of the array and moving it to the beginning. This process divides the array into two parts: a sorted subarray and an unsorted subarray. Initially, the sorted subarray is empty and the unsorted subarray is the entire array.

## How It Works

1. **Start with the Full Array**: The entire array is initially unsorted.

2. **Find the Minimum Element**: In each iteration, select the minimum element from the unsorted portion of the array.

3. **Swap with the First Unsorted Element**: Swap this minimum element with the first element of the unsorted part.

4. **Update the Boundary**: After each iteration, the boundary between the sorted and unsorted parts is moved one element to the right.

5. **Repeat Until Sorted**: Continue this process until the entire array is sorted.

### Example

Consider the array `[29, 10, 14, 37, 13]`:

- **First Iteration**:
   - Find the minimum (`10`) and swap with the first element. Array becomes `[10, 29, 14, 37, 13]`.
- **Second Iteration**:
   - Find the minimum (`13`) in the unsorted part and swap with the first unsorted element. Array becomes `[10, 13, 14, 37, 29]`.
- **Continue**:
   - Repeat for each unsorted element.

### Characteristics

- **Time Complexity**: O(n²) for average and worst-case scenarios.
- **Space Complexity**: O(1), as it only requires a single additional memory space.
- **Not Stable**: Does not maintain the relative order of equal elements.
- **In-Place**: Only a constant amount of additional memory space is needed.

### When to Use

Selection Sort is best suited for small datasets due to its higher time complexity. Its simplicity makes it an excellent choice for educational purposes to demonstrate basic sorting algorithms.

