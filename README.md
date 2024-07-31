---
# Just the Run Times and the Reasoning
---
### 1. Arrays
---
```markdown
# Arrays

## Introduction
Arrays are a linear data structure that stores elements in contiguous memory locations. Each element can be accessed directly using its index.

## Time Complexity
- **Access: O(1)**
  - **Reason**: Direct access is possible through the index, which takes constant time regardless of the size of the array.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the array is reached.
- **Insertion: O(n)**
  - **Reason**: Inserting an element requires shifting all subsequent elements one position to the right, which in the worst case, involves moving all n elements.
- **Deletion: O(n)**
  - **Reason**: Deleting an element requires shifting all subsequent elements one position to the left, which in the worst case, involves moving all n elements.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the array.
```
---
### 2. Stacks
---
```markdown
# Stacks

## Introduction
A stack is a linear data structure that follows the Last In, First Out (LIFO) principle. Elements are added to and removed from the same end called the top of the stack.

## Time Complexity
- **Push: O(1)**
  - **Reason**: Adding an element to the top of the stack takes constant time.
- **Pop: O(1)**
  - **Reason**: Removing an element from the top of the stack takes constant time.
- **Peek: O(1)**
  - **Reason**: Accessing the top element of the stack takes constant time.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the stack is reached.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the stack.
```
---
### 3. Queues
---
```markdown
# Queues

## Introduction
A queue is a linear data structure that follows the First In, First Out (FIFO) principle. Elements are added from the rear end and removed from the front end.

## Time Complexity
- **Enqueue: O(1)**
  - **Reason**: Adding an element to the rear of the queue takes constant time.
- **Dequeue: O(1)**
  - **Reason**: Removing an element from the front of the queue takes constant time.
- **Peek: O(1)**
  - **Reason**: Accessing the front element of the queue takes constant time.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the queue is reached.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the queue.
```
---
### 4. Hashing
---
```markdown
# Hashing

## Introduction
Hashing is a technique used to uniquely identify a specific object from a group of similar objects. Hash tables store key-value pairs, where a hash function is used to compute an index into an array of buckets or slots, from which the desired value can be found.

## Time Complexity
- **Insertion: O(1)**
  - **Reason**: Inserting a value into a hash table on average takes constant time, assuming a good hash function and low load factor.
- **Deletion: O(1)**
  - **Reason**: Deleting a value from a hash table on average takes constant time, assuming a good hash function and low load factor.
- **Search: O(1)**
  - **Reason**: Searching for a value in a hash table on average takes constant time, assuming a good hash function and low load factor.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of key-value pairs stored in the hash table.
```
---
### 5. Sliding Window
---
```markdown
# Sliding Window

## Introduction
The sliding window technique is used for problems that involve arrays or lists. This technique helps reduce the time complexity by using a window that slides over the data to avoid redundant computations.

## Time Complexity
- **General: O(n)**
  - **Reason**: The window slides across the array, ensuring each element is processed at most twice, resulting in linear time complexity.

## Space Complexity
- **O(1)**
  - **Reason**: The space required does not scale with the input size; only a fixed number of extra variables are used.
```
---
### 6. Two Pointers
---
```markdown
# Two Pointers

## Introduction
The two-pointers technique is commonly used to solve problems related to arrays and linked lists. It involves using two pointers to iterate through the data structure, often to find pairs or sequences that satisfy certain conditions.

## Time Complexity
- **General: O(n)**
  - **Reason**: Each pointer traverses the array or list, and typically each element is processed at most twice, resulting in linear time complexity.

## Space Complexity
- **O(1)**
  - **Reason**: The space required is constant and does not depend on the input size.
```
---
### 7. Prefix Sum
---
```markdown
# Prefix Sum

## Introduction
Prefix sum is a technique used to preprocess an array of numbers so that queries for the sum of any subarray can be answered quickly. It involves creating a new array where each element at index i is the sum of all elements from the start of the array up to index i.

## Time Complexity
- **Preprocessing: O(n)**
  - **Reason**: Calculating the prefix sums requires a single pass through the array.
- **Query: O(1)**
  - **Reason**: Once the prefix sums are calculated, the sum of any subarray can be found in constant time.

## Space Complexity
- **O(n)**
  - **Reason**: An additional array of the same size as the input array is required to store the prefix sums.
```
---
### 8. Linked Lists
---
```markdown
# Linked Lists

## Introduction
A linked list is a linear data structure where each element (node) contains a value and a reference (link) to the next node in the sequence. There are different types of linked lists such as singly linked lists, doubly linked lists, and circular linked lists.

## Time Complexity
- **Access: O(n)**
  - **Reason**: Accessing an element requires traversing the list from the head node up to the desired node.
- **Search: O(n)**
  - **Reason**: Searching for an element requires traversing the list from the head node up to the node containing the desired value.
- **Insertion: O(1)**
  - **Reason**: Insertion at the head of the list takes constant time. Insertion at any other position requires traversal, making it O(n) in the worst case.
- **Deletion: O(1)**
  - **Reason**: Deletion at the head of the list takes constant time. Deletion at any other position requires traversal, making it O(n) in the worst case.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of nodes in the list.
```
---
### 9. Sorting
---
```markdown
# Sorting

## Introduction
Sorting algorithms are used to rearrange elements in a list or array in a certain order, typically ascending or descending. There are many different sorting algorithms with varying time and space complexities.

## Time Complexity
- **Bubble Sort: O(n^2)**
  - **Reason**: Each element is compared with every other element, resulting in quadratic time complexity.
- **Merge Sort: O(n log n)**
  - **Reason**: The array is recursively divided in half, and each half is sorted and merged, resulting in O(n log n) complexity.
- **Quick Sort: O(n log n) average, O(n^2) worst**
  - **Reason**: The array is partitioned and recursively sorted. In the worst case, the partitioning is unbalanced, resulting in quadratic time complexity.
- **Heap Sort: O(n log n)**
  - **Reason**: Building a heap takes O(n) time, and each of the n elements is extracted in O(log n) time.

## Space Complexity
- **Bubble Sort: O(1)**
  - **Reason**: Sorting is done in place without requiring additional storage.
- **Merge Sort: O(n)**
  - **Reason**: Additional space is required for the temporary arrays used during merging.
- **Quick Sort: O(log n)**
  - **Reason**: Space is required for the recursion stack in the best case.
- **Heap Sort: O(1)**
  - **Reason**: Sorting is done in place without requiring additional storage.
```
---
### 10. Binary Search
---
```markdown
# Binary Search

## Introduction
Binary search is an efficient algorithm for finding an element in a sorted array. It repeatedly divides the search interval in half and compares the target value with the middle element.

## Time Complexity
- **General: O(log n)**
  - **Reason**: The search interval is halved with each step, resulting in logarithmic time complexity.

## Space Complexity
- **O(1)**
  - **Reason**: Binary search is typically implemented iteratively, requiring only a constant amount of extra space.
```
---
### 11. Trees
---
```markdown
# Trees

## Introduction
A tree is a hierarchical data structure consisting of nodes, with a single node designated as the root. Each node may have child nodes, and there are no cycles in the structure.

## Time Complexity
- **Access/Search: O(log n)**
  - **Reason**: For balanced trees, operations such as access and search can be done in logarithmic time.
- **Insertion: O(log n)**
  - **Reason**: For balanced trees, insertion maintains the balance, resulting in logarithmic time complexity.
- **Deletion: O(log n)**
  - **Reason**: For balanced trees, deletion maintains the balance, resulting in logarithmic time complexity.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of nodes in the tree.
```
---
### 12. Heaps
---
```markdown
# Heaps

## Introduction
A heap is a specialized tree-based data structure that satisfies the heap property. In a max heap, for any given node, the value is greater than or equal to the values of its children. In a min heap, the value is less than or equal to the values of its children.

## Time Complexity
- **Access: O(1)**
  - **Reason**: The maximum or minimum element is always at the root of the heap.
- **Insertion: O(log n)**
  - **Reason**: Inserting an element may require adjusting the heap to maintain the heap property, which takes logarithmic time.
- **Deletion: O(log n)**
  - **Reason**: Deleting the root element and adjusting the heap to maintain the heap property takes logarithmic time.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements in the heap.
```
---
### 13. Backtracking
---
```markdown
# Backtracking

## Introduction
Backtracking is a general algorithmic technique for solving problems incrementally by trying partial solutions and then abandoning them if they are not suitable.

## Time Complexity
- **General: O(2^n)**
  - **Reason**: In the worst case, all possible combinations of elements are explored.

## Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the depth of the recursion tree.
```
---
### 14. Graphs
---
```markdown
# Graphs

## Introduction
A graph is a collection of nodes (vertices) and edges connecting pairs of nodes. Graphs can be directed or undirected, and may contain cycles.

## Time Complexity
- **Breadth-First Search (BFS): O(V + E)**
  - **Reason**: Each vertex and each edge is explored once.
- **Depth-First Search (DFS): O(V + E)**
  - **Reason**: Each vertex and each edge is explored once.

## Space Complexity
- **O(V + E)**
  - **Reason**: Space required to store the graph and for the auxiliary data structures used during traversal.
```
---
### 15. Bit Manipulation
---
```markdown
# Bit Manipulation

## Introduction
Bit manipulation involves operations on individual bits of binary numbers. These operations are often used for optimization and low-level programming.

## Time Complexity
- **General: O(1)**
  - **Reason**: Bitwise operations (AND, OR, XOR, NOT, shifts) take constant time.

## Space Complexity
- **O(1)**
  - **Reason**: Bitwise operations do not require additional space.
```
---
### 16. Dynamic Programming (DP)
---
```markdown
# Dynamic Programming (DP)

## Introduction
Dynamic programming is a technique used to solve problems by breaking them down into simpler subproblems and storing the results of these subproblems to avoid redundant computations.

## Time Complexity
- **General: O(n^2)**
  - **Reason**: Problems are often solved using nested loops to fill in a table of subproblem solutions, resulting in quadratic time complexity.

## Space Complexity
- **O(n^2)**
  - **Reason**: Space is required to store the table of subproblem solutions.
```

These templates provide the time complexities, reasons, and space complexities for each data structure and algorithm. You can now create the folders and README files in your GitHub repository following this structure.
