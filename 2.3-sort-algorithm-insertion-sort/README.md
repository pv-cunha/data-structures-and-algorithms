# Insertion Sort Algorithm

Insertion Sort is a simple yet efficient algorithm, particularly effective for small datasets or arrays that are already partially sorted. It builds the final sorted array one item at a time.

## How It Works

1. **Begin with the Second Element**: Consider the first element as sorted. Start the sorting process from the second element.

2. **Select an Element to Insert**: In each iteration, pick an element from the unsorted part of the array.

3. **Find the Correct Position**: Compare this element with the elements in the sorted part. Move backwards, shifting each element that is greater than the selected element to the right. This makes space for the new element to be inserted.

4. **Insert the Element**: Insert the element at its correct position where all elements to the left are smaller and all to the right are greater.

5. **Repeat for All Elements**: Continue this process for each element in the unsorted part until the entire array is sorted.

### Example

Consider the array `[8, 4, 3, 7, 6]`:

- **First Iteration**:
  - Select `4` and compare with `8`. Shift `8` right and insert `4`. Array becomes `[4, 8, 3, 7, 6]`.
- **Second Iteration**:
  - Select `3`, shift `8` and `4` right, and insert `3`. Array becomes `[3, 4, 8, 7, 6]`.
- **Continue**:
  - Repeat with the remaining elements.

### Characteristics

- **Time Complexity**: O(n²) in average and worst-case scenarios but efficient for small or nearly sorted datasets.
- **Space Complexity**: O(1), as it requires minimal additional memory space.
- **Stability**: Maintains the relative order of equal elements.
- **Adaptivity**: Highly efficient for datasets that are already partially sorted.

### Usage

Insertion Sort is ideal for small datasets and shines in scenarios where the data is already partially sorted. It's a preferred choice for its simplicity and efficiency in specific cases, despite its quadratic time complexity.

