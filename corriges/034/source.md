# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td34-probabilites-II.pdf)

## Autocorrection A



```math
\mathbb E[(X-1)^2]=\frac1n\sum_{j=0}^{n-1}j^2=\boxed{\frac{(n-1)(2n-1)}6}.
```




```math
\mathbb E[e^X]=\frac1n\sum_{k=1}^ne^k=\boxed{\frac{e(e^n-1)}{n(e-1)}}.
```



## Autocorrection B

Pour $p>0$,


```math
\mathbb E\left[\frac1{X+1}\right]=\sum_{k=0}^n\frac1{k+1}\binom nkp^k(1-p)^{n-k}
```




```math
=\frac1{(n+1)p}\sum_{j=1}^{n+1}\binom{n+1}jp^j(1-p)^{n+1-j}=\boxed{\frac{1-(1-p)^{n+1}}{(n+1)p}}.
```


Pour $p=0$, $X=0$ presque sûrement et l'espérance vaut $1$.

## Exercice 1

### 1



```math
\mathbb P(X=k)=ck,\quad1=c\sum_{k=1}^6k=21c\Rightarrow\mathbb P(X=k)=k/21.
```




```math
\mathbb EX=\frac1{21}\sum_{k=1}^6k^2=\frac{91}{21}=\boxed{\frac{13}3}>\frac72.
```



### 2



```math
\mathbb P(Y=1/k)=k/21\quad(1\le k\le6),\qquad\mathbb EY=\sum_{k=1}^6\frac1k\frac k{21}=\boxed{\frac27}.
```



## Exercice 2

### 1



```math
|X-Y|=\mathbf1_{X\ne Y},\qquad\mathbb E|X-Y|=p(1-p)+(1-p)p=\boxed{2p(1-p)}.
```



### 2



```math
\mathbb E|X-Y|=\frac2{n^2}\sum_{1\le i<j\le n}(j-i)=\frac2{n^2}\sum_{d=1}^{n-1}d(n-d)=\boxed{\frac{n^2-1}{3n}}.
```



## Exercice 3

### 1



```math
\mathbb E[(-1)^X]=\sum_{k=0}^{2n}\binom{2n}k(-p)^k(1-p)^{2n-k}=\boxed{(1-2p)^{2n}}.
```



### 2



```math
Y=\frac X2-\frac{1-(-1)^X}{4}\Rightarrow\boxed{\mathbb EY=np-\frac{1-(1-2p)^{2n}}4}.
```



## Exercice 4

### 1

Les positions des $n$ boules noires forment une partie uniforme de taille $n$ de $\{1,\ldots,2n\}$.


```math
\boxed{\mathbb P(X=k)=\frac{\binom{k-1}{n-1}}{\binom{2n}n}\quad(n\le k\le2n).}
```



### 2



```math
k\binom{k-1}{n-1}=n\binom kn\Rightarrow\mathbb EX=\frac n{\binom{2n}n}\sum_{k=n}^{2n}\binom kn
```




```math
=\frac{n\binom{2n+1}{n+1}}{\binom{2n}n}=\boxed{\frac{n(2n+1)}{n+1}}.
```



## Exercice 5

### 1

Pour $\mathbb P(A)>0$,


```math
X\mathbf1_A=Y\mathbf1_A\Rightarrow\mathbb E[X\mid A]=\frac{\mathbb E[X\mathbf1_A]}{\mathbb P(A)}=\mathbb E[Y\mid A].
```



### 2



```math
S=\sum_{i=1}^nX_i\mathbf1_{N\ge i},\qquad X_i\perp\!\!\!\perp N.
```




```math
\mathbb ES=\sum_{i=1}^n\mathbb EX_i\,\mathbb P(N\ge i)=p\sum_{i=1}^n\mathbb P(N\ge i)=\boxed{p\mathbb EN}.
```



## Autocorrection C



```math
T=\sum_{j=1}^r\mathbf1_{\text{boule }j\text{ dans le tiroir }1},\qquad\boxed{\mathbb ET=r/n}.
```




```math
V=\sum_{i=1}^n\mathbf1_{\text{tiroir }i\text{ vide}},\qquad\boxed{\mathbb EV=n(1-1/n)^r}.
```



