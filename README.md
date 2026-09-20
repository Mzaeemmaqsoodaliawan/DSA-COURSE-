DSA Lab 01 Problems

This repository contains the Python solutions for DSA Lab 01.
The problems focus on array searching, finding minimum elements,
selection sort, and string slicing.

Problems Included

1. Search an Element in an Array

Given the array:

X = [22, 2, 1, 7, 11, 13, 5, 2, 9]

SearchA(Arr, x) searches the complete array and returns all indices
where x is found.

Example:

Input: 2
Output: Index: 1, 7

Approach: Check every element of the array.

Time Complexity: O(n)

2. Search in a Sorted Array

The same searching problem is considered when the input array is sorted.

SearchB(Arr, x) uses the sorted order to stop searching when an
element greater than x is reached. Original indices are kept so that
the result can still be reported as:

Input: 2
Output: Index: 1, 7

Approach: Sort the values while keeping their original indices, then
stop once the value becomes greater than x.

Time Complexity: O(n log n) for sorting, followed by O(n)
scanning.

3. Find the Minimum Element Index

The function:

Minimum(Arr, starting, ending)

returns the index of the minimum element between the given starting
and ending indices.

Example:

Arr = [3, 4, 7, 8, 0, 1, 23, -2, -5]
starting = 4
ending = 7

The relevant portion is:

Index:  4   5   6   7
Value:  0   1  23  -2

Output:

7

Approach: Start with the first index as the minimum and compare it
with the remaining elements.

Time Complexity: O(n) for the selected range.

4. Sort an Array Using Minimum()

Sort4(Arr) sorts an array by repeatedly finding the minimum element
from the unsorted part and placing it at the beginning.

This is the basic idea of Selection Sort.

Example:

X = [35, 1, 100, -4, 101, 0, 4, -5, 1, -3]

Output:

X = [-5, -4, -3, 0, 1, 1, 4, 35, 100, 101]

Approach:

Find the minimum element in the unsorted part.

Swap it with the first element of that part.

Move to the next position.

Repeat until the array is sorted.

Time Complexity: O(n²)

5. Reverse a Portion of a String

Given:

s = "University of Engineering and Technology Lahore"

StringReverse(str, starting, ending) extracts the required portion and
returns it in reverse order.

The solution must use no loop and no reverse() method.

Example:

Starting Index: 27
Ending Index: 40

Output:
ygolonhceT dn

Approach: Python string slicing is used:

str[starting:ending][::-1]

Time Complexity: O(k), where k is the length of the selected
portion.

Concepts Used

Python functions

Arrays / lists

Linear search

Searching in sorted data

Array indices

Minimum element search

Selection sort

Swapping elements

String slicing

Reverse slicing using [::-1]

Technologies

Python 3

Visual Studio Code

Git & GitHub

How to Run

Clone the repository.

Open the project folder in VS Code.

Make sure Python 3 is installed.

Run the required Python file:

python problem01.py

Change the filename according to the problem you want to run.

Author

Muhammad Zaeem

BS Computer Science Student
University of Engineering and Technology (UET), Lahore
