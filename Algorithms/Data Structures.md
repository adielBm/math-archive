

- **dictionary** operations - insert, delete, search
- **dynamic set** operations - dictionary operations (insert, delete, search), minimun, maximum, successor, predecessor

____


# Hash Tables

### Hash function


### Collision resolution
- Chaining
- Open addressing
	- Linear probing
	- Quadratic probing
	- Double hashing


# Linked list


|                  |        | desc                                                |
| ---------------- | ------ | --------------------------------------------------- |
| list-insert(L,x) | $O(1)$ | insert x onto the front of the linked list                                                   |
| list-delete(L,x) | $O(1)$ | delete element x from the linked list                                                  |
| list-search(L,k) | $O(n)$ | returning a pointer to the first element with key k |


# Binary Search Tree (BST)

- Type of: [[Binary Tree]]
- Sorted data structure
- all **dynamic set operations** take $O(h)$ time
- **Traversal** (*Inorder*, *preorder*, and *postorder*) take $\Theta(n)$ time

- (12.4) The expected height of a **randomly built BST** on $n$ distinct keys is $O(\lg n)$

## Red-Black Tree (RB)

- Type of: BST

Red-Black tree properties:
- Every node is either **black** or **red**
- The **root** is black
- Every **leaf** (NIL) is black
- if node red, then both of its children are black (thus, red nodes $<$ black nodes)
- For each node, all simple paths from the node to leaves have the same number of black nodes, (limiting h ???)


- (13.1) A red-black tree with $n$ internal nodes has height at most $2\lg{(n+1)}$. (which means that it's **approximatly balanced**)

- **dynamic set operations** take $O(\lg{n})$ time


###  **Augmenting** a red-black tree 

- (Theorem 14.1) Let $f$ be a field that augments a red-black tree $T$ of $n$ nodes, and suppose that the contents of $f$ for a node $x$ can be computed using only the information in nodes $x$, $\text{left}[x]$, and $\text{right}[x]$, including $f[\text{left}[x]]$ and $f[\text{right}[x]]$. **Then**, we can maintain the values of $f$ in all nodes of $T$ during insertion and deletion without asymptotically affecting the $O(\lg n)$ performance of these operations. 


# Stack

- **LIFO**

|                |        | desc                                                             |
| -------------- | ------ | ---------------------------------------------------------------- |
| Push(S,x)      | $O(1)$ | adds an element to the collection                                |
| Pop(S)         | $O(1)$ | removes the most recently added element that was not yet removed |
| Stack-empty(S) | $O(1)$ |                                                                  |
| Top(S)         | $O(1)$ |                                                                  |


# Queue

- **FIFO**

|                |        | desc |
| -------------- | ------ | ---- |
| enqueue(Q,x)   | $O(1)$ | g    |
| dequeue(Q)     | $O(1)$ |      |
| queue-empty(Q) | $O(1)$ |      |
| queue-full(Q)  | $O(1)$ |      |

# deque

- (double-ended queue)


|                   |        | desc |
| ----------------- | ------ | ---- |
| head-enqueue(Q,x) | $O(1)$ | g    |
| tail-enqueue(Q,x) | $O(1)$ | g    |
| head-dequeue(Q)   | $O(1)$ |      |
| tail-dequeue(Q)   |        |      |