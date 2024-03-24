# Natural Merge Sort

This repository contains a C++ implementation of Natural Merge Sort. Natural Merge Sort is a variation of Merge Sort that takes advantage of pre-existing order in the input array to achieve better performance.

## Overview

The program takes an array of integers as input and sorts it using Natural Merge Sort. Natural Merge Sort is an efficient sorting algorithm that divides the input array into multiple sorted subarrays, then merges them to produce the final sorted array. It utilizes the natural order present in the array to identify sorted subsequences, resulting in improved performance for nearly sorted arrays.

## Implementation Details

### `merge` Function

The `merge` function is responsible for merging two sorted subarrays into a single sorted array. It takes four parameters:
- `arr[]`: The input array
- `start`: The starting index of the first subarray
- `mid`: The ending index of the first subarray
- `end`: The ending index of the second subarray

### `naturalSort` Function

The `naturalSort` function implements the Natural Merge Sort algorithm. It identifies sorted subsequences in the input array and merges them using the `merge` function. This process continues until the entire array is sorted.

### `printSort` Function

The `printSort` function is used to print the sorted array after sorting is complete.

## Usage

To use the program, follow these steps:
1. Compile the program using a C++ compiler.
2. Run the compiled executable.
3. Enter the size of the array followed by the elements of the array.
4. The program will output the sorted array.

## Example

```bash
$ g++ -o natural_merge_sort natural_merge_sort.cpp
$ ./natural_merge_sort
5
4 2 7 1 3
Output:
1 2 3 4 7
```

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
