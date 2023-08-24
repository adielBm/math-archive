## Binary heap

- Type of: **Nearly Complete [[Binary Tree]]** (by CRLS)
- **max heap property:** for every node $i$ other than the root, $A[\text{parent}(i)]\geq A[i]$

Theorems:
- The index $i$ of the $k$-greatest ($k\neq{1}$) element in max-heap is $2\leq{i}\leq{2}^{k}-1$ ^[the same for  $k$-smallest element in min-heap]
> #todo CHECK IT!!!! There are at most $\lceil{n}/{2^{h+1}}\rceil$ nodes of height $h$ in any $n$-element heap <sup>(6.3-3)</sup>

### Procedures (max heap)

| procedure                  | run time    | desc                                                            |
| -------------------------- | ----------- | --------------------------------------------------------------- |
| heapify(A, i)              | $O(h)$      | (the height of $A[i]$ is $h$)                                   |
| max-heapify(A, i)          | $O(\lg n)$  |                                                                 |
| build-max-heap(A)          | $O(n)$      |                                                                 |
| heap-maximum(A)            | $O(1)$      | returns the element of $A$ with the largest key                 |
| heap-extract-max(A)        | $O(\lg{n})$ | remove max and retrun it                                        |
| heap-increase-key(A,i,key) | $O(\lg{n})$ | increases the value of $i$ to new value $key$ (larger or equal) |
| max-heap-insert(A,key)     | $O(\lg{n})$ | insert $key$ to $A$                                             |

- in **min-heap** the procedures will be: *min-heapify, build-min-heap, heap-minimum, heap-extract-min, heap-decrease-key, min-heap-insert*

# Heap Sort

- sorting array $A$ in-place
- $\text{heap-sort}(A)=O(n \lg n)$ - 
