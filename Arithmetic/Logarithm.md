$$\large \log_b{x}=y\quad\iff\quad b^a=y$$

- $0<b\neq 1$
- $0<x$
### Logarithmic identities

- Log of the Base    $\log_{b}b=1 {\color{gray}\impliedby b^1=b}$
- Log of Product   $\log_{b}({\color{red}x}{\color{blue}y})=\log_{b}{\color{red}x}+\log_{b}{\color{blue}y}$  
- Log of Quotient  $\log_{c}({\color{red}x}/{\color{blue}y})=\log_{b}{\color{red}x}-\log_{b}{\color{blue}y}$
- Log of Power     $\log_b{x^{\color{red}n}}={\color{red}n}\log_b{x}$
	- Log of One $\log_{b}1=0 {\color{gray}\impliedby b^0=1}$
- Log of the nth Root  $\log_{b}(\sqrt[n]{x})=\frac{\log_{b}x}{n}$           
- Change of Base     $\log_{\color{blue}b}{\color{red}x}=\frac{\log_c{\color{red}x}}{\log_c{\color{blue}b}}$ 
	- (special case $c=a$) Reciprocal of Logarithm - $\log_b{x}=\frac{1}{\log_x{b}}$ 
- Power of a Log ${\color{red}x}^{\log_b{\color{blue}y}}={\color{blue}y}^{\log_b{\color{red}x}}$ 
	- (special case $c=b$) $b^{\log_b{a}}=a$ 
- Logarithm of Reciprocal $\log_b{(1/a)}=-\log_b{a}$
- $\log_{b}{b^x}=x$ ($x \in \mathbb{R}$)
- $b^{\log_{b} x}=x$
- $b^{r\log_{b} x}=x^r$

# Binary logarithm 

- $\log_2{n}=\lg{n}$
- $(\lg{n})^{\lg{n}}=n^{\lg\lg{n}}$
- $2^{\lg\lg{n}}=\lg{n}$
- $2^{\lg{n}}={n^{\lg{2}}}={n^1}=n$
- $4^{\lg{n}}={n^{\lg{4}}}={n^2}$
- $4^{\lg{n}}={n^2}$
- $n^{1/\lg{n}}=2$
- $n^{1/\lg{n}}=2$
- $(n/2)\lg(n/2)\leq\lg{(n!)}\leq{n\lg{n}}$
	- $\implies\lg(n!)=\Theta{(n\lg{n})}$ ^[see CRLS: t8.1, e8.1-2]

>[!notation]
>- $\lg^{k}{n}=(\lg{n})^k$
> - $\lg^{(k)}{n}$
> 	- $\lg{\lg{n}}=\lg({\lg{n}})=\lg^{(2)}{n}$

# Natural Logarithm

- $\ln {x}:=\log _{e}{(x)}$
- $\ln(1)=0$
- $\ln(e)=1$
- $\ln({e^x})=x$
- $e^{\ln x}=x$
- $e^{r\ln x}=x^r$