# Types of Tree Data Structures

## Table of Contents

1. [Introduction](#introduction)
2. [Types of Trees](#types-of-trees)
   - [Binary Tree](#1-binary-tree)
   - [Full Binary Tree](#2-full-binary-tree)
   - [Complete Binary Tree](#3-complete-binary-tree)
   - [Balanced Binary Tree](#4-balanced-binary-tree)
   - [Ternary Tree](#5-ternary-tree)
   - [N-ary Tree (Generic Tree)](#6-n-ary-tree-generic-tree)
3. [Comparison of Tree Types](#comparison-of-tree-types)
4. [Conclusion](#conclusion)

---

## Introduction

A **tree** is a non-linear data structure used to organize data in a hierarchical manner. It consists of nodes connected by edges. The topmost node is called the **root**, while nodes that do not have any children are called **leaf nodes**.

Tree data structures are commonly used in file systems, databases, search algorithms, and hierarchical data representation.

Trees can be classified according to the maximum number of children each node can have and the structure of their nodes.

---

## Types of Trees

### 1. Binary Tree

**What is a Binary Tree?**

A **Binary Tree** is a tree data structure in which each node can have a maximum of two children, known as the **left child** and the **right child**.

**Characteristics:**

- Each node can have zero, one, or two children.
- Each node has at most one left child and one right child.
- Binary trees are used in searching, sorting, and expression evaluation.

**Example:**

```text
        10
       /  \
      20   30
     / \
    40  50
```

In this example, `10` is the root node, `20` and `30` are its children, and `40` and `50` are the children of node `20`.

---

### 2. Full Binary Tree

**What is a Full Binary Tree?**

A **Full Binary Tree** is a binary tree in which every node has either zero or two children. No node has exactly one child.

**Characteristics:**

- Every internal node has exactly two children.
- Leaf nodes have no children.
- It follows the structural rules of a binary tree.

**Example:**

```text
        10
       /  \
      20   30
     / \
    40  50
```

In this example, every internal node has exactly two children, while the leaf nodes have no children. Therefore, it is a full binary tree.

---

### 3. Complete Binary Tree

**What is a Complete Binary Tree?**

A **Complete Binary Tree** is a binary tree in which all levels are completely filled except possibly the last level. The last level is filled from left to right.

**Characteristics:**

- All levels before the last level are completely filled.
- The last level contains nodes as far to the left as possible.
- Complete binary trees are commonly used to implement heaps.

**Example:**

```text
        10
       /  \
      20   30
     / \   /
    40 50 60
```

In this example, the last level is filled from left to right without any gaps, so it is a complete binary tree.

---

### 4. Balanced Binary Tree

**What is a Balanced Binary Tree?**

A **Balanced Binary Tree** is a binary tree in which the heights of the left and right subtrees are kept within a specified limit at each node, according to the balancing rule being used.

**Characteristics:**

- The tree avoids becoming unnecessarily tall.
- Its height is generally proportional to the logarithm of the number of nodes when it is height-balanced.
- Balanced trees can provide efficient searching, insertion, and deletion.

**Example:**

```text
        20
       /  \
      10   30
     / \   / \
    5  15 25 35
```

This tree is balanced because its left and right subtrees have equal heights at every node.

---

### 5. Ternary Tree

**What is a Ternary Tree?**

A **Ternary Tree** is a tree data structure in which each node can have a maximum of three children, commonly called the **left**, **middle**, and **right** children.

**Characteristics:**

- Each node can have zero to three children.
- Nodes may have different numbers of children.
- Ternary trees can be used in specialized searching and data-processing applications.

**Example:**

```text
          10
       /   |   \
      20   30   40
     / \
    50  60
```

In this example, node `10` has three children: `20`, `30`, and `40`.

---

### 6. N-ary Tree (Generic Tree)

**What is an N-ary Tree?**

An **N-ary Tree**, also known as a **Generic Tree**, is a tree data structure in which each node can have any number of children, depending on the requirements of the application.

**Characteristics:**

- Each node stores some data.
- Each node can have zero or more children.
- A node maintains references to its child nodes.
- Duplicate values may be allowed or disallowed depending on the implementation.
- Unlike a linked list, where each node typically points to the next node, a generic tree node can reference multiple child nodes.

**Example:**

```text
              10
          /    |    \
         20    30    40
        / \          |
       50  60        70
```

In this example, node `10` has three children, while node `20` has two children. This demonstrates that different nodes can have different numbers of children.

---

## Comparison of Tree Types

| Tree Type | Maximum Children | Main Property |
|---|---:|---|
| Binary Tree | 2 | Each node has at most two children |
| Full Binary Tree | 2 | Every node has either 0 or 2 children |
| Complete Binary Tree | 2 | The last level is filled from left to right |
| Balanced Binary Tree | 2 | Subtree heights follow a balancing rule |
| Ternary Tree | 3 | Each node has at most three children |
| N-ary Tree | No fixed limit | Each node can have any number of children |

---

## Conclusion

Tree data structures are essential for organizing hierarchical data efficiently. Binary trees allow a maximum of two children per node, while ternary trees allow up to three children. N-ary trees provide greater flexibility by allowing any number of children.

Understanding these tree types helps in selecting the appropriate data structure for applications such as searching, sorting, hierarchical storage, and database management.

