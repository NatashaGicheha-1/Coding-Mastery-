# 💜📚 Efficiency of Algorithms - Assignments Only

Focus ON:

✅ O(log n) calculations  
✅ O(n) vs O(n log n) comparisons  
✅ O(2ⁿ) calculations  
✅ Bubble Sort tracing  
✅ Insertion Sort tracing  
✅ Merge Sort tracing  
✅ Quick Sort partitioning  
✅ Space Complexity analysis  
✅ DFS traversal and backtracking

---

# 💜 Class Assignment 1 - Logarithmic Time O(log n)

A database system uses logarithmic time to quickly locate a record in a sorted list of user IDs. Assuming the database contains **500 records**:

1. Giving an example of the specific algorithm, explain how this algorithm functions.
2. Write the general formula for the number of steps required by logarithmic time in the worst case.
3. Using the formula above, calculate the number of steps for **500 records**.
4. If the number of records is doubled to **1000**, how many additional steps are required? Show your working.

【1-02fa4b】

---

# 💜 Class Assignment 2 - Linear vs Linearithmic Time

A software company is developing two features for a data processing system that handles **n records**.

- **Feature A** processes records by scanning each record exactly once.
- **Feature B** processes records by repeatedly dividing the data into smaller parts and then combining the results.

Questions:

1. State the time complexity of Feature A and Feature B. Explain.
2. Between the two features, which one is faster as **n** becomes very large? Explain your answer.
3. If the system must handle millions of records in real time, which feature would you recommend and why?
4. Give examples of algorithms used in both Feature A and Feature B.

【1-02fa4b】

---

# 💜 Class Assignment 3 - Exponential Time O(2ⁿ)

A cybersecurity system uses a brute-force algorithm to crack a password.

The algorithm tries all possible combinations, and for every additional character added to the password, the number of possible combinations doubles.

Assume the number of steps grows as **2ⁿ**, where **n** is the password length.

### Questions

a) Write the time complexity of this algorithm.

b) Calculate the number of steps required when:

- i) n = 5
- ii) n = 10

c) Explain why this algorithm becomes impractical as **n** increases.

d) Suggest one real-world situation where such an exponential-time algorithm might still be acceptable.

【1-02fa4b】

---

# 💜 Class Assignment 5 - Bubble Sort

Bubble Sort is a simple comparison-based sorting algorithm where adjacent elements are repeatedly compared and swapped if they are in the wrong order.

Given the array:

```text
A = 7 3 8 2 5
```

### Questions

a) Using the Bubble Sort algorithm, show the array after each comparison and swap during the **first two passes only**.

b) Explain why Bubble Sort is said to be an **in-place sorting algorithm**.

c) State the **space complexity** of Bubble Sort. Explain.

【1-02fa4b】

---

# 💜 Class Assignment 6 - Insertion Sort

Insertion Sort works like sorting cards in your hand. You take one element at a time and insert it into its correct position in the already sorted part of the array.

Given:

```text
A = [6, 4, 9, 3, 7]
```

### Questions

1. Using the Insertion Sort algorithm, show the state of the array after each insertion step (starting from the second element). (6 marks)

2. State and explain the property of the left part of the array at each step of Insertion Sort. (2 marks)

3. Identify the space complexity of Insertion Sort and briefly justify your answer using:
   - Input storage
   - Auxiliary variables

(2 marks)

【1-02fa4b】

---

# 💜 Class Assignment 7 - Merge Sort

A school maintains a list of student roll numbers that must be displayed in ascending order on the notice board.

Initial list:

```text
[5, 2, 9, 1]
```

The school decides to use Merge Sort.

### Questions

1. Explain how Merge Sort applies the divide-and-conquer strategy to sort the given list.
2. Show all divide steps until each subarray contains only one element.
3. Perform the merge steps, showing how the subarrays are combined in sorted order at each stage.
4. What is the final sorted array?
5. Analyze the space complexity of Merge Sort by clearly explaining:
   - Input storage
   - Auxiliary (temporary) space
   - Recursive stack space
6. Why might Merge Sort be preferred over Bubble Sort or Insertion Sort for a large number of student records even though it uses more memory?

