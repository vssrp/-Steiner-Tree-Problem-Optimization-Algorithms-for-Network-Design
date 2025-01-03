# Steiner Tree Problem 🔗
---

## Overview
The Steiner Tree Problem is a combinatorial optimization challenge in graph theory, aimed at finding a minimum-cost tree connecting a subset of vertices (terminals) in a graph. This project explores both exact and heuristic approaches to solve the problem, highlighting their trade-offs in terms of accuracy and computational efficiency. The solution has significant applications in **VLSI design**, **telecommunications**, **transportation networks**, and other fields requiring cost-efficient connectivity.

---

## Objectives
- Identify a minimum-cost tree spanning specific terminal vertices.
- Balance the trade-off between accuracy and computational efficiency for NP-hard problems.
- Explore the **Branch-and-Bound** algorithm for exact solutions and the **Vazirani and Yannakakis** approximation algorithm for faster, near-optimal results.

---

## Key Features
- **Exact Solution**: Implemented the **Branch-and-Bound algorithm**, ensuring optimal solutions with exponential time complexity.
- **Approximation Approach**: Developed the **Vazirani and Yannakakis algorithm**, providing efficient solutions within a guaranteed error bound.
- **Trade-Off Analysis**: Compared the computational performance and accuracy of both methods.

---

## Real-Life Applications
- **VLSI Design**: Optimize integrated circuit layouts to minimize costs and improve efficiency.
- **Telecommunications**: Design cost-effective fiber optic and cable networks.
- **Transportation Networks**: Optimize routes for pipelines, power lines, and road systems.
- **Molecular Biology**: Construct phylogenetic trees for studying evolutionary relationships.
- **Robotics**: Enable robots to traverse shortest paths with minimal costs.

---

## Algorithms Implemented

### 1. **Branch-and-Bound Algorithm**
- Guarantees an exact solution by systematically exploring all possible trees.
- Uses bounds to prune suboptimal solutions, improving efficiency.
- **Complexity**:  
  - Time: \(O(2^n)\) in the worst case.  
  - Space: \(O(n)\).

### 2. **Vazirani and Yannakakis Algorithm**
- Approximation algorithm with a guaranteed error bound (approximation ratio ≤ 2).
- Constructs a Minimum Spanning Tree (MST) for clusters of terminal nodes and connects them.
- **Complexity**:  
  - Time: \(O(|E| \log(|V|))\), where \(|E|\) is the number of edges and \(|V|\) is the number of vertices.  
  - Space: \(O(n)\).

---

## Results
- **Branch-and-Bound Algorithm**: Achieved optimal solutions but required significantly more computational time, particularly for larger graphs.
- **Approximation Algorithm**: Delivered near-optimal solutions over 200 times faster than the exact method, making it ideal for real-world applications.

---

## Methodology
1. **Graph Definition**:
   - Input: Graph \(G(V, E)\) with terminal vertices \(T(V)\) and edge weights \(Cost(E)\).
2. **Algorithm Implementation**:
   - **Branch-and-Bound**:
     - Recursive search with pruning for efficiency.
     - Optimal solutions guaranteed.
   - **Vazirani and Yannakakis**:
     - Construct MST clusters and connect them to form a near-optimal solution.
3. **Performance Metrics**:
   - Execution time.
   - Optimality of solutions.
   - Error bound for approximation.

---

## How to Run the Project
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/steiner-tree-problem.git
   cd steiner-tree-problem