## Exercice 6



```math
N=\sum_{i=1}^nI_i,\qquad\mathbb EI_i=\frac{\binom{2n-2}{r-2}}{\binom{2n}r}=\frac{r(r-1)}{2n(2n-1)}.
```




```math
\boxed{\mathbb EN=\frac{r(r-1)}{2(2n-1)}.}
```



## Autocorrection D

### 1



```math
\mathbb P(M\le k)=\mathbb P(X\le k,Y\le k)=\boxed{\frac{k^2}{n^2}}\quad(0\le k\le n).
```



### 2



```math
\mathbb P(M=k)=\frac{k^2-(k-1)^2}{n^2}=\frac{2k-1}{n^2}.
```




```math
\mathbb EM=\frac1{n^2}\left(2\sum_{k=1}^nk^2-\sum_{k=1}^nk\right)=\boxed{\frac{(n+1)(4n-1)}{6n}}.
```



### 3



```math
N+M=X+Y\Rightarrow\mathbb EN=n+1-\mathbb EM=\boxed{\frac{(n+1)(2n+1)}{6n}}.
```



### 4



```math
\mathbb P(N\ge k)=\left(\frac{n-k+1}n\right)^2\Rightarrow\mathbb EN=\frac1{n^2}\sum_{j=1}^nj^2=\frac{(n+1)(2n+1)}{6n}.
```



### 5



```math
\mathbb EM^2=\frac1{n^2}\left(2\sum_{k=1}^nk^3-\sum_{k=1}^nk^2\right)=\frac{(n+1)(3n^2+n-1)}{6n}.
```




```math
\boxed{\operatorname{Var}M=\frac{(n^2-1)(2n^2+1)}{36n^2}.}
```



## Autocorrection E

### 1



```math
\mathbb P(X=k)=1/n,\qquad\mathbb P(Y=j\mid X=k)=\frac1k\mathbf1_{1\le j\le k}.
```



### 2



```math
\boxed{\mathbb P(Y=j)=\frac1n\sum_{k=j}^n\frac1k\quad(1\le j\le n).}
```




```math
\mathbb E[Y\mid X=k]=\frac{k+1}2\Rightarrow\boxed{\mathbb EY=\frac{n+3}4}.
```




```math
\mathbb E[Y^2\mid X=k]=\frac{(k+1)(2k+1)}6,
```




```math
\mathbb EY^2=\frac{2\mathbb EX^2+3\mathbb EX+1}6=\frac{4n^2+15n+17}{36}.
```




```math
\boxed{\operatorname{Var}Y=\frac{(n-1)(7n+13)}{144}.}
```



## Exercice 7



```math
a=\min X,\quad b=\max X,\quad m=\mathbb EX.
```




```math
(X-a)(b-X)\ge0\Rightarrow\mathbb EX^2\le(a+b)m-ab.
```




```math
\operatorname{Var}X\le(m-a)(b-m)=\frac{(b-a)^2}4-\left(m-\frac{a+b}2\right)^2\le\frac{(b-a)^2}4.
```


Si $a<b$, égalité si et seulement si


```math
X\in\{a,b\}\text{ p.s.},\quad m=(a+b)/2\iff\mathbb P(X=a)=\mathbb P(X=b)=1/2.
```


Si $a=b$, l'égalité est automatique.

## Exercice 8

### 1



```math
\boxed{\mathbb P(X=k)=\frac{\binom{k-1}{r-1}}{\binom nr}\quad(r\le k\le n).}
```




```math
\sum_{k=r}^n\mathbb P(X=k)=1\Rightarrow\boxed{\sum_{k=r}^n\binom{k-1}{r-1}=\binom nr.}
```



### 2



```math
\mathbb EX=\frac r{\binom nr}\sum_{k=r}^n\binom kr=\frac{r\binom{n+1}{r+1}}{\binom nr}=\boxed{\frac{r(n+1)}{r+1}}.
```



### 3



```math
k(k+1)\binom{k-1}{r-1}=r(r+1)\binom{k+1}{r+1},
```




