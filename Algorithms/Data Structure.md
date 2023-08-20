
# Binary Search Tree (BST)

- Sorted data structure
- all **dynamic set operations** take $O(h)$ time
- **Traversal** (*Inorder*, *preorder*, and *postorder*) take $\Theta(n)$ time

- (12.4) The expected height of a **randomly built BST** on $n$ distinct keys is $O(\lg n)$

## Red-Black Tree (RB)

Red-Black tree properties:
- Every node is either **black** or **red**
- The **root** is black
- Every **leaf** (NIL) is black
- if node red, then both of its children are black (thus, red nodes $<$ black nodes)
- For each node, all simple paths from the node to leaves have the same number of black nodes, (limiting h ???)


- (13.1) A red-black tree with $n$ internal nodes has height at most $2\lg{(n+1)}$. (which means that it's **approximatly balanced**)

- **dynamic set operations** take $O(\lg{n})$ time

___


- **dictionary** operations - insert, delete, search
- **dynamic set** operations - dictionary operations (insert, delete, search), minimun, maximum, successor, predecessor
- 