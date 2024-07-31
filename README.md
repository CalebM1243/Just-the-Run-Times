# Data Structures and Algorithms Complexity
---

1. [Arrays](#arrays)
2. [Stacks](#stacks)
3. [Queues](#queues)
4. [Hashing](#hashing)
5. [Sliding Window](#sliding-window)
6. [Two Pointers](#two-pointers)
7. [Prefix Sum](#prefix-sum)
8. [Linked Lists](#linked-lists)
9. [Sorting](#sorting)
10. [Binary Search](#binary-search)
11. [Trees](#trees)
12. [Heaps](#heaps)
13. [Backtracking](#backtracking)
14. [Graphs](#graphs)
15. [Bit Manipulation](#bit-manipulation)
16. [Dynamic Programming (DP)](#dynamic-programming-dp)

---
## Arrays
---
### Time Complexity
- **Access: O(1)**
  - **Reason**: Direct access is possible through the index, which takes constant time regardless of the size of the array.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the array is reached.
- **Insertion: O(n)**
  - **Reason**: Inserting an element requires shifting all subsequent elements one position to the right, which in the worst case, involves moving all n elements.
- **Deletion: O(n)**
  - **Reason**: Deleting an element requires shifting all subsequent elements one position to the left, which in the worst case, involves moving all n elements.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the array.

---
## Stacks
---
### Time Complexity
- **Push: O(1)**
  - **Reason**: Adding an element to the top of the stack takes constant time.
- **Pop: O(1)**
  - **Reason**: Removing an element from the top of the stack takes constant time.
- **Peek: O(1)**
  - **Reason**: Accessing the top element of the stack takes constant time.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the stack is reached.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the stack.

---
## Queues
---
### Time Complexity
- **Enqueue: O(1)**
  - **Reason**: Adding an element to the rear of the queue takes constant time.
- **Dequeue: O(1)**
  - **Reason**: Removing an element from the front of the queue takes constant time.
- **Peek: O(1)**
  - **Reason**: Accessing the front element of the queue takes constant time.
- **Search: O(n)**
  - **Reason**: In the worst case, every element might need to be checked until the desired element is found or the end of the queue is reached.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements stored in the queue.

---
## Hashing
---
### Time Complexity
- **Insertion: O(1)**
  - **Reason**: Inserting a value into a hash table on average takes constant time, assuming a good hash function and low load factor.
- **Deletion: O(1)**
  - **Reason**: Deleting a value from a hash table on average takes constant time, assuming a good hash function and low load factor.
- **Search: O(1)**
  - **Reason**: Searching for a value in a hash table on average takes constant time, assuming a good hash function and low load factor.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of key-value pairs stored in the hash table.

---
## Sliding Window
---
### Time Complexity
- **General: O(n)**
  - **Reason**: The window slides across the array, ensuring each element is processed at most twice, resulting in linear time complexity.

### Space Complexity
- **O(1)**
  - **Reason**: The space required does not scale with the input size; only a fixed number of extra variables are used.

---
## Two Pointers
---
### Time Complexity
- **General: O(n)**
  - **Reason**: Each pointer traverses the array or list, and typically each element is processed at most twice, resulting in linear time complexity.

### Space Complexity
- **O(1)**
  - **Reason**: The space required is constant and does not depend on the input size.

---
## Prefix Sum
---
### Time Complexity
- **Preprocessing: O(n)**
  - **Reason**: Calculating the prefix sums requires a single pass through the array.
- **Query: O(1)**
  - **Reason**: Once the prefix sums are calculated, the sum of any subarray can be found in constant time.

### Space Complexity
- **O(n)**
  - **Reason**: An additional array of the same size as the input array is required to store the prefix sums.

---
## Linked Lists
---
### Time Complexity
- **Access: O(n)**
  - **Reason**: Accessing an element requires traversing the list from the head node up to the desired node.
- **Search: O(n)**
  - **Reason**: Searching for an element requires traversing the list from the head node up to the node containing the desired value.
- **Insertion: O(1)**
  - **Reason**: Insertion at the head of the list takes constant time. Insertion at any other position requires traversal, making it O(n) in the worst case.
- **Deletion: O(1)**
  - **Reason**: Deletion at the head of the list takes constant time. Deletion at any other position requires traversal, making it O(n) in the worst case.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of nodes in the list.

---
## Sorting
---
### Time Complexity
- **Bubble Sort: O(n^2)**
  - **Reason**: Each element is compared with every other element, resulting in quadratic time complexity.
- **Merge Sort: O(n log n)**
  - **Reason**: The array is recursively divided in half, and each half is sorted and merged, resulting in O(n log n) complexity.
- **Quick Sort: O(n log n) average, O(n^2) worst**
  - **Reason**: The array is partitioned and recursively sorted. In the worst case, the partitioning is unbalanced, resulting in quadratic time complexity.
- **Heap Sort: O(n log n)**
  - **Reason**: Building a heap takes O(n) time, and each of the n elements is extracted in O(log n) time.

### Space Complexity
- **Bubble Sort: O(1)**
  - **Reason**: Sorting is done in place without requiring additional storage.
- **Merge Sort: O(n)**
  - **Reason**: Additional space is required for the temporary arrays used during merging.
- **Quick Sort: O(log n)**
  - **Reason**: Space is required for the recursion stack in the best case.
- **Heap Sort: O(1)**
  - **Reason**: Sorting is done in place without requiring additional storage.

---
## Binary Search
---
### Time Complexity
- **General: O(log n)**
  - **Reason**: The search interval is halved with each step, resulting in logarithmic time complexity.

### Space Complexity
- **O(1)**
  - **Reason**: Binary search is typically implemented iteratively, requiring only a constant amount of extra space.

---
## Trees
---
### Time Complexity
- **Access/Search: O(log n)**
  - **Reason**: For balanced trees, operations such as access and search can be done in logarithmic time.
- **Insertion: O(log n)**
  - **Reason**: For balanced trees, insertion maintains the balance, resulting in logarithmic time complexity.
- **Deletion: O(log n)**
  - **Reason**: For balanced trees, deletion maintains the balance, resulting in logarithmic time complexity.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of nodes in the tree.

---
## Heaps
---
### Time Complexity
- **Access: O(1)**
  - **Reason**: The maximum or minimum element is always at the root of the heap.
- **Insertion: O(log n)**
  - **Reason**: Inserting an element may require adjusting the heap to maintain the heap property, which takes logarithmic time.
- **Deletion: O(log n)**
  - **Reason**: Deleting the root element and adjusting the heap to maintain the heap property takes logarithmic time.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the number of elements in the heap.

---
## Backtracking
---
### Time Complexity
- **General: O(2^n)**
  - **Reason**: In the worst case, all possible combinations of elements are explored.

### Space Complexity
- **O(n)**
  - **Reason**: Space required is proportional to the depth of the recursion tree.

---
## Graphs
---
###

 Time Complexity
- **Breadth-First Search (BFS): O(V + E)**
  - **Reason**: Each vertex and each edge is explored once.
- **Depth-First Search (DFS): O(V + E)**
  - **Reason**: Each vertex and each edge is explored once.

### Space Complexity
- **O(V + E)**
  - **Reason**: Space required to store the graph and for the auxiliary data structures used during traversal.

---

## Bit Manipulation

### Time Complexity
- **General: O(1)**
  - **Reason**: Bitwise operations (AND, OR, XOR, NOT, shifts) take constant time.

### Space Complexity
- **O(1)**
  - **Reason**: Bitwise operations do not require additional space.

---
## Dynamic Programming (DP)
---
### Time Complexity
- **General: O(n^2)**
  - **Reason**: Problems are often solved using nested loops to fill in a table of subproblem solutions, resulting in quadratic time complexity.

### Space Complexity
- **O(n^2)**
  - **Reason**: Space is required to store the table of subproblem solutions.
