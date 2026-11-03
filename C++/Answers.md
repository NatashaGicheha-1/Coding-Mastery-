# 💜📚 Efficiency of Algorithms - Assignments with Answers

> 🌸 **学海无涯苦作舟**
>
> *Xué hǎi wú yá kǔ zuò zhōu*
>
> "The sea of knowledge is endless; diligence is your boat."

Based on SLIDE 9 EFFICIENCY OF ALGORITHM.pptx. 【1-b01c67】

---
# 🎯 Ultra-Short Answers

```text
O(1)      Array Access
O(log n)  Binary Search
O(n)      Linear Search
O(n log n) Merge Sort, Quick Sort
O(n²)     Bubble Sort, Insertion Sort
O(2ⁿ)     Brute Force Password Cracking
O(n!)     Traveling Salesman

Bubble Sort Space = O(1)
Insertion Sort Space = O(1)
Merge Sort Space = O(n)
Quick Sort Space = O(log n)

BFS = Queue
DFS = Stack / Recursion

DFS Order:
A → B → D → E → C → F
```
---------

# 💜 Class Assignment 1 - Logarithmic Time O(log n)

## Question

A database system uses logarithmic time to quickly locate a record in a sorted list of user IDs. Assuming the database contains **500 records**:

1. Giving an example of the specific algorithm, explain how this algorithm functions.
2. Write the general formula for the number of steps required by logarithmic time in the worst case.
3. Using the formula above, calculate the number of steps for 500 records.
4. If the number of records is doubled to 1000, how many additional steps are required?

---

## Answer

### 1. Algorithm Example

**Binary Search**

Binary Search repeatedly checks the middle element of a sorted list.

Example:

```text
[1,2,3,4,5,6,7,8,9]
```

Searching for 8:

```text
Middle = 5
8 > 5 → Search Right Side

Middle = 7
8 > 7 → Search Right Side

Middle = 8
Found
```

### 2. Formula

```text
Steps = log₂(n)
```

### 3. For 500 Records

```text
log₂(500) ≈ 8.97
```

Worst case:

```text
9 steps
```

### 4. For 1000 Records

```text
log₂(1000) ≈ 9.97
```

Worst case:

```text
10 steps
```

Additional steps:

```text
10 - 9 = 1 step
```

✅ Final Answer: **Only 1 extra step is needed.**

---

# 💜 Class Assignment 2 - Linear vs Linearithmic Time

## Question

A software company is developing two features:

- Feature A scans every record once.
- Feature B repeatedly divides data and combines results.

Answer the questions provided.

---

## Answer

### 1. Time Complexities

| Feature | Complexity |
|----------|------------|
| Feature A | O(n) |
| Feature B | O(n log n) |

Feature A scans every item once.

Feature B divides data and processes each part.

---

### 2. Which Is Faster?

As n becomes very large:

```text
O(n) < O(n log n)
```

✅ Feature A is faster.

---

### 3. Recommendation

For a real-time system handling millions of records:

✅ Recommend **Feature A (O(n))**

Reason:

- Fewer operations
- Faster execution
- Better scalability

---

### 4. Algorithm Examples

| Feature | Example |
|----------|----------|
| O(n) | Linear Search |
| O(n log n) | Merge Sort, Quick Sort |

---

# 💜 Class Assignment 3 - Exponential Time O(2ⁿ)

## Question

A password cracking system doubles the number of possibilities whenever one more character is added.

---

## Answer

### a) Time Complexity

```text
O(2ⁿ)
```

---

### b) Number of Steps

#### i) n = 5

```text
2⁵ = 32
```

#### ii) n = 10

```text
2¹⁰ = 1024
```

---

### c) Why Impractical?

As n increases:

```text
n = 20 → 1,048,576
n = 30 → 1,073,741,824
```

The number of operations grows extremely fast.

✅ Execution time becomes too large.

---

### d) Real-World Use

Possible use:

- Brute-force testing of very short passwords
- Small encryption keys for demonstrations

---

# 💜 Class Assignment 5 - Bubble Sort

## Question

Using Bubble Sort, sort:

```text
7 3 8 2 5
```

Show the first two passes.

---

## Answer

### Pass 1

```text
7 3 8 2 5

7↔3
3 7 8 2 5

8↔2
3 7 2 8 5

8↔5
3 7 2 5 8
```

Result:

```text
3 7 2 5 8
```

---

### Pass 2

