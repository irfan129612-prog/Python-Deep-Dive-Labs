# 🧪 Lab 37: BFS / DFS Implementation (Data Structures)

## 📌 Lab Summary

In this lab, two fundamental graph traversal algorithms, **Breadth-First Search (BFS)** and **Depth-First Search (DFS)**, were implemented using Python. A graph was represented as an adjacency list, and both traversal methods were used to explore its nodes. BFS utilized a queue (`deque`), while DFS employed recursion. These algorithms form the foundation of many applications in networking, artificial intelligence, and cybersecurity.

---

## 🎯 Objectives

- Understand graph traversal algorithms
- Represent a graph using an adjacency list
- Implement Breadth-First Search (BFS)
- Implement Depth-First Search (DFS)
- Compare BFS and DFS traversal techniques

---

## 🛠️ Tools Used

- Ubuntu Linux
- Python 3.x
- PyCharm Community Edition
- Ubuntu Terminal

---

## 🗂️ Lab Environment

| Component | Details |
|----------|---------|
| Operating System | Ubuntu Linux |
| Python Version | Python 3.x |
| IDE | PyCharm Community Edition |
| Data Structure | Graph (Adjacency List) |
| Terminal | Ubuntu CLI |

---

## ✅ Task 1: Create the Graph

The graph was represented using an adjacency list.

```python
graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}
```

### Result

- ✅ Graph successfully created using a dictionary.

---

## ✅ Task 2: Implement Breadth-First Search (BFS)

The BFS algorithm was implemented using a queue provided by `collections.deque`.

```python
from collections import deque

def bfs(start_node, graph):

    visited = set()

    queue = deque([start_node])

    while queue:

        node = queue.popleft()

        if node not in visited:

            print(node, end=" ")

            visited.add(node)

            queue.extend(
                [n for n in graph[node]
                 if n not in visited]
            )
```

### Result

The graph was traversed level by level.

---

## ✅ Task 3: Implement Depth-First Search (DFS)

The DFS algorithm was implemented recursively.

```python
def dfs(node, graph, visited=None):

    if visited is None:
        visited = set()

    if node not in visited:

        print(node, end=" ")

        visited.add(node)

        for neighbor in graph[node]:
            dfs(neighbor, graph, visited)
```

### Result

The graph was explored deeply before backtracking.

---

## ✅ Task 4: Execute the Traversal

Run both algorithms.

```python
bfs("A", graph)

print()

dfs("A", graph)
```

### Output

```text
BFS Traversal:
A B C D E F

DFS Traversal:
A B D E F C
```

---

## 💻 Complete Code

```python
from collections import deque

graph = {
    'A': ['B', 'C'],
    'B': ['D', 'E'],
    'C': ['F'],
    'D': [],
    'E': ['F'],
    'F': []
}

def bfs(start_node, graph):

    visited = set()

    queue = deque([start_node])

    while queue:

        node = queue.popleft()

        if node not in visited:

            print(node, end=" ")

            visited.add(node)

            queue.extend(
                [n for n in graph[node]
                 if n not in visited]
            )

def dfs(node, graph, visited=None):

    if visited is None:
        visited = set()

    if node not in visited:

        print(node, end=" ")

        visited.add(node)

        for neighbor in graph[node]:
            dfs(neighbor, graph, visited)

bfs("A", graph)

print()

dfs("A", graph)
```

---

## 💻 Commands Used

```bash
python3 bfs_dfs.py
```

---

## 📋 Validation

The following tasks were successfully completed:

- ✅ Graph represented using an adjacency list
- ✅ BFS implemented using `deque`
- ✅ DFS implemented using recursion
- ✅ Graph traversal completed successfully
- ✅ Expected traversal output verified

---

## 📚 Key Concepts

| Concept | Description |
|----------|-------------|
| Graph | A collection of nodes connected by edges |
| Adjacency List | A memory-efficient graph representation using dictionaries and lists |
| BFS (Breadth-First Search) | Traverses nodes level by level using a queue |
| DFS (Depth-First Search) | Traverses nodes deeply before backtracking using recursion or a stack |
| Queue | FIFO (First In, First Out) data structure used in BFS |
| Recursion | A programming technique where a function calls itself |

---

## 🌍 Real-World Applications

Graph traversal algorithms are widely used in:

- Network Discovery
- Routing Algorithms
- Shortest Path Finding
- Social Network Analysis
- Web Crawling
- Maze Solving
- Artificial Intelligence Search
- Cybersecurity Attack Path Analysis
- Dependency Analysis

---

## 📸 Screenshots

Include screenshots for:

- Complete Python source code
- Graph representation
- BFS execution output
- DFS execution output
- Terminal execution

---

## 📖 What I Learned

- How to represent graphs using adjacency lists.
- How Breadth-First Search (BFS) explores nodes level by level.
- How Depth-First Search (DFS) explores nodes recursively.
- How queues (`deque`) are used in BFS.
- How recursion simplifies DFS implementation.
- Why graph traversal algorithms are important in networking, AI, and cybersecurity.

---

## ✅ Conclusion

This lab demonstrated the implementation of **Breadth-First Search (BFS)** and **Depth-First Search (DFS)** using Python and adjacency lists. BFS utilized a queue to explore nodes level by level, while DFS relied on recursion to traverse each branch before backtracking. These traversal techniques are fundamental algorithms in computer science and play a critical role in **network routing, artificial intelligence, graph analysis, and cybersecurity tasks such as attack path discovery and network topology analysis**.