```math
\mathbb E[X(X+1)]=\frac{r(r+1)\binom{n+2}{r+2}}{\binom nr}=\frac{r(n+1)(n+2)}{r+2}.
```




```math
\operatorname{Var}X=\mathbb E[X(X+1)]-\mathbb EX-(\mathbb EX)^2=\boxed{\frac{r(n+1)(n-r)}{(r+1)^2(r+2)}}.
```



## Exercice 9

### 1



```math
\boxed{\mathbb P(N=k)=\frac{\binom nk^2}{\binom{2n}n}\quad(0\le k\le n).}
```



### 2



```math
N=\sum_{i=1}^nI_i,\qquad\mathbb EI_i=\frac n{2n}=\frac12\Rightarrow\boxed{\mathbb EN=n/2}.
```



### 3



```math
i\ne j:\quad\mathbb E[I_iI_j]=\frac{n(n-1)}{2n(2n-1)}=\frac{n-1}{2(2n-1)}.
```




```math
\mathbb E[N(N-1)]=\sum_{i\ne j}\mathbb E[I_iI_j]=\frac{n(n-1)^2}{2(2n-1)}.
```




```math
\boxed{\operatorname{Var}N=\frac{n^2}{4(2n-1)}.}
```



## Exercice 10

### 1



```math
M=\text{position de la dernière rouge},\qquad X=2n-M.
```




```math
\boxed{\mathbb P(X=k)=\frac{\binom{2n-k-1}{n-1}}{\binom{2n}n}\quad(0\le k\le n).}
```



### 2

L'exercice 8 avec $(n,r)$ remplacé par $(2n,n)$ donne


```math
\mathbb EX=2n-\frac{n(2n+1)}{n+1}=\boxed{\frac n{n+1}}.
```



### 3



```math
\operatorname{Var}X=\operatorname{Var}M=\boxed{\frac{n^2(2n+1)}{(n+1)^2(n+2)}}.
```



## Autocorrection F

### (i)



```math
\begin{array}{c|cccc}
(u,v)&(0,0)&(1,1)&(1,-1)&(2,0)\\\hline
\mathbb P(U=u,V=v)&(1-p)^2&p(1-p)&p(1-p)&p^2
\end{array}
```



### (ii)



```math
\operatorname{Cov}(U,V)=\operatorname{Var}X-\operatorname{Var}Y=0.
```



### (iii)



```math
\mathbb P(U=0,V=1)=0,\quad\mathbb P(U=0)\mathbb P(V=1)=(1-p)^2p(1-p)>0.
```


$U$ et $V$ ne sont pas indépendantes.

## Exercice 11

### 1



```math
X\sim\mathcal B(n,p),\qquad\mathbb EX=np.
```




```math
\mathbb P(Y=k)=\binom nkp^kq^{n-k}+\frac{q^n}{n}\quad(1\le k\le n).
```




```math
\boxed{\mathbb EY=np+\frac{n+1}2q^n.}
```



### 2(a)–(b)

Pour les événements de probabilité non nulle,


```math
\mathcal L(Y\mid X=0)=\mathcal U(\{1,\ldots,n\}),\qquad\mathbb E[Y\mid X=0]=(n+1)/2,
```




```math
j\ge1:\quad\mathbb P(Y=j\mid X=j)=1,\qquad\mathbb E[Y\mid X=j]=j.
```



### 3(a)



```math
0<q<1,\quad a=npq^{n-1}>0.
```




```math
\mathbb P(X=1,Y=1)=a,\qquad\mathbb P(X=1)\mathbb P(Y=1)=a\left(a+\frac{q^n}n\right).
```


Or $\mathbb P(Y=2)>0$, donc $a+q^n/n=\mathbb P(Y=1)<1$ ; les deux quantités diffèrent.

### 3(b)



```math
XY=X^2\Rightarrow\mathbb E[XY]=npq+n^2p^2.
```




```math
\boxed{\operatorname{Cov}(X,Y)=npq\left(1-\frac{n+1}2q^{n-1}\right).}
```




```math
q_0=\left(\frac2{n+1}\right)^{1/(n-1)}\in(0,1)\Rightarrow\operatorname{Cov}(X,Y)=0.
```



### 3(c)

