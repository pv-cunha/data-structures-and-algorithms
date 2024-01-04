# Radix Sort Algorithm

Radix Sort is a unique, non-comparison-based sorting algorithm that sorts integers by processing individual digits. Unlike traditional sorting algorithms, Radix Sort sorts data from the least significant digit to the most significant digit, using Counting Sort or Bucket Sort as a subroutine.

## How Radix Sort Works

### Steps in Radix Sort

1. **Determine Maximum Number**: Find out the maximum number in the array to know the maximum number of digits.

2. **Sorting Each Digit**: Starting from the least significant digit (LSD), sort the numbers using a stable sorting algorithm based on that digit. Repeat this for each subsequent digit, moving towards the most significant digit (MSD).

3. **Using Buckets for Sorting**: In each iteration, place numbers into buckets based on their digit values. After placing all numbers, empty the buckets sequentially and collect the numbers back.

4. **Repeat for Each Digit**: Continue this process for each digit, from the least significant to the most significant.

### Example

Consider an array `[170, 45, 75, 90, 802, 24, 2, 66]`:

- **First Pass (LSD)**: Sort based on units digit, resulting in `[170, 90, 802, 24, 45, 75, 66, 2]`.
- **Second Pass**: Sort based on tens digit, leading to `[802, 2, 24, 45, 66, 170, 75, 90]`.
- **Third Pass (MSD)**: Sort based on hundreds digit to get the final sorted array `[2, 24, 45, 66, 75, 90, 170, 802]`.

### Characteristics

- **Time Complexity**: O(d(n+k)), where `d` is the number of digits, `n` is the number of elements, and `k` is the range of input.
- **Space Complexity**: O(n + k), owing to the use of additional storage.
- **Non-Comparison Based**: It groups elements by digit rather than directly comparing elements.
- **Efficiency**: Most effective when the range of input numbers is not significantly larger than the number of items to sort.

### Ideal Use Cases

Radix Sort is ideal for:
- Large datasets where keys are integers or can be represented as integers.
- Situations where the range of data is not much larger than the number of items.

It's not well-suited for sorting data that cannot be represented as integers or where the range of data values is significantly larger than the number of items to be sorted.

