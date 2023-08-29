<div align="center">
<h1> Hands-on Data Structure and Algorithmic Problem Solving</h1>
<h3> A 100% open source one-stop coding problem referring material! </a> <h3>
<br> DSA · Python · LeetCode · Principles · Problem patterns<br>
</div>

<hr>

## Contributing
The material is written by Celia Lyu (celialyu1024@gmail.com) and Ricky Zhang (ruiqizhang8279@outlook.com). Feel free to send us email to contribute contents. Before you start to improve the contents, it would be helpful to know the [high-level structure of the material](#about-this-material).

All contributors (with decent amount of contributions) will be listed as authors in the project.

<hr>

## About this material

In short, this material offers intermediate to advanced algorithm content, tailored to enhance the essential knowledge required for an engineer's role. The structure of the material: 
* **Data Structures**: These are the building blocks of our computational systems. Understanding them is vital as they lay the groundwork for more complex programming tasks, offering ways to organize, store, and access data efficiently.
* **Classical algorithms**: Our approach is about more than just understanding algorithms; it's about internalizing their core principles. By diving deep into a range of traditional problems, we build a reference database in our minds, allowing us to quickly draw parallels and solutions when faced with new challenges.

<hr>

## Rationale behind this material

Navigating the intricacies of data structures and algorithms can be daunting, especially when applying them in real-world engineering tasks. Yet, mastering them is essential for every engineer striving for excellence in their respective field.

At the core of computer science is a fusion of various disciplines. From enumerative combinatorics to linear algebra in computer vision, the essence lies in the application of these principles to solve genuine challenges. What drives progress in this field is not just rote learning, but a genuine passion for understanding and implementing these principles.

While numerous resources delve into algorithmic theories (Introduction to Algorithms, Algorithmic Problem Solving, and so on) or exclusively focus on interview preparation (Cracking the Coding Interview, Coding Interview Questions, etc.), there's a noticeable gap. Few materials bridge the foundational knowledge with its practical, on-the-job application. This material is designed to fill that void. It underscores principles, patterns, and real-world problem-solving, using algorithmic concepts.

It's essential to note that this material does NOT aim to be a shortcut for interview success or offer hiring insights. Instead, it seeks to illuminate the elegance of algorithmic problem-solving. It's about nurturing a deeper appreciation for software engineering, with interview-style questions serving merely as a practical framework to solidify our understanding.

<hr>

## For Readers

We're in the process of crafting a book now, which is inspired by and expanding upon the core concepts presented in this material.

Stay tuned and consider following us for upcoming updates.

## Data Structure
<hr>

### Array
A contiguous block of memory containing elements of the same type. Use an array when you have a fixed number of items and you want quick access to each item based on its position, like books on a numbered shelf. 

<p align="center">
  <img src="figures/ds_array_1.png" alt="array_1" width="500" height="140" title="Figure 1.1: Visualization of the Array Data Structure: Elements and Indices."/>
</p>

**Simple Example**

Think of a shelf in a bookstore. The shelf has specific spots for books, numbered from 1 to 100. If you know the number, you can directly reach out and grab the book from its exact location without having to search.

### Linked List

Elements are stored in nodes, and each node points to the next node, forming a chain.

- **Singly Linked List**: Each node has data and a pointer to the next node.
- **Doubly Linked List**: Each node has data and two pointers, one pointing to the next node and another pointing to the previous node.
- **Circular Linked List**: The last node in the list points back to the first node.

<p align="center">
  <img src="figures/ds_ll_1.png" alt="ll_1" width="500" height="210" title="Figure 1.2: Visualization of the Linked List Data Structure: Elements and Indices."/>
</p>

**Simple Example**

Imagine a scavenger hunt game where each hint card has a clue to the location of the next card. The first card leads you to the second, the second leads to the third, and so on until you find the treasure.



### Stack

A last-in-first-out (LIFO) data structure. Operations mainly include push (to add) and pop (to remove). Use a stack when you want quick access to the most recent item, like a pile of plates.

<p align="center">
  <img src="figures/ds_stack_1.png" alt="stack_1" width="400" height="230" title="Figure 1.3: Visualization of the Stack Data Structure: Elements and Indices."/>
</p>

**Simple Example**

Think of a stack of plates in a cafeteria. When a new plate is washed, it's placed on the top of the stack. When someone needs a plate, they take the one from the top, which is the last plate that was washed.

### Queue

A first-in-first-out (FIFO) data structure. Operations mainly include enqueue (to add) and dequeue (to remove). Use a queue when you need to maintain the order of arrival, like customers waiting in line.

<p align="center">
  <img src="figures/ds_queue_1.png" alt="queue_1" width="500" height="160" title="Figure 1.4: Visualization of the Queue Data Structure: Elements and Indices."/>
</p>

**Simple Example**

Picture a line of people at a movie theater ticket counter. The first person in line will be the first to buy a ticket and leave the line, while others wait their turn.


### Tree

A hierarchical structure with a root and nodes connected by edges.

- **Binary Search Trees (BST)**:
    
    A binary tree with the property that all nodes in the left subtree have values less than the node and all nodes in the right subtree have values greater than the node. BSTs are particularly useful when you want to store data that you'll need to retrieve, insert, or delete quickly, while maintaining order.

    **Simple Example**
    
    Imagine you run a library. When a book is borrowed or returned, you need a quick way to update the list. Also, you often want to find books with titles "before" or "after" a given title in alphabetical order. A BST would be a good choice because it can keep the book titles in order while allowing for quick updates and lookups.

<p align="center">
  <img src="figures/ds_BST_1.png" alt="BST_1" width="300" height="180" title="Figure 1.5: Visualization of the Binary Search Trees (BST) Data Structure: Elements and Indices."/>
</p>

- **Tries (or Prefix Trees)**:
    
    A tree for storing a dynamic set of strings. They are commonly used in scenarios involving large datasets of strings.
    
    A Trie is a tree-like data structure used to store a dynamic set of strings. The key characteristic is that the position of a node in this tree defines the key with which that node is associated. As a result, strings with common prefixes share the same path until the point their prefixes diverge.

    **Simple Example**
    
    You're designing the search functionality for a dictionary app. When a user starts typing "choc", you want to immediately suggest words like "chocolate", "chock", and "chock-full". A trie can help you do this efficiently since it can quickly narrow down the list of words based on the typed prefix.

  <p align="center">
  <img src="figures/ds_tries_1.png" alt="tries_1" width="500" height="350" title="Figure 1.6: Visualization of the Tries Data Structure: Elements and Indices."/>
</p>

- **Heaps**:
    
    A tree-based data structure used primarily in algorithms like heap sort. Heaps are used when you need frequent access to the 'largest' or 'smallest' element, without the need to sort the entire set of data.

    - **Max Heap**: For any given node, its value is always greater than or equal to the values of its children. This means the highest value is at the root.
    - **Min Heap**: For any given node, its value is always less than or equal to the values of its children, keeping the smallest value at the root.
      
    **Simple Example**
    
    You run a music streaming service, and you want to always recommend the top 10 most listened to songs. As songs get played, their counts change. A heap can help you keep track of the top songs efficiently. When a song is played, you can quickly update its count and its position in the top songs without having to rearrange everything.
 
    <p align="center">
  <img src="figures/ds_heap_1.png" alt="heap_1" width="450" height="280" title="Figure 1.7: Visualization of the Heap Data Structure: Elements and Indices."/>
</p>

### Graph

A set of nodes connected by edges. Can be directed (with arrows) or undirected.

**Simple Example**

Think of a social gathering where people are interacting with each other. You can use a graph data structure to keep track of who's talking to whom.

- **Adjacency Matrix**: A 2D array of size V x V where V is the number of vertices in a graph.

    <p align="center">
  <img src="figures/ds_am_1.png" alt="am_1" width="500" height="180" title="Figure 1.8: Visualization of the Adjacency Matrix Data Structure: Elements and Indices."/>
</p>
  
- **Adjacency List**: An array of lists. The size of the array is the number of vertices.

    <p align="center">
  <img src="figures/ds_al_1.png" alt="al_1" width="500" height="300" title="Figure 1.9: Visualization of the Adjacency List Data Structure: Elements and Indices."/>
</p>

### Matrix

A matrix is like a table or grid with rows and columns, where each cell in the grid contains a piece of data. Think of it like an Excel spreadsheet, where you have rows (often represented by numbers) and columns (often represented by letters). The spot where a particular row and column intersect is a cell, and you can store information in it.

  <p align="center">
  <img src="figures/ds_matrix_1.png" alt="al_1" width="500" height="160" title="Figure 1.10: Visualization of the Matrix Data Structure: Elements and Indices."/>
</p>

**Simple Example**
Imagine a big board, like a chessboard, but it can be as large as you want. Each individual square on this board is a place where you can write down a number or a piece of information. This entire board, with all its individual squares filled with data, is what we call a matrix in the world of computer science and mathematics.

### Hash Map / Hash Table

Used to store key-value pairs, allowing for quick storage and retrieval. They use a hash function to compute an index where an element will be stored. The real efficiency of a hash map comes from being able to quickly access the data you want without searching through everything.

**A Brief Introduction**

Imagine a massive room with many lockers. You have many books, each with a unique title, and you want a system that allows you to place each book in a specific locker so that whenever you need a particular book, you can find it instantly without checking every locker.

A "hash map" works in a similar fashion. It's like this room with lockers. The hash map takes the book title, processes it through a special function (called a "hash function"), and gives you a locker number. You then put the book in that locker or retrieve it from there when needed.

  <p align="center">
  <img src="figures/ds_hm_1.png" alt="hm_1" width="500" height="250" title="Figure 1.11: Visualization of the Hash Map Data Structure: Elements and Indices."/>
</p>

**Simple Example**

Let's say you have three books: "Harry Potter", "Moby Dick", and "Pride and Prejudice".

1. You want to store "Harry Potter". The hash function tells you to put it in locker #5.
2. Next, for "Moby Dick", the function points you to locker #23.
3. Lastly, "Pride and Prejudice" goes into locker #8.

Now, when you want to read "Moby Dick", instead of searching through every locker, the hash map directly tells you, "Look in locker #23!"

### Union Find

"Union Find" is a data structure used to keep track of disjoint sets (i.e., sets that have no element in common) and is particularly useful for certain problems that involve determining connected components in a network or ensuring the absence of cycles in a graph. 

It typically uses an array (or sometimes a tree structure) to represent each individual's group. Initially, each person is their own group. As people become acquainted, their group identities merge.

**Main Idea**

Union Find has two primary operations:

1. **Union**: When two individuals or groups decide to merge, you note down this merge event in the magical notebook. This is the "union" operation.
2. **Find**: If you ever want to check if two people are in the same group, you consult the notebook. This quick check is the "find" operation.

By repeatedly using these operations, you can determine which people are connected either directly (by shaking hands) or indirectly (knowing someone who knows someone).

  <p align="center">
  <img src="figures/ds_uf_1.png" alt="uf_1" width="400" height="260" title="Figure 1.12: Visualization of the Union Find Data Structure: Elements and Indices."/>
</p>

**Simple Example**
Imagine a room full of people where everyone is standing alone, and no one knows anyone else. The objective is to form groups (or teams) and find out if two people belong to the same group.

"Union Find" is like a magical notebook that keeps track of these groups. Whenever two people decide to team up (or even if two teams decide to merge into a larger team), you make a note in this notebook. And when you're curious about whether two people are in the same team, you can quickly check the notebook to get your answer.

**Real-world Applications**

Consider, for example, a network of computers. If you want to see if two computers are connected directly or indirectly, the "Union Find" structure can help. It's like quickly checking if two computers belong to the same network cluster.

*Note: everything is still in progress, so use it with caution.*

<hr>


## Algorithm
<hr>

### Two Pointers

### 


*Note: everything is still in progress, so use it with caution.*

<hr>

## Referring Resources and Materials

* https://www.geeksforgeeks.org/what-is-array/
* [https://devopedia.org/linked-list-data-structure]
* [https://www.programiz.com/dsa/stack]
* [https://www.javatpoint.com/data-structure-queue]
* [https://courses.engr.illinois.edu/cs225/sp2023/resources/bst/]
* [https://www.geeksforgeeks.org/trie-insert-and-search/]
* [https://www.geeksforgeeks.org/heap-data-structure/]
* [https://www.geeksforgeeks.org/add-and-remove-edge-in-adjacency-matrix-representation-of-a-graph/]
* [https://www.jomaclass.com/blog/graph-representation-edge-list-adjacency-matrix-and-adjacency-lists]
* [https://www.geeksforgeeks.org/sparse-matrix-representation/]
* [https://www.geeksforgeeks.org/hashing-data-structure/]
* [https://iq.opengenus.org/union-find/]
* []
* []
* []

## Feedback

If you have ideas to improve the material, about formatting, more contents, or correct the errors, do not hesitate to let me know.

<!-- Citation -->
To cite this content, please use:
<hr>
```bibtex
@misc{handsondsa,
    author       = {Xiaoxi Celia Lyu, Ruiqi Ricky Zhang},
    title        = {Hands-on Data Structure and Algorithmic Problem Solving},
    howpublished = {\url{https://github.com/CeliaXxLYU/DataStructure-Algorithm-Intro.git}},
    year         = {2023}
}
```
