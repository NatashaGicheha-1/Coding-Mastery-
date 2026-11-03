# 💜📚1.  Efficiency of Algorithms

> 💜 **功夫不负有心人**
>
> *Gōngfu bù fù yǒuxīn rén*
>
> "Hard work never disappoints a determined person."

---
# 📝 Expected Exam Format

### 1️⃣ Definitions (Theory)
Be able to define:
- Algorithm Efficiency
- Time Complexity
- Space Complexity
- Recursion
- Iteration
- BFS
- DFS

### 2️⃣ Complexity Identification
Identify complexity from code:

```java
for(...)              → O(n)

for(...)
   for(...)           → O(n²)

for(...)
   for(...)
      for(...)        → O(n³)
```

### 3️⃣ Calculations
Be able to calculate:
- O(log n)
- O(2ⁿ)
- n!

### 4️⃣ Algorithm Tracing
Show step-by-step execution of:
- Bubble Sort
- Insertion Sort
- Merge Sort
- Quick Sort
- Linear Search
- Binary Search

### 5️⃣ BFS & DFS Questions
- Traversal order
- Queue vs Stack
- Backtracking

----------

# 🎯 30-Second Cram

```text
O(1)      → Array Access
O(log n)  → Binary Search
O(n)      → Linear Search
O(n log n)→ Merge Sort, Quick Sort
O(n²)     → Bubble Sort, Insertion Sort
O(n³)     → Three Nested Loops
O(2ⁿ)     → Recursive Fibonacci
O(n!)     → Traveling Salesman

Recursive → O(n) Space
Iterative → O(1) Space

BFS → Queue
DFS → Stack/Recursion
```
 ------- 
 
# 🎯 What is Algorithm Efficiency?

Algorithm efficiency measures how well an algorithm uses:

- ⏱️ Time (execution speed)
- 💾 Memory (space usage)

Why it matters:

- 🚀 Faster programs
- 💾 Less memory usage
- 📊 Better for large datasets
- ⚡ Saves resources


---

# ⏱️ Time Complexity (Big O)

| Complexity | Meaning | Example |
|------------|----------|----------|
| 🏆 O(1) | Constant time | Array access |
| 🥈 O(log n) | Reduce problem by half | Binary Search |
| 🥉 O(n) | Check every item once | Linear Search |
| ⭐ O(n log n) | Divide and process | Merge Sort, Quick Sort |
| ⚠️ O(n²) | Two nested loops | Bubble Sort, Insertion Sort |
| ❌ O(n³) | Three nested loops | 3D Matrix Operations |
| ☠️ O(2ⁿ) | Doubles every step | Recursive Fibonacci |
| 💀 O(n!) | Factorial growth | Traveling Salesman |

---

# 📌 Key Algorithms

### 🔍 Linear Search
- Checks elements one by one
- Time: **O(n)**
- Space: **O(1)**

### 🔎 Binary Search
- Works only on sorted data
- Repeatedly checks the middle element
- Time: **O(log n)**
- Space: **O(1)** (iterative)

### 🫧 Bubble Sort
- Swaps adjacent elements
- Largest element moves to the end
- Time: **O(n²)**
- Space: **O(1)**

### 🃏 Insertion Sort
- Like arranging cards in your hand
- Inserts each item into the correct position
- Time: **O(n²)**
- Space: **O(1)**

### 🔀 Merge Sort
- Divide → Sort → Merge
- Time: **O(n log n)**
- Space: **O(n)**

### ⚡ Quick Sort
- Choose a pivot
- Place smaller values left and larger values right
- Time: **O(n log n)** (average)
- Space: **O(1)** + recursion stack

---

# 💾 Space Complexity

Space complexity measures memory used by an algorithm.

### Memory Sources
- Variables
- Arrays
- Temporary storage
- Recursion stack

---

# 🔄 Recursion vs Iteration

| Feature | Recursive | Iterative |
|----------|-----------|-----------|
| Call Stack | ✅ Yes | ❌ No |
| Extra Space | O(n) | O(1) |
| Stack Overflow Risk | ✅ Yes | ❌ No |

🧠 Memory Trick:

- 🍽️ Recursion = stacking plates
- ♻️ Iteration = reusing one plate

---

# 🌳 Graph Traversal

### 🚶 BFS (Breadth-First Search)
- Visits level by level
- Uses a Queue
- Example: A → B → C → D → E → F

### 🕳️ DFS (Depth-First Search)
- Goes as deep as possible first
- Uses Stack/Recursion
- Example: A → B → D → E → C → F
- Backtracking = returning to previous nodes when stuck







