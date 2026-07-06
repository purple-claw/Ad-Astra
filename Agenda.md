# Rules - Must Follow

**Subject:** Algorithms & Data Structures (from scratch → FAANG-ready → systems-builder level)
**Timeline:** 2–3 years, ~8–15 hrs/week
**Language:** Python first → transition to C++ around month 6+ (Phase 10)
**Grounded in:** MIT 6.006 (Demaine/Ku/Solomon) structure + CLRS Parts I–VI, adapted for a self-taught, math-first, systems-thinking track.

**Learner starting point:** Comfortable writing small programs, no formal DSA yet. Math: starting from true basics (assume nothing).

---

## Phase 0 — Mathematical Foundations (the toolkit everything else depends on)
*This phase exists because you can't reason about correctness or efficiency without it. CLRS itself opens with a "Mathematical Foundations" part for the same reason.*

- 0.1 Mathematical logic & proof techniques (direct proof, contrapositive, proof by contradiction)
- 0.2 Proof by induction (weak & strong) — the backbone of correctness proofs
- 0.3 Sets, functions, relations — notation you'll see everywhere
- 0.4 Exponents & logarithms — algebraic properties (this *is* complexity analysis in disguise)
- 0.5 Summations & series (arithmetic, geometric, manipulating Σ notation)
- 0.6 Basic combinatorics & counting principles
- 0.7 Basic probability (needed later for hashing & randomized algorithms)
- 0.8 Modular arithmetic (needed for hashing, number theory)
- 0.9 Graph theory basics — pure math (vertices, edges, degree) before any code
- 0.10 Recurrence relations — setting them up (solving comes in Phase 1)

## Phase 1 — Computational Thinking & Complexity Analysis
- 1.1 What is an algorithm? Problem vs. algorithm vs. program
- 1.2 The RAM model of computation
- 1.3 Big-O — the formal definition (not the hand-wavy version)
- 1.4 Big-Omega & Big-Theta — formal definitions
- 1.5 Combining complexities — sum rule, product rule
- 1.6 Analyzing loops — single and nested
- 1.7 Best / worst / average case analysis
- 1.8 Amortized analysis — intuition and the accounting method
- 1.9 Space complexity fundamentals — stack vs. heap, cost of recursion
- 1.10 Solving recurrences — substitution method
- 1.11 Solving recurrences — recursion tree method
- 1.12 The Master Theorem
- 1.13 Python's cost model — what actually costs time in Python (list ops, string ops)
- 1.14 Empirical complexity — benchmarking your own code, spotting constant-factor lies