Pour $q=q_0$, les variables sont non corrélées, mais non indépendantes.

## Exercice 12

### 1



```math
\boxed{\mathbb EZ=0,\qquad\operatorname{Var}Z=\operatorname{Var}X+\operatorname{Var}Y=n/2.}
```



### 2



```math
n-Y\sim\mathcal B(n,1/2),\quad X\perp\!\!\!\perp(n-Y)\Rightarrow Z+n\sim\mathcal B(2n,1/2).
```




```math
\boxed{\mathbb P(Z=k)=2^{-2n}\binom{2n}{n+k}\quad(-n\le k\le n).}
```



### 3



```math
\operatorname{Cov}(X,Z)=\operatorname{Var}X-\operatorname{Cov}(X,Y)=n/4.
```


Pour $n\ge1$, cette covariance est non nulle : $X,Z$ ne sont pas indépendantes.

## Exercice 13



```math
\mu=\mathbb EX,\quad\nu=\mathbb EY,\quad\sigma^2=\operatorname{Var}X>0,\quad c=\operatorname{Cov}(X,Y).
```




```math
\mathbb E[(Y-aX-b)^2]=\operatorname{Var}Y-2ac+a^2\sigma^2+(\nu-a\mu-b)^2
```




```math
=\operatorname{Var}Y-\frac{c^2}{\sigma^2}+\sigma^2\left(a-\frac c{\sigma^2}\right)^2+(\nu-a\mu-b)^2.
```




```math
\boxed{a=\frac{\operatorname{Cov}(X,Y)}{\operatorname{Var}X},\qquad b=\mathbb EY-a\mathbb EX.}
```



## Exercice 14

Récurrence sur $n$. Pour $n=1$, $T\sim\mathcal B(p)$ :


```math
\operatorname{Cov}(f(T),g(T))=p(1-p)(f(1)-f(0))(g(1)-g(0))\ge0.
```


Pour l'hérédité, conditionnons par $T_n$ :


```math
\operatorname{Cov}(X,Y)=\mathbb E[\operatorname{Cov}(X,Y\mid T_n)]+\operatorname{Cov}(\mathbb E[X\mid T_n],\mathbb E[Y\mid T_n]).
```


Le premier terme est positif par récurrence : pour chaque valeur de $T_n$, les restrictions de $f,g$ sont croissantes. L'indépendance assure


```math
\mathbb E[f(T_1,\ldots,T_{n-1},1)]\ge\mathbb E[f(T_1,\ldots,T_{n-1},0)],
```


et la même inégalité pour $g$. Le second terme est positif par le cas $n=1$.

## Exercice 15

### 1



```math
\mathbb P(\mathbf1_{A_1}=\varepsilon_1,\ldots,\mathbf1_{A_n}=\varepsilon_n)=2^{-n}=\prod_{i=1}^n\frac12.
```


Les indicatrices sont indépendantes, de loi $\mathcal B(1/2)$.

### 2



```math
N=\sum_i\mathbf1_{A_i}\sim\mathcal B(n,1/2),\qquad\boxed{\mathbb EN=n/2,\quad\operatorname{Var}N=n/4.}
```



### 3



```math
T=\sum_{i=1}^ni\mathbf1_{A_i},\quad\boxed{\mathbb ET=\frac{n(n+1)}4},
```




```math
\boxed{\operatorname{Var}T=\frac14\sum_{i=1}^ni^2=\frac{n(n+1)(2n+1)}{24}.}
```



## Exercice 16

### 1



```math
\mathbb P(X_i=1)=\frac{\binom{2n-1}{n-1}}{\binom{2n}n}=\frac12\Rightarrow X_i\sim\mathcal B(1/2).
```



### 2



```math
\mathbb E[X_iX_j]=\frac{\binom{2n-2}{n-2}}{\binom{2n}n}=\frac{n-1}{2(2n-1)},
```




```math
\boxed{\operatorname{Cov}(X_i,X_j)=-\frac1{4(2n-1)}.}
```



### 3



```math
S=\sum_{i=1}^niX_i,\qquad\boxed{\mathbb ES=\frac{n(n+1)}4}.
```




