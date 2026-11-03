# Task 1: Sorting Algorithms

*Module:* KH5002CMD Advanced Algorithms
*Language:* C++

## Description
This project implements three comparison-based sorting algorithms in C++: Bubble Sort, Selection Sort and Insertion Sort. Each function sorts an integer array in place and increments a counter once for every comparison between two elements, so the running behaviour of each algorithm can be measured on different inputs.

## Files
| File | Purpose |
|---|---|
| sorting_algorithms.h | SortAnalyser class with bubbleSort, selectionSort and insertionSort |
| main.cpp | Test driver: helper functions and the seven test cases (TC1 to TC7) |

## Build and run

g++ -std=c++17 main.cpp -o sorting
./sorting

On Windows, run sorting.exe instead of ./sorting.

## Test cases
The driver sorts a 10-element array and counts comparisons for each algorithm on random, already-sorted and reverse-sorted input.

| Test | Algorithm | Input | Comparisons |
|---|---|---|---|
| TC1 | Bubble Sort | Random | 45 |
| TC2 | Selection Sort | Random | 45 |
| TC3 | Insertion Sort | Random | 29 |
| TC4 | Bubble Sort | Sorted | 45 |
| TC5 | Insertion Sort | Sorted | 9 |
| TC6 | Bubble Sort | Reverse sorted | 45 |
| TC7 | Insertion Sort | Reverse sorted | 45 |

## Time complexity
| Algorithm | Best | Average | Worst | Extra space |
|---|---|---|---|---|
| Bubble Sort | O(n²) | O(n²) | O(n²) | O(1) |
| Selection Sort | O(n²) | O(n²) | O(n²) | O(1) |
| Insertion Sort | O(n) | O(n²) | O(n²) | O(1) |

The bubble sort used here has no early-exit check, so it always makes n(n-1)/2 comparisons (45 for n = 10).
