# Recursion in C++

### Introduction

Recursion is a programming technique where a **function calls itself** to solve a larger problem by breaking it into **smaller, similar sub-problems**. It follows the **Divide and Conquer** principle, solving each smaller instance until a **base case** is reached. Afterward, results are returned step by step as the recursion unwinds.

**Example:**

```text
Factorial(5) → 5 × Factorial(4) → 5 × 4 × Factorial(3) → … → 5 × 4 × 3 × 2 × 1
```

---

### Key Components of Recursion

* **Base Case:** Condition that stops recursion to prevent infinite calls.
* **Recursive Case:** The portion where the function calls itself.
* **Call Stack:** Each recursive call uses system memory until the base case is met.

---

### Advantages of Recursion

* Simplifies complex problems (tree/graph traversal, backtracking, divide-and-conquer).
* Closely matches mathematical formulations (factorial, Fibonacci, GCD).
* Reduces code length and improves readability for repetitive problems.

### Disadvantages of Recursion

* Memory intensive; deep recursion may cause **stack overflow**.
* Performance overhead due to repeated function calls.
* Harder to debug compared to iterative solutions.

---

### Types of Recursion

1. **Direct Recursion:** Function calls itself directly.

   * Example: `factorial(n)` calls `factorial(n-1)`
2. **Indirect Recursion:** Function calls another function, which calls the first.
3. **Tail Recursion:** Recursive call is the last statement; optimizable by compiler.
4. **Non-Tail Recursion:** Recursive call followed by additional operations (e.g., multiplication in factorial).

---

### Recursion vs Iteration

| Feature          | Recursion                       | Iteration                    |
| ---------------- | ------------------------------- | ---------------------------- |
| Definition       | Function calls itself           | Loop repeats until condition |
| Termination      | Requires a base case            | Requires loop condition      |
| Memory Usage     | High (call stack)               | Low (no stack calls)         |
| Performance      | Slower due to function calls    | Faster via direct looping    |
| Code Readability | More elegant, compact           | More verbose                 |
| Risk             | Stack overflow                  | Infinite loop risk           |
| Applications     | Trees, graphs, divide & conquer | Counting, summation          |

---

### Applications of Recursion

* **Mathematics:** Factorials, Fibonacci series, exponentiation.
* **Data Structures:** Tree and graph traversal (DFS).
* **Algorithms:** Quick Sort, Merge Sort, Binary Search (recursive).
* **Backtracking:** Sudoku solver, N-Queens, maze solving.
* **System Programs:** Directory traversal, compiler parsing.

---

### Example Programs

#### 1️⃣ Factorial and Sum

**Algorithm:**

1. Input number `n`.
2. **Factorial:**

   * Base case: If `n == 0 or 1`, return 1.
   * Recursive case: `return n * factorial(n-1)`
3. **Sum of first n numbers:**

   * Base case: If `n == 0`, return 0.
   * Recursive case: `return n + sum(n-1)`
4. Display results.

---

#### 2️⃣ String Reversal

**Algorithm:**

1. Input string `str`.
2. Base case: If `start >= end`, return.
3. Swap `str[start]` and `str[end]`.
4. Recursively call function with `start+1` and `end-1`.
5. Print reversed string.

---

### Conclusion

* Recursion simplifies problem-solving for tasks like **factorials, summation, and string reversal**.
* A **base case** is essential to avoid infinite recursion.
* Compared to iteration, recursion **uses more memory** but produces **cleaner, more mathematical solutions**.
* Mastery of recursion is essential for handling **complex problems in C++ programming**.