```math
A=\sum_{i=1}^ni,\quad B=\sum_{i=1}^ni^2,\qquad\operatorname{Var}S=\frac B4-\frac{A^2-B}{4(2n-1)}
```




```math
=\frac{2nB-A^2}{4(2n-1)}=\boxed{\frac{n^2(n+1)(5n+1)}{48(2n-1)}}.
```



## Exercice 17

### 1



```math
X=\sum_{i=1}^nI_i,\quad\mathbb EI_i=1/n\Rightarrow\boxed{\mathbb EX=1}.
```



### 2

Pour $n\ge2$,


```math
i\ne j:\quad\mathbb E[I_iI_j]=\frac{(n-2)!}{n!}=\frac1{n(n-1)}.
```




```math
\mathbb E[X(X-1)]=1\Rightarrow\operatorname{Var}X=1+1-1=\boxed1.
```


Pour $n=1$, $X=1$ et $\operatorname{Var}X=0$.

## Autocorrection G



```math
X\le|X|\Rightarrow\mathbb EX\le\mathbb E|X|,
```




```math
(\mathbb E|X|)^2=(\mathbb E[|X|\cdot1])^2\le\mathbb EX^2\,\mathbb E1^2=\mathbb EX^2.
```



## Exercice 18



```math
\mathbb E[X/Y]=\mathbb EX\,\mathbb E[1/Y]=\mathbb EX\,\mathbb E[1/X].
```




```math
1=\left(\mathbb E[\sqrt X\,X^{-1/2}]\right)^2\le\mathbb EX\,\mathbb E[1/X].
```



## Exercice 19



```math
|\mathbb P(A\cap B)-\mathbb P(A)\mathbb P(B)|=|\operatorname{Cov}(\mathbf1_A,\mathbf1_B)|
```




```math
\le\sqrt{p(1-p)q(1-q)}\le\frac14.
```


Égalité si et seulement si


```math
p=q=1/2,\qquad\mathbf1_A-1/2=\pm(\mathbf1_B-1/2)\text{ p.s.}
```




```math
\boxed{\mathbb P(A)=\mathbb P(B)=1/2,\quad A=B\text{ p.s. ou }A=B^c\text{ p.s.}}
```



## Exercice 20

### 1



```math
\mathbb EX_n=2n,\qquad\boxed{\operatorname{Var}X_n=n.}
```



### 2



```math
\mathbb P(|X_n-2n|\ge n)\le\frac{\operatorname{Var}X_n}{n^2}=\frac1n\to0.
```



### 3



```math
1-\frac1n\le\mathbb P(|X_n-2n|\le n)\le1\Rightarrow\boxed{\lim\mathbb P(|X_n-2n|\le n)=1.}
```



### 4



```math
2^{-4n}x_n=\mathbb P(n\le X_n\le3n)\to1\Rightarrow\boxed{x_n\sim2^{4n}.}
```



## Exercice 21



```math
X_n=(T_1,\ldots,T_n),\quad T_i\text{ indépendantes de loi }\mathcal B(1/2),\quad\|X_n\|^2=\sum_iT_i.
```




```math
Z_n=\|X_n\|^2/n,\quad\mathbb EZ_n=1/2,\quad\operatorname{Var}Z_n=1/(4n).
```




```math
\left|\sqrt{Z_n}-\frac1{\sqrt2}\right|=\frac{|Z_n-1/2|}{\sqrt{Z_n}+1/\sqrt2}\le\sqrt2|Z_n-1/2|.
```




```math
\mathbb P\left(\left|\frac{\|X_n\|}{\sqrt n}-\frac1{\sqrt2}\right|\ge\varepsilon\right)\le\frac1{2n\varepsilon^2}\to0.
```



## Exercice 22

### 1

Le domaine correct est $s\ge0$. Pour $s>0$, l'inégalité de Markov donne


```math
\mathbb P(S_n/n\ge a)=\mathbb P(e^{sS_n}\ge e^{sna})\le e^{-nsa}\mathbb E[e^{sS_n}]=e^{-nsa}(1-p+pe^s)^n.
```


