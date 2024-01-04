# Counting Sort Algorithm

Counting Sort is an efficient non-comparison-based sorting algorithm, ideal for sorting integers or objects according to integer keys. It operates by counting the number of objects that have each distinct key value, and using arithmetic to determine the positions of each key value in the output sequence.

## How Counting Sort Works

### Steps in Counting Sort

1. **Determine Range**: Identify the range of input values (usually the maximum value in the input array).

2. **Initialize Count Array**: Set up an auxiliary count array with the size equal to the range of input values, initializing all counts to 0.

3. **Count Occurrences**: For each element in the input array, increment the count in the corresponding index of the count array.

4. **Cumulative Count**: Modify the count array by adding the count of the previous indexes. This step helps in determining the positions of each element in the sorted array.

5. **Create Output Array**: Place each element from the input array into its correct position in the output array, based on the cumulative counts.

6. **Finalize Sorted Array**: If in-place sorting is required, copy the elements from the output array back to the original array.

### Example

Consider the array `[4, 2, 2, 8, 3, 3, 1]`:

- **Find Range**: Maximum value is `8`.
- **Count Array**: Count occurrences of each value from `1` to `8`.
- **Cumulative Count**: Update the count array to be cumulative.
- **Sorting**: Place each item in the correct position using the cumulative counts.

### Characteristics

- **Time Complexity**: O(n + k), where `n` is the number of elements and `k` is the range of input.
- **Space Complexity**: O(k), due to the auxiliary space needed.
- **Stability**: Maintains relative order of equal elements.
- **Non-Comparison Based**: Directly calculates the position of each element.

### Ideal Use Cases

Counting Sort is best used when:
- The range of input values (`k`) is not significantly larger than the number of elements (`n`).
- A stable sort is required.
- The elements are integers or can be mapped to integers.

It's worth noting that Counting Sort is not suitable for data sets where the range (`k`) is very large, as it might lead to large space requirements.

