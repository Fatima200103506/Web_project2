# Java Projects: Tasks 1–5

Hi!I am KIKBAY BIBI FATIMA,and as part of Modules 1 to 6,I implemented 5 core data structure and algorithm tasks in Java. Each task demonstrates fundamental concepts like trees, heaps, queues, and sorting algorithms. Below, I explain what I did for each task, how to run the code, and what test cases I used to verify correctness.

Task 1: Percolation System Simulator
File: PercolationSimulator.java
I built a percolation simulation using the Union-Find data structure with Weighted Quick Union and Path Compression. The system checks whether a path exists between the top and bottom of an n x n grid through open cells.
What I implemented:
Class Percolation with methods: open(row, col), isOpen(), percolates().
Internally used a union-find array to track connected open sites.
Simulated vertical and random site openings.
Test Cases:
Open vertical line in column 0 should percolate.
Randomly open sites test percolates() before and after.
Check isOpen() returns correct results.
Open corner cells to verify index bounds.
Tested on 3×3 and 5×5 grids.


Task 2: Deque and RandomizedQueue
File: Task2Structures.java
I implemented two generic data structures:
A Deque (double-ended queue)
A RandomizedQueue (returns random items in constant amortized time)
What I implemented:
addFirst(), addLast(), removeFirst(), removeLast() in Deque.
enqueue() and dequeue() in RandomizedQueue.
Custom iterators for both structures.
Test Cases:
Insert/remove from both ends in Deque order is correct.
Enqueue multiple items dequeue returns random one.
Check iterator correctness.
Exception handling when removing from empty structures.
Interleaved operations (add/remove) to verify stability.



Task 3: Student Sorting (MergeSort + QuickSort)
File: StudentSorter.java
I created a Student class and implemented both MergeSort and QuickSort to sort students in descending GPA order.
What I implemented:
Student class with name and GPA.
Both sorting algorithms from scratch (no Collections.sort()).
Compared execution time on large input.
Test Cases:
Created 100,000 students with random GPAs.
Verified top 5 students have highest GPA.
Measured and compared MergeSort vs QuickSort runtime.
Verified correctness using Java’s built-in sort.
Tested sorting with students having equal GPAs.




Task 4: Median Finder Using Priority Queues
File: MedianFinder.java
I built a data structure that maintains the median of a stream of numbers using two heaps.
What I implemented:
A max-heap for the lower half, and a min-heap for the upper half.
Methods: insert(double num) and getMedian().
Supports floating-point values and maintains balance between heaps.
Test Cases:
Inserted numbers [5,15,1,3] step-by-step checked median each time.
Inserted 4.5 and 100.1 → confirmed floating-point median.
Tested with ascending and descending sequences.
Validated performance with large input.
Checked edge case with just one number.





Task 5: Symbol Table with Binary Search Tree
File: SymbolTableBST.java
I implemented a Binary Search Tree (BST) that behaves as a symbol table, supporting operations like insertion, search, deletion, and rank-based queries.
What I implemented:
Methods: put, get, delete, min, max, floor, ceiling, rank, select.
Used generics: Key extends Comparable<Key>, Value.
Compared output with Java’s built-in TreeMap.
Test Cases:
Inserted 100 random keys → printed keys in sorted (in-order) order.
Tested rank(k) and checked that select(rank(k)) == k.
Verified min() and max() match TreeMap.
Used floor() and ceiling() with various edge keys.
Deleted a key → checked get() returns null and size reduced.


 
