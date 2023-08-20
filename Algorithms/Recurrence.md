
- $T(n)=T(n/2)+\Theta(1)=O(\lg{n})$

- $T(n)=2T(n/2)+\Theta(1)=O(n)$

- $T(n)=2T(\lfloor{n/2}\rfloor)+\Theta(n)=O(n \lg n)$ 
- $T(n)=3T({n/2})+\Theta(n)=O(n^{\lg 3})$ 
- $T(n)=4T({n/2})+\Theta(n)=O(n^2)$ 


- $T(n)=2T(n/2)+\Theta(n)=\Theta(n \lg n)$

- $T(n)=T(n-1)+n=O(n^2)$
- $T(n)=2T(n/2+17)+n=O(n\lg{n})$
- $T(n)=2T(n/3)+\Theta(n)=\Theta(n)$



## Master Theorem
$$\large T(n)=aT(n/b)+f(n)$$
1. if $f(n)=O(n^{\log_{b}a-\epsilon})$ for some constant $\epsilon>0$, then $T(n)=\Theta(n^{\log _{b}a})$
	- $T(n)=4T(n/2)+\Theta(n)=\Theta(n^{\log_{2}4})=\Theta(n^2)$
	- $T(n)=9T(n/3)+n=\Theta(n^{\log_{3}9})=\Theta(n^2)$
2. if $f(n)=\Theta(n^{\log_{b}a})$, then $T(n)=\Theta(n^{\log_{b}a}\lg{n})$
	- $T(n)=T(2n/3)+1=\Theta(n^{\log _{2/3}1}\lg{n})=\Theta(n^{0}\lg{n})=\Theta(\lg{n})$
3. if $f(n)=\Omega(n^{\log_{b}a+\epsilon})$ for some constant $\epsilon>0$, and if $af(n/b)\leq cf(n)$ for some constant $c<1$ and all sufficiently large $n$, then $T(n)=\Theta(f(n))$ 
	- $T(n)=4T(n/3)+n\lg n=\Theta(n \lg  n)$