【1-02fa4b】

---

# 💜 Assignment 8 - Quick Sort

Quick Sort is a divide-and-conquer sorting algorithm.

Consider the array:

```text
A = [8, 3, 6, 2, 7, 5, 4]
```

Assumptions:

- The last element is always chosen as the pivot.
- The algorithm uses in-place partitioning.

### a) First Partition (4 Marks)

1. Identify the pivot in the first call.
2. Show the array after the first partition.
3. Indicate the final position of the pivot after partitioning.

### b) Recursive Calls (4 Marks)

Using the result from part (a):

1. Write down the left subarray and the right subarray.
2. Perform one more partition on each subarray.
3. Show the array after each partition step.

### c) Space Complexity (2 Marks)

Explain the space complexity of Quick Sort by discussing:

- Input storage
- Auxiliary variables
- Recursive stack space

【1-02fa4b】

---

# 🌸 Self-Reading Assignment 1 - Quadratic Time O(n²)

A school is testing the performance of its computer system when handling pairs of students for group assignments.

Each student must be paired with every other student (including themselves).

Assume there are **n students**.

### Questions

1. Write a Java program using two for loops to print all possible pairs of students in the format:

```text
i, j
```

where **i** and **j** represent student numbers from **0 to n−1**.

2. If **n = 5**, write down how many times the inner print statement will execute.

3. Explain why this algorithm has Quadratic Time Complexity **O(n²)**.

【1-02fa4b】

---

# 🌸 Self-Reading Assignment 2 - Depth First Search (DFS)

A school has a computer network where each computer is connected as shown below:

```text
    A
   / \
  B   C
 / \   \
D   E   F
```

The network administrator wants to test the system by visiting each computer using the **Depth-First Search (DFS)** method, starting from computer **A**.

### Questions

1. Using the DFS technique, list the order in which the computers will be visited, starting from node A.
2. Explain briefly what is meant by **backtracking** in DFS.

【1-02fa4b】

---



> 💜 **天道酬勤**
>
> *Tiān dào chóu qín*
>
> "Heaven rewards hard work."

Source: SLIDE 9 EFFICIENCY OF ALGORITHM.pptx. 【1-02fa4b】


---------
# 💜📚 Efficiency of Algorithms 
1. A database system uses logarithmic time to quickly locate a record in a sorted list of user IDs. Assuming the
database contains 500 records,
a) Giving an example of the specific algorithm, Explain how this algorithm functions
b) Write the general formula for the number of steps required by logarithmic time in the worst case.
c) Using the formula in above calculate the number of steps for 500 records
d) If the number of records is doubled to 1000, how many additional steps are required? Show your
working.

2. A software company is developing two features for a data processing system that handles n
records. Feature A processes the records by scanning each record exactly once while Feature B
processes the records by repeatedly dividing the data into smaller parts and then combining the
results.
a) State the time complexity of feature A and feature Explain.
b) Between the two features, which one is faster as n becomes very large? Explain your answer
c) If the system must handle millions of records in real time, which feature would you
recommend and why?
d) Give examples of these algorithms in both feature A and B

3. A school is testing the performance of its computer system when handling pairs of students for group
assignments. Each student must be paired with every other student (including themselves) so that the
system can display all possible combinations. Assume there are n students in the class.
a) Write a Java program using two for loops to print all possible pairs of students in the format: i, j where
i and j represent student numbers from 0 to n-1.
b) If n = 5, write down how many times the inner print statement will execute.
c) Explain why this algorithm has Quadratic Time Complexity O(n²).

4. A cybersecurity system uses a brute-force algorithm to crack a password. The algorithm tries all possible
combinations, and for every additional character added to the password, the number of possible combinations
doubles. Assumeing that when the algorithm performs 1 step per password combination, the number of steps grows
as 2ⁿ, where n is the password length
a) Write the time complexity of this algorithm.
b) Calculate the number of steps required when:
i) n = 5
ii) n = 10
c) Explain why this algorithm becomes impractical as n increases.
d) Suggest one real-world situation where such an exponential-time algorithm might still be acceptable