Pour $s=0$, le majorant vaut $1$.
La formule imprimée pour tout $s\in\mathbb R$ est fausse : avec $n=100$, $p=1/2$, $a=1/10$ et $s=-\ln9$, le majorant vaut $(5\cdot9^{1/10}/9)^{100}<1/2$, tandis que $\mathbb P(S_n\ge10)>1/2$.

### 2

Supposons $0<p<1$ et $0<a<1$.


```math
h(s)=\ln(1-p+pe^s)-as,\quad h'(s)=\frac{pe^s}{1-p+pe^s}-a,\quad h''(s)>0.
```


Si $a\le p$, le minimum sur $[0,+\infty)$ est $h(0)=0$.
Si $p<a<1$,


```math
e^{s_*}=\frac{a(1-p)}{p(1-a)},\qquad h(s_*)=-D(a\|p).
```




```math
\boxed{\mathbb P(S_n/n\ge a)\le e^{-nD(a\|p)}.}
```


Pour $a=1$, l'infimum vaut $p^n$, obtenu lorsque $s\to+\infty$. Pour $a>1$, l'infimum vaut $0$. Les cas $p=0,1$ sont déterministes.

### 3

Pour $0<q<p<1$,


```math
\frac\partial{\partial q}D(p\|q)=\frac{q-p}{q(1-q)},\qquad D(p\|p)=0.
```




```math
D(p\|q)=\int_q^p\frac{p-t}{t(1-t)}\,dt\ge4\int_q^p(p-t)\,dt=\boxed{2(p-q)^2}.
```


La même démonstration avec les bornes inversées donne cette inégalité pour tous $p,q\in(0,1)$.

### 4



```math
\mathbb P(S_n/n-p\ge\varepsilon)\le e^{-nD(p+\varepsilon\|p)}\le e^{-2n\varepsilon^2}
```


lorsque $p+\varepsilon\le1$ ; sinon la probabilité est nulle.
Appliquons le même résultat à $n-S_n\sim\mathcal B(n,1-p)$ :


```math
\mathbb P(p-S_n/n\ge\varepsilon)\le e^{-2n\varepsilon^2}.
```




```math
\boxed{\mathbb P(|S_n/n-p|\ge\varepsilon)\le2e^{-2n\varepsilon^2}.}
```


Les valeurs limites des divergences traitent les seuils $0$ et $1$.

## Exercice 23



```math
I_k=\mathbf1_{k\in X},\quad\mathbb EI_k=1/2.
```




```math
\boxed{\mathbb E|X|=\sum_{k=1}^n\mathbb EI_k=n/2,\qquad\mathbb E\left[\sum_{k\in X}k\right]=\frac12\sum_{k=1}^nk=\frac{n(n+1)}4.}
```



## Exercice 24

Pour la matrice imprimée $M$,


```math
\mathbb EM=0,\qquad\operatorname{Cov}(X_{ij},X_{k\ell})=\delta_{ik}\delta_{j\ell}.
```


La matrice de covariance de ses $n^2$ coefficients vaut $I_{n^2}$.

Pour le déterminant $D$ défini dans l'énoncé,


```math
D=\sum_{\sigma\in S_n}\varepsilon(\sigma)\prod_{i=1}^nX_{i,\sigma(i)}.
```




```math
\mathbb ED=\sum_\sigma\varepsilon(\sigma)\prod_i\mathbb EX_{i,\sigma(i)}=0.
```




```math
\mathbb ED^2=\sum_{\sigma,\tau}\varepsilon(\sigma)\varepsilon(\tau)\mathbb E\left[\prod_iX_{i,\sigma(i)}X_{i,\tau(i)}\right].
```


Si $\sigma\ne\tau$, un coefficient apparaît une seule fois : son espérance nulle annule le terme. Si $\sigma=\tau$, le produit vaut $1$.


```math
\boxed{\mathbb ED=0,\qquad\operatorname{Var}D=n!.}
```



## Exercice 25

### 1(a)

L'échange des positions $1,2$ est une bijection entre les permutations vérifiant $\Sigma(1)<\Sigma(2)$ et celles vérifiant l'inégalité inverse.


```math
\boxed{\mathbb P(\Sigma(1)<\Sigma(2))=1/2.}
```



### 1(b)



