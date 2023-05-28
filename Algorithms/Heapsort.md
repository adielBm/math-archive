## Binary heap

- Binary heap is **Nearly Complete [[Binary Tree]]** (by CRLS) see its properties there.
- The index $i$ of the $k$-greatest ($k\neq{1}$) element in max-heap is $2\leq{i}\leq{2}^{k}-1$ ^[the same for  $k$-smallest element in min-heap]
- the

> #todo CHECK IT!!!! There are at most $\lceil{n}/{2^{h+1}}\rceil$ nodes of height $h$ in any $n$-element heap <sup>(6.3-3)</sup>

### run-time
- $\text{heapify}(A, i)=O(h)$.    (the height of $A[i]$ is $h$)
- $\text{max-heapify}(A, i)=O(\lg n)$
- $\text{heap-sort}(A)=O(n \lg n)$
- $\text{build-max-heap}(A)=O(n)$