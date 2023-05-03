
## Binary heap

- The number $n$ of nodes in a heap of height $h$ is     $2^h\leq{n}\leq{2^{h+1}-1}$ 
- The height $h$ of $n$-element heap is    $h=\lfloor{\lg{n}}\rfloor$
- The number of leaves in heap is   $\lceil{n/2}\rceil$
- There are at most $\lceil{n}/{2^{h+1}}\rceil$ nodes of height $h$ in any $n$-element heap <sup>(6.3-3)</sup>
- The index $i$ of the $k$-greatest ($k\neq{1}$) element in max-heap is $2\leq{i}\leq{2}^{k}-1$ ^[the same for  $k$-smallest element in min-heap]
- the 

### run-time
- $\text{heapify}(A, i)=O(h)$.    (the height of $A[i]$ is $h$)
- $\text{max-heapify}(A, i)=O(\lg n)$
- $\text{heap-sort}(A)=O(n \lg n)$