```math
\mathbb P(\Sigma(1)=1,\Sigma(2)=1)=0\ne1/n^2.
```


Les variables ne sont pas indépendantes.

### 1(c)



```math
\Sigma(1),\Sigma(2)\sim\mathcal U(\{1,\ldots,n\}),
```




```math
\boxed{\mathbb P(\Sigma(1)=a,\Sigma(2)=b)=\frac{\mathbf1_{a\ne b}}{n(n-1)}.}
```



### 1(d)



```math
\#\{(a,b):|a-b|=1\}=2(n-1)\Rightarrow\boxed{\mathbb P(|\Sigma(1)-\Sigma(2)|=1)=2/n.}
```



### 1(e)



```math
I=\sum_{i<j}\mathbf1_{\Sigma(i)>\Sigma(j)}\Rightarrow\boxed{\mathbb EI=\frac12\binom n2=\frac{n(n-1)}4.}
```



### 2



```math
F=\sum_i\mathbf1_{\Sigma(i)=i},\quad\mathbb EF=1,\quad\mathbb E[F(F-1)]=n(n-1)\frac{(n-2)!}{n!}=1.
```




```math
\boxed{\operatorname{Var}F=1.}
```



### 3



```math
L\ge k\iff\Sigma(1)<\cdots<\Sigma(k)\Rightarrow\mathbb P(L\ge k)=1/k!.
```




```math
\boxed{\mathbb P(L=k)=\frac1{k!}-\frac1{(k+1)!}\ (1\le k<n),\qquad\mathbb P(L=n)=1/n!.}
```




```math
\boxed{\mathbb EL=\sum_{k=1}^n\frac1{k!}.}
```



### 4(a)



```math
I_i=\mathbf1_{\Sigma(i)=\min(\Sigma(i),\ldots,\Sigma(n))},\quad\mathbb EI_i=\frac1{n-i+1}.
```


Pour $i<j$, conditionnellement à $I_i=1$, l'ordre relatif des valeurs aux positions $i+1,\ldots,n$ reste uniforme.


```math
\mathbb E[I_iI_j]=\frac1{(n-i+1)(n-j+1)}=\mathbb EI_i\mathbb EI_j.
```




```math
H_n=\sum_{k=1}^n1/k,\qquad\boxed{\mathbb ER_n=H_n,\quad\operatorname{Var}R_n=H_n-\sum_{k=1}^n1/k^2.}
```



### 4(b)

Le $X_n$ imprimé désigne ici $R_n$.


```math
H_n/\ln n\to1,\qquad\operatorname{Var}R_n\le H_n.
```


Pour $n$ assez grand, $|H_n/\ln n-1|\le\varepsilon/2$, donc


```math
\mathbb P\left(\left|\frac{R_n}{\ln n}-1\right|>\varepsilon\right)\le\mathbb P(|R_n-H_n|>\tfrac\varepsilon2\ln n)\le\frac{4H_n}{\varepsilon^2(\ln n)^2}\to0.
```



### 5(a)



```math
|C|=k,\qquad\#\{\sigma:C\text{ est un cycle}\}=(k-1)!(n-k)!.
```




```math
\boxed{\mathbb P(C\text{ est un cycle})=\frac{(k-1)!(n-k)!}{n!}=\frac1{k\binom nk}.}
```



### 5(b)

Pour $K$ taille du cycle contenant $1$, la partie formée par ses $K-1$ autres éléments est uniforme.


```math
\mathbb P(2\text{ dans le cycle de }1\mid K=k)=\frac{k-1}{n-1}.
```


La loi obtenue en 5(c) donne


```math
\boxed{\mathbb P(1,2\text{ dans le même cycle})=\frac1n\sum_{k=1}^n\frac{k-1}{n-1}=1/2.}
```



### 5(c)



```math
\mathbb P(K=k)=\binom{n-1}{k-1}\frac{(k-1)!(n-k)!}{n!}=\boxed{1/n}\quad(1\le k\le n).
```



## Exercice 26

Pour des variables à supports finis, soit $S=X(\Omega)\cup Y(\Omega)$ et, pour $a\in S$,


```math
L_a(T)=\prod_{\substack{b\in S\\b\ne a}}\frac{T-b}{a-b}.
```