```text
3 7 2 5 8

7↔2
3 2 7 5 8

7↔5
3 2 5 7 8
```

Result:

```text
3 2 5 7 8
```

---

### b) Why In-Place?

Bubble Sort only swaps elements within the same array.

✅ No extra array is needed.

---

### c) Space Complexity

```text
O(1)
```

Reason:

Only a temporary variable is required for swapping.

---

# 💜 Class Assignment 6 - Insertion Sort

## Question

Sort:

```text
[6,4,9,3,7]
```

Using Insertion Sort.

---

## Answer

### Step 1

Insert 4

```text
[4,6,9,3,7]
```

---

### Step 2

Insert 9

```text
[4,6,9,3,7]
```

(No change)

---

### Step 3

Insert 3

```text
[3,4,6,9,7]
```

---

### Step 4

Insert 7

```text
[3,4,6,7,9]
```

---

### Property of Left Side

At every step:

✅ The left portion is always sorted.

---

### Space Complexity

```text
O(1)
```

Reason:

- Input array stays in memory.
- Only a few variables are used.

---

# 💜 Class Assignment 7 - Merge Sort

## Question

Sort:

```text
[5,2,9,1]
```

Using Merge Sort.

---

## Answer

### Divide Phase

```text
[5,2,9,1]

[5,2] [9,1]

[5][2] [9][1]
```

---

### Merge Phase

Merge:

```text
[5] [2]
→ [2,5]

[9] [1]
→ [1,9]
```

Merge again:

```text
[2,5] [1,9]

→ [1,2,5,9]
```

---

### Final Sorted Array

```text
[1,2,5,9]
```

---

### Space Complexity Analysis

#### Input Storage

```text
O(n)
```

#### Temporary Arrays

```text
O(n)
```

#### Recursive Calls

```text
O(log n)
```

Overall:

```text
O(n)
```

---

### Why Better for Large Data?

✅ Faster than Bubble Sort

✅ Faster than Insertion Sort

✅ Complexity:

```text
O(n log n)
```

instead of

```text
O(n²)
```

---

# 💜 Assignment 8 - Quick Sort

## Question

Sort:

```text
[8,3,6,2,7,5,4]
```

Pivot = Last Element

---

## Answer

### a) First Partition

Pivot:

```text
4
```

After partition:

```text
[3,2,4,8,7,5,6]
```

Pivot position:

```text
Index 2
```

---

### b) Recursive Partitions

Left:

```text
[3,2]
```

Pivot:

```text
2
```

Result:

```text
[2,3]
```

---

Right:

```text
[8,7,5,6]
```

Pivot:

```text
6
```

Result:

```text
[5,6,8,7]
```

---

Array becomes:

```text
[2,3,4,5,6,8,7]
```

Continue recursively:

```text
[2,3,4,5,6,7,8]
```

---

### c) Space Complexity

#### Input Storage

```text
O(n)
```

#### Auxiliary Variables

```text
O(1)
```

#### Recursive Stack

```text
O(log n)
```

Average overall space:

```text
O(log n)
```

---

# 🌸 Self-Reading Assignment 1 - Quadratic Time

## Question

Students must be paired with every other student.

---

## Answer

### Java Program

```java
for(int i=0;i<n;i++)
{
    for(int j=0;j<n;j++)
    {
        System.out.println(i + "," + j);
    }
}
```

---

### For n = 5

Outer loop:

```text
5 times
```

Inner loop:

```text
5 times
```

Total:

```text
5 × 5 = 25
```

✅ Answer: **25 executions**

---

### Why O(n²)?

Nested loops:

```text
n × n = n²
```

Therefore:

```text
O(n²)
```

---

# 🌸 Self-Reading Assignment 2 - DFS

## Question

Perform DFS on:

```text
    A
   / \
  B   C
 / \   \
D   E   F
```

---

## Answer

### DFS Traversal

Start at A.

Go left first.

```text
A → B → D
```

Backtrack.

```text
A → B → E
```

Backtrack to A.

```text
A → C → F
```

✅ DFS Order:

```text
A → B → D → E → C → F
```

---

### Backtracking

Backtracking means returning to a previous node when there are no unvisited neighbors.

Example:

```text
A → B → D
```

D has no children.

Return to:

```text
B
```

This return process is called **backtracking**.

---



💜 **功夫不负有心人**
(*Gōngfu bù fù yǒuxīn rén*)

*"Hard work never disappoints a determined person."*
