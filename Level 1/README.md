
# 🌳 Trees (DSA)

## 1. What is a Tree?

A **tree** is a **non-linear data structure** made up of **nodes** connected by **edges**, used to represent **hierarchical relationships**.

In simple words:

> A tree shows data in **parent–child form**, just like a **family tree**, **folder structure**, or **organization chart**.

---

## 2. Basic Structure of a Tree

* A tree has **one special node** called the **root**
* Every node (except root) has **exactly one parent**
* Nodes can have **zero or more children**
* There is **only one path** between any two nodes

---

## 3. Example Tree (We’ll use this everywhere)

```
            A
       /    |    \
     B      C     D
    /  \     |     \
   E    F    G      H
 / | \       | \
I  J  K      L   M
```

---

## 4. Tree Terminologies (With Strong Intuition)

### 4.1 Node

Each **entity/data element** in a tree is called a **node**.
Example: `A, B, C, D, E, F, ...`

---

### 4.2 Root Node

* The **topmost node** of the tree
* Has **no parent**

📌 In our example:
**Root Node = A**

---

### 4.3 Parent Node

A node that has **one or more children**.

📌 Example:

* `A` is parent of `B, C, D`
* `B` is parent of `E, F`

---

### 4.4 Child Node

A node that is the **immediate successor** of another node.

📌 Example:

* `B, C, D` are children of `A`
* `E, F` are children of `B`

---

### 4.5 Sibling

Nodes that share the **same parent**.

📌 Example:

* `B, C, D` are siblings
* `I, J, K` are siblings

---

### 4.6 Leaf Node (External Node)

A node that has **no children**.

📌 In our example, leaf nodes are:
`I, J, K, L, M, F, H, C`

💡 **Important rule**:

> Degree of all leaf nodes is **0**

---

### 4.7 Internal Node

Any node that has **at least one child**.

📌 Example:
`A, B, D, E, G`

---

### 4.8 Edge

A **connection/link** between two nodes.

📌 Example:

* Edge between `A → B`
* Edge between `E → I`

💡 **Key property**:
If a tree has **N nodes**, it will always have **(N − 1) edges**

---

### 4.9 Path

A **sequence of consecutive edges** from one node to another.

📌 Example:
Path from `A` to `K`:

```
A → B → E → K
```

---

### 4.10 Ancestors

All nodes that come **before a node** on the path from the **root**.

📌 Example:
Ancestors of `K` are:

```
A, B, E
```

---

### 4.11 Descendants

All nodes that come **after a node** on paths toward leaf nodes.

📌 Example:
Descendants of `B` are:

```
E, F, I, J, K
```

---

### 4.12 Subtree

A **tree formed by any node and all of its descendants**.

📌 Example:
Subtree rooted at `B`:

```
     B
   /   \
  E     F
 / | \
I  J  K
```

---

## 5. Degree Concepts

### 5.1 Degree of a Node

Number of **children** a node has.

📌 Examples:

* Degree of `A` = 3
* Degree of `B` = 2
* Degree of `E` = 3
* Degree of `I` = 0

---

### 5.2 Degree of the Tree

The **maximum degree** among all nodes in the tree.

📌 In our example:
Maximum children = **3**
So, **Degree of Tree = 3**

---

## 6. Depth, Height, and Level (Very Important Section)

### 6.1 Depth of a Node

Number of **edges from the root to that node**.

📌 Examples:

* Depth of `A` = 0
* Depth of `B` = 1
* Depth of `E` = 2
* Depth of `K` = 3

💡 Rule:

> Depth of **ROOT node is always 0**

---

### 6.2 Height of a Node

Number of **edges in the longest path** from that node to a **leaf node**.

📌 Examples:

* Height of `K` = 0
* Height of `E` = 1
* Height of `B` = 2
* Height of `A` = 3

---

### 6.3 Height of the Tree

Height of the **root node**.

📌 In our example:
**Height of Tree = 3**

---

### 6.4 Level of a Node

Level is **same as depth** (counting edges from root).

📌 Example:

* Level of `A` = 0
* Level of `B` = 1
* Level of `E` = 2

---

## 7. Important Relationships

✔ Level of Tree = Height of Tree,
✔ Level of Node = Depth of Node,
❌ Level of Node ≠ Height of Node,

---

## 8. Key Properties Summary

* Root has **no parent**
* Leaf nodes have **degree 0**
* Depth of root is **0**
* Tree with **N nodes** has **N − 1 edges**
* Every node has **exactly one parent** (except root)

---
