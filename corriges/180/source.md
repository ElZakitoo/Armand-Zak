# corrigé zakito

[Énoncé](http://christophebertault.fr/documents/dm/DM%20-%20Iterations.pdf)

## 1

### a

```math
A=f^0(A)\subset B,\qquad f(B)=\bigcup_{n\ge0}f^{n+1}(A)\subset B.
```

### b

```math
A\subset C,\quad f(C)\subset C.
```

```math
f^0(A)\subset C,\qquad f^n(A)\subset C\Rightarrow f^{n+1}(A)\subset f(C)\subset C.
```

```math
\forall n\in\mathbb N,\quad f^n(A)\subset C\Rightarrow B\subset C.
```

## 2

```math
f^n(3)=3^{2^n},\qquad i\mapsto-1\mapsto1\mapsto1.
```

```math
\boxed{B=\{3^{2^n}:n\in\mathbb N\}\cup\{i,-1,1\}.}
```

## 3

### a

```math
f\in C^0(\mathbb R_+),\qquad 0\le x<y\Rightarrow f(y)-f(x)=\frac{(y-x)(x+y)}4>0.
```

```math
u_0=2,\quad v_0=4,\qquad u_{n+1}=\frac{u_n^2+3}4,\quad v_{n+1}=\frac{v_n^2+3}4.
```

```math
f^n(A)=[u_n,v_n]\Rightarrow f^{n+1}(A)=[f(u_n),f(v_n)]=[u_{n+1},v_{n+1}].
```

```math
\forall n\in\mathbb N,\quad f^n(A)=[u_n,v_n],\qquad0\le u_n\le v_n.
```

### b

```math
f(x)-x=\frac{(x-1)(x-3)}4,\qquad f(1)=1,\quad f(3)=3.
```

```math
1<u_n<3\Rightarrow1<u_{n+1}<u_n<3.
```

```math
u_n\downarrow\ell\in[1,2],\qquad\ell=f(\ell)\Rightarrow\ell\in\{1,3\}\Rightarrow\ell=1.
```

```math
v_n>3\Rightarrow v_{n+1}>v_n>3.
```

```math
v_n\uparrow L<+\infty\Rightarrow L\ge4,\quad L=f(L)\Rightarrow L\in\{1,3\},\quad\bot.
```

```math
\boxed{u_n\downarrow1,\qquad v_n\uparrow+\infty.}
```

### c

```math
[u_n,v_n]\subset(1,+\infty)\Rightarrow B\subset(1,+\infty).
```

```math
x>1\Rightarrow\exists N,M,\quad u_N<x,\quad v_M>x.
```

```math
n=\max(N,M)\Rightarrow x\in[u_n,v_n]\subset B.
```

```math
\boxed{B=(1,+\infty).}
```

## 4

```math
X=\bigcup_{n\ge0}f^n(E\setminus A)=(E\setminus A)\sqcup f(X),\qquad f(X)\subset A.
```

```math
E\setminus X\subset A,\qquad A=f(X)\sqcup(E\setminus X).
```

```math
\varphi(X)=f(X)\subset A,\qquad\varphi(E\setminus X)=E\setminus X\subset A.
```

```math
f_{|X}:X\longrightarrow f(X)\text{ bijective},\qquad\operatorname{id}_{E\setminus X}:E\setminus X\longrightarrow E\setminus X\text{ bijective}.
```

```math
\boxed{\varphi:E=X\sqcup(E\setminus X)\longrightarrow A=f(X)\sqcup(E\setminus X)\text{ bijective}.}
```

## 5

```math
u:E\hookrightarrow F,\qquad v:F\hookrightarrow E,\qquad A=v(F)\subset E.
```

```math
v\circ u:E\hookrightarrow A\overset{4}{\Longrightarrow}\exists b:E\xrightarrow{\sim}A.
```

```math
v:F\xrightarrow{\sim}A\Rightarrow\boxed{v^{-1}\circ b:E\xrightarrow{\sim}F.}
```

## 6

```math
\Phi(A,B)=2A\cup(2B+1).
```

```math
n\in A\iff2n\in\Phi(A,B),\qquad n\in B\iff2n+1\in\Phi(A,B).
```

```math
\Phi(A,B)=\Phi(C,D)\Rightarrow A=C,\quad B=D.
```

```math
\mathcal P(\mathbb N)^2\hookrightarrow\mathcal P(\mathbb N),\qquad A\mapsto(A,\varnothing):\mathcal P(\mathbb N)\hookrightarrow\mathcal P(\mathbb N)^2.
```

```math
\boxed{\mathcal P(\mathbb N)^2\simeq\mathcal P(\mathbb N).}
```

## 7

### a

```math
\alpha(f)=\alpha(g),\quad n\in\mathbb N\Rightarrow\exists m\in\mathbb N,\quad p_{n+1}^{f(n)+1}=p_{m+1}^{g(m)+1}.
```

```math
\text{Unicité de la décomposition en facteurs premiers}\Rightarrow m=n,\quad f(n)=g(n).
```

```math
\boxed{\alpha:\mathbb N^{\mathbb N}\hookrightarrow\mathcal P(\mathbb N).}
```

### b

```math
A\mapsto\mathbf1_A:\mathcal P(\mathbb N)\hookrightarrow\mathbb N^{\mathbb N}.
```

```math
\boxed{\mathbb N^{\mathbb N}\simeq\mathcal P(\mathbb N).}
```

## 8

### a

```math
x=\sigma^0(x)\Rightarrow x\sim x.
```

```math
y=\sigma^k(x)\Rightarrow x=\sigma^{-k}(y)\Rightarrow y\sim x.
```

```math
y=\sigma^k(x),\quad z=\sigma^\ell(y)\Rightarrow z=\sigma^{k+\ell}(x)\Rightarrow x\sim z.
```

### b

```math
m=|E|,\qquad x,\sigma(x),\ldots,\sigma^m(x)\in E.
```

```math
\exists0\le i<j\le m,\quad\sigma^i(x)=\sigma^j(x)\Rightarrow\sigma^{j-i}(x)=x.
```

```math
\{k\ge1:\sigma^k(x)=x\}\ne\varnothing\Rightarrow n(x)=\min\{k\ge1:\sigma^k(x)=x\}.
```

### c

```math
0\le i<j<n(x),\quad\sigma^i(x)=\sigma^j(x)\Rightarrow\sigma^{j-i}(x)=x,\quad0<j-i<n(x),\quad\bot.
```

```math
k\in\mathbb Z,\quad k=qn(x)+r,\quad0\le r<n(x)\Rightarrow\sigma^k(x)=\sigma^r(x).
```

```math
\boxed{[x]=\{x,\sigma(x),\ldots,\sigma^{n(x)-1}(x)\},\qquad|[x]|=n(x).}
```

## 9

### a

```math
x\in X_i\Rightarrow n(x)=n_i\Rightarrow\sigma_i^{n_i}(x)=\sigma^{n_i}(x)=x.
```

```math
x\notin X_i\Rightarrow\sigma_i^{n_i}(x)=x.
```

```math
\sigma_i^{n_i}=\operatorname{id}_E,\qquad\boxed{\sigma_i^{-1}=\sigma_i^{n_i-1}.}
```

### b

```math
i\ne j,\qquad X_i\cap X_j=\varnothing,\quad\sigma(X_i)=X_i,\quad\sigma(X_j)=X_j.
```

```math
\sigma_i\sigma_j(x)=\sigma_j\sigma_i(x)=\begin{cases}\sigma(x)&x\in X_i\cup X_j,\\x&x\notin X_i\cup X_j.\end{cases}
```

### c

```math
N=\operatorname{ppcm}(n_1,\ldots,n_r),\qquad E=\bigsqcup_{i=1}^rX_i.
```

```math
x\in X_i\Rightarrow N=q_in_i\Rightarrow\sigma^N(x)=(\sigma^{n_i})^{q_i}(x)=x.
```

```math
\boxed{\sigma^N=\operatorname{id}_E.}
```

## 10

### a

```math
E_k=f^k(E),\qquad E_{k+1}=f^k(f(E))\subset f^k(E)=E_k.
```

```math
|E_0|\ge|E_1|\ge\cdots\ge1\Rightarrow\exists p,\quad E_{p+1}=E_p.
```

```math
p=\min\{k\in\mathbb N:E_{k+1}=E_k\}\Rightarrow\forall k<p,\quad E_{k+1}\subsetneq E_k.
```

```math
E_{p+1}=E_p\Rightarrow\forall j\ge0,\quad E_{p+j}=f^j(E_p)=E_p.
```

### b

```math
F=E_p,\qquad f(F)=E_{p+1}=F\Rightarrow\sigma=f_{|F}:F\twoheadrightarrow F.
```

```math
F\text{ fini}\Rightarrow\sigma\text{ bijective}.
```

```math
k=\max(1,p)\Rightarrow\forall x\in E,\quad f^k(x)\in E_k=F.
```