```math
L_a(X)=\mathbf1_{X=a},\qquad L_a(Y)=\mathbf1_{Y=a}.
```


L'égalité des moments et la linéarité donnent


```math
\mathbb P(X=a)=\mathbb E[L_a(X)]=\mathbb E[L_a(Y)]=\mathbb P(Y=a).
```




```math
\boxed{X\sim Y.}
```


Sans l'hypothèse de support fini du cadre étudié, l'assertion générale est fausse. Par exemple, sur $(0,+\infty)$,


```math
f_\varepsilon(x)=\frac{e^{-(\ln x)^2/2}}{x\sqrt{2\pi}}\bigl(1+\varepsilon\sin(2\pi\ln x)\bigr),\qquad|\varepsilon|\le1.
```


Ces densités distinctes ont les mêmes moments : avec $t=\ln x$ et $k\in\mathbb N$,


```math
\int_0^\infty x^kf_\varepsilon(x)\,dx=e^{k^2/2},
```


car


```math
\int_{\mathbb R}e^{kt-t^2/2}\sin(2\pi t)\,dt=e^{k^2/2}\int_{\mathbb R}e^{-u^2/2}\sin(2\pi(u+k))\,du=0.
```



## Exercice 27

Pour $Z$ à support fini dans $\mathbb N$, $g_Z$ est un polynôme ; pour un support fini dans $\mathbb Z$, c'est un polynôme de Laurent.

### 1



```math
[X^k]g_Z=\mathbb P(Z=k).
```



### 2



```math
g_{Z_1+Z_2}=\sum_{j,k}\mathbb P(Z_1=j,Z_2=k)X^{j+k}
```




```math
=\left(\sum_j\mathbb P(Z_1=j)X^j\right)\left(\sum_k\mathbb P(Z_2=k)X^k\right)=g_{Z_1}g_{Z_2}.
```



### 3



```math
g_Z=\sum_{k=0}^n\binom nkp^k(1-p)^{n-k}X^k=\boxed{(1-p+pX)^n}.
```



### 4



```math
g_{Z_1+Z_2}=(1-p+pX)^{n_1+n_2}\Rightarrow\boxed{Z_1+Z_2\sim\mathcal B(n_1+n_2,p).}
```



### 5(a)

Les deux lancers sont supposés indépendants. Posons


```math
g_{Z_1}=XA(X),\qquad g_{Z_2}=XB(X),\qquad\deg A,\deg B\le5.
```


Si $T$ était uniforme sur $\{2,\ldots,12\}$,


```math
A(X)B(X)=\frac1{11}(1+X+\cdots+X^{10}).
```


Les termes extrêmes imposent $\deg A=\deg B=5$. Un polynôme réel de degré impair a une racine réelle, alors que


```math
1+x+\cdots+x^{10}>0\qquad(x\in\mathbb R),
```


car pour $x\ne1$ il vaut $(x^{11}-1)/(x-1)>0$, et pour $x=1$ il vaut $11$. Contradiction.

### 5(b)



```math
A(X)B(X)=\frac1{36}(1+X+\cdots+X^5)^2,
```




```math
1+X+\cdots+X^5=(X+1)(X^2+X+1)(X^2-X+1).
```


Les deux polynômes $A,B$ ont degré $5$, et leurs coefficients sont positifs ou nuls. Leurs facteurs irréductibles réels appartiennent à cette liste. Si


```math
A=c(X+1)^a(X^2+X+1)^b(X^2-X+1)^d,
```


alors $a,b,d\in\{0,1,2\}$ et $a+2b+2d=5$, donc $a=1$ et $b+d=2$.
Le choix $(b,d)=(0,2)$ est impossible, car


```math
(X+1)(X^2-X+1)^2=X^5-X^4+X^3+X^2-X+1
```


a des coefficients négatifs. Le choix $(b,d)=(2,0)$ imposerait le choix impossible $(0,2)$ pour $B$. Ainsi $b=d=1$ pour les deux facteurs.


```math
A(1)=B(1)=1\Rightarrow A=B=\frac16(1+X+\cdots+X^5).
```


Les deux dés sont équilibrés.