## Phase 2 — Memory Model & Linear Data Structures
- 2.1 How memory actually works — stack, heap, references vs. values
- 2.2 Arrays — static vs. dynamic, why contiguous memory matters
- 2.3 Dynamic arrays — amortized doubling (how Python's `list` really works)
- 2.4 Strings as arrays — Python's immutability and what it costs you
- 2.5 Singly linked lists — concept & implementation
- 2.6 Doubly linked & circular linked lists
- 2.7 Stacks — LIFO, array vs. linked-list implementation
- 2.8 Queues — FIFO, circular queue, deque
- 2.9 Two-pointer technique
- 2.10 Sliding window technique
- 2.11 Recursion deep-dive — call stack tracing, base case design
- 2.12 Recursion vs. iteration — the real space-complexity tradeoff

## Phase 3 — Sorting & Searching
- 3.1 Binary search — the concept and its invariants
- 3.2 Binary search variants (first/last occurrence, rotated array search)
- 3.3 Bubble / insertion / selection sort — why they still matter conceptually
- 3.4 Merge sort — your first real divide-and-conquer algorithm
- 3.5 Quick sort — partitioning logic, pivot strategy
- 3.6 The comparison-sort lower bound — proving Ω(n log n)
- 3.7 Non-comparison sorts — counting sort, radix sort, bucket sort
- 3.8 Choosing the right sort — stability, in-place, adaptiveness

## Phase 4 — Hashing
- 4.1 Hash functions — what makes one "good"
- 4.2 Collision resolution — chaining
- 4.3 Collision resolution — open addressing (linear/quadratic probing, double hashing)
- 4.4 Load factor & rehashing (table doubling)
- 4.5 Python's `dict`/`set` internals
- 4.6 Hashing-based problem-solving patterns

## Phase 5 — Trees & Heaps
- 5.1 Tree terminology & properties
- 5.2 Binary trees — traversals (pre/in/post/level order)
- 5.3 Binary Search Trees — properties & operations
- 5.4 BST complexity analysis — why worst case degrades to O(n)
- 5.5 Why balance matters — the core idea behind self-balancing trees
- 5.6 AVL trees — rotations
- 5.7 Red-black trees — conceptual understanding (not obsessive implementation)
- 5.8 Binary heaps — heapify, priority queues
- 5.9 Heap applications — k-th largest, merge-k-sorted-lists
- 5.10 Tries — prefix trees
- 5.11 Segment trees — range queries
- 5.12 Fenwick tree / Binary Indexed Tree
- 5.13 Union-Find / Disjoint Set Union

## Phase 6 — Graphs
- 6.1 Graph representations — adjacency matrix vs. list, tradeoffs
- 6.2 BFS — concept, implementation, complexity
- 6.3 DFS — concept, implementation, complexity
- 6.4 Connected components
- 6.5 Topological sort
- 6.6 Cycle detection (directed & undirected)
- 6.7 Shortest paths — Dijkstra
- 6.8 Shortest paths — Bellman-Ford
- 6.9 Shortest paths — Floyd-Warshall
- 6.10 Minimum Spanning Tree — Prim's
- 6.11 Minimum Spanning Tree — Kruskal's
- 6.12 Strongly connected components — Tarjan / Kosaraju
- 6.13 Network flow basics — Ford-Fulkerson (systems-relevant)

## Phase 7 — Algorithmic Paradigms & Problem-Solving Thinking
*This is the heart of "learning the logic," not just the algorithms.*
- 7.1 The brute-force → optimize mindset — the systematic thinking process
- 7.2 Greedy algorithms — when greedy works, proving it (exchange argument)
- 7.3 Divide & conquer as a general paradigm (beyond sorting)
- 7.4 Dynamic programming — overlapping subproblems & optimal substructure
- 7.5 DP — memoization (top-down)
- 7.6 DP — tabulation (bottom-up)
- 7.7 DP on 1D problems
- 7.8 DP on 2D problems (grids, strings)
- 7.9 DP — knapsack family
- 7.10 DP — interval DP
- 7.11 DP — state machine / bitmask DP
- 7.12 Backtracking — systematic search & pruning
- 7.13 Branch and bound
- 7.14 Bit manipulation techniques

## Phase 8 — Advanced Topics & Systems-Level Thinking
- 8.1 String matching — KMP
- 8.2 String matching — Rabin-Karp, Z-algorithm
- 8.3 Suffix arrays/trees (conceptual)
- 8.4 Computational geometry basics
- 8.5 NP-completeness — what it means and why it matters practically
- 8.6 Approximation algorithms — intuition
- 8.7 Randomized algorithms
- 8.8 Cache-aware / external-memory algorithms — real systems relevance
- 8.9 Concurrency-adjacent data structures — bridging toward "building real systems"

## Phase 9 — Interview Craft & Applied Practice
- 9.1 A structured framework for novel problems (clarify → examples → brute force → optimize → code → test)
- 9.2 Communicating your thought process out loud
- 9.3 Testing & edge-case thinking
- 9.4 Time-boxing & knowing when to pivot approach
- 9.5 How DSA choices ripple into system design
- 9.6 Mock interview practice loop

## Phase 10 — C++ Transition Layer (starts once your C++ course is done)
- Re-implementing core structures in modern C++
- STL mapped against what you learned in Python
- Manual memory management — pointers, RAII (vs. Python's abstracted memory)
- Templates & generic programming
- Competitive-programming-grade C++ idioms (fast I/O, etc.)

---

## Orion State — DSA Mastery
- **Position:** Curriculum proposed, awaiting buy-in — not yet started
- **Standards:** Not yet locked in (Step 3, next)
- **Mastered:** none yet
- **Watch for:** —
- **Up next:** 0.1 Mathematical logic & proof techniques
