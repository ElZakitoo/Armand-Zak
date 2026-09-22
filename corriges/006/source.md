# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td06-matrices.pdf)

## Autocorrection A

```math
(AB)_{ij}=\sum_ka_{ik}b_{kj},\qquad\text{(i) }AB=40I_4,\qquad\text{(ii) }AB=\operatorname{diag}(2,4,-2).
```

## Exercice 1

```math
v^Tv=\sum_{i=1}^nv_i^2=0\iff\forall i,\ v_i=0\iff v=0.
```

## Exercice 2

```math
(JMJ)_{ij}=\sum_{k,\ell=1}^nm_{k\ell}\Rightarrow\boxed{JMJ=\left(\sum_{k,\ell=1}^nm_{k\ell}\right)J.}
```

## Exercice 3

```math
E_{ij}E_{k\ell}=\delta_{jk}E_{i\ell}.
```

```math
\text{(i) }A=E_{11},\quad B=E_{21}\Rightarrow AB=0,\ BA=E_{21}\ne0.
```

```math
\text{(ii) }A=E_{11},\quad B=E_{22}\Rightarrow AB=BA=0,\ A\ne0,\ B\ne0.
```

## Exercice 4

### 1

```math
S(a,b)+S(c,d)=S(a+c,b+d),
```

```math
S(a,b)S(c,d)=S(ac-bd,ad+bc)=S(c,d)S(a,b).
```

### 2

```math
S(a,b)^T=S(a,-b),\qquad S(a,b)S(a,b)^T=(a^2+b^2)I_2.
```

### 3

```math
(a,b)\ne(0,0)\Rightarrow S(a,b)^{-1}=\frac1{a^2+b^2}S(a,-b).
```

```math
S(0,0)=0\Rightarrow\boxed{S(a,b)\in GL_2(\mathbb R)\iff a^2+b^2>0.}
```

### 4

```math
S(\cos\alpha,\sin\alpha)S(\cos\beta,\sin\beta)=S(\cos(\alpha+\beta),\sin(\alpha+\beta)).
```

```math
\boxed{S(\cos\theta,\sin\theta)^n=S(\cos(n\theta),\sin(n\theta))}\qquad(n\in\mathbb Z).
```

## Exercice 5

```math
Q(a,b)=\begin{pmatrix}a&b\\-\overline b&\overline a\end{pmatrix}.
```

### 1

```math
Q(a,b)+Q(c,d)=Q(a+c,b+d),
```

```math
Q(a,b)Q(c,d)=Q(ac-b\overline d,ad+b\overline c).
```

### 2

```math
Q(a,b)Q(\overline a,-b)=(|a|^2+|b|^2)I_2.
```

```math
\boxed{\mathbb H\cap GL_2(\mathbb C)=\mathbb H\setminus\{0\},\qquad Q(a,b)^{-1}=\frac{Q(\overline a,-b)}{|a|^2+|b|^2}\in\mathbb H.}
```

## Exercice 6

```math
X^2+X=J\Rightarrow XJ=JX.
```

```math
X=\begin{pmatrix}a&b\\c&d\end{pmatrix},\quad XJ=JX\Rightarrow c=b,\ d=a.
```

```math
X^2+X=J\iff a^2+b^2+a=1,\quad b(2a+1)=1.
```

```math
a,b\in\mathbb Z\Rightarrow(b,2a+1)=(1,1)\text{ ou }(-1,-1).
```

```math
\boxed{X=\begin{pmatrix}0&1\\1&0\end{pmatrix}\quad\text{ou}\quad X=\begin{pmatrix}-1&-1\\-1&-1\end{pmatrix}.}
```

## Exercice 7

```math
M=\underbrace{\frac{M+M^T}2}_{S}+\underbrace{\frac{M-M^T}2}_{A},\qquad S^T=S,\quad A^T=-A.
```

```math
M=S_1+A_1\Rightarrow M^T=S_1-A_1\Rightarrow S_1=S,\quad A_1=A.
```

## Exercice 8

```math
\operatorname{tr}(PQ)=\sum_{i,j}p_{ij}q_{ji}=\operatorname{tr}(QP).
```

```math
PQ-QP=I_n\Rightarrow0=\operatorname{tr}(PQ-QP)=n,\quad\bot\qquad(\mathbb K=\mathbb R\text{ ou }\mathbb C).
```

## Exercice 9

```math
(AB)^T=B^TA^T=BA\Rightarrow AB\in S_n(\mathbb R)\iff AB=BA.
```

## Exercice 10

```math
(AD-DA)_{ij}=(d_j-d_i)a_{ij}.
```

```math
AD=DA\iff\forall i\ne j,\ a_{ij}=0\iff A\text{ diagonale}.
```

## Exercice 11

Dimension corrigée : $A\in M_{n+1}(\mathbb K)$.

```math
AD=DA\iff(d_j-d_i)a_{ij}=0.
```

```math
\boxed{A=\operatorname{diag}(a_1,\ldots,a_{n-1},B),\quad a_i\in\mathbb K,\quad B\in M_2(\mathbb K).}
```

## Exercice 12

```math
AE_{kk}=E_{kk}A\quad(1\le k\le n)\Rightarrow A=\operatorname{diag}(a_1,\ldots,a_n).
```

```math
AE_{ij}=a_iE_{ij},\quad E_{ij}A=a_jE_{ij}\Rightarrow a_i=a_j.
```

```math
\boxed{A=\lambda I_n.}
```

## Exercice 13

```math
AA^T=A^TA\Rightarrow\sum_{j=1}^na_{1j}^2=\sum_{j=1}^na_{j1}^2=a_{11}^2\Rightarrow a_{1j}=0\quad(j>1).
```

```math
A=\operatorname{diag}(a_{11},B),\quad B\text{ triangulaire supérieure},\quad BB^T=B^TB.
```

Récurrence sur $n$ : $B$, puis $A$, est diagonale.

## Exercice 14

```math
n=1:\quad\mathcal C=M_1(\mathbb K).
```

```math
n=2:\quad J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad AJ=JA\iff A=\begin{pmatrix}a&b\\-b&a\end{pmatrix}.
```

Pour $n\ge3$, soit $F_{ij}=E_{ij}-E_{ji}$.

```math
AF_{ij}=F_{ij}A\Rightarrow AF_{ij}^2=F_{ij}^2A,\qquad F_{ij}^2=-E_{ii}-E_{jj}.
```

Pour $i,j,k$ distincts,

```math
2E_{ii}=-(F_{ij}^2+F_{ik}^2-F_{jk}^2)\Rightarrow AE_{ii}=E_{ii}A.
```

```math
A=\operatorname{diag}(a_i),\quad AF_{ij}=F_{ij}A\Rightarrow a_i=a_j.
```

```math
\boxed{\mathcal C=\mathbb K I_n\quad(n\ge3).}
```

## Exercice 15

```math
AB=A+B\Rightarrow(A-I)(B-I)=I.
```

```math
A-I\text{ et }B-I\text{ inversibles}\Rightarrow(B-I)(A-I)=I\Rightarrow BA=A+B=AB.
```

## Autocorrection B

```math
s=\sin x,\quad c=\cos x,\qquad A^2=\begin{pmatrix}-c^2&-sc&c\\-sc&-s^2&s\\-c&-s&1\end{pmatrix},\qquad A^3=0.
```

```math
\boxed{(I_3+A)^m=I_3+mA+\frac{m(m-1)}2A^2}\qquad(m\in\mathbb Z).
```

Pour $m\ge0$, binôme de Newton ; pour $m<0$, $(I+A)^{-1}=I-A+A^2$ et récurrence descendante.

## Exercice 16

L'exposant est noté $m\ge1$.

### (i)

```math
(aI_n)^m=a^mI_n.
```

### (ii)

```math
A^2=2A\Rightarrow A^m=2^{m-1}\begin{pmatrix}1&-1\\-1&1\end{pmatrix}.
```

### (iii)

```math
\begin{pmatrix}1&1\\0&2\end{pmatrix}^m=\begin{pmatrix}1&\sum_{j=0}^{m-1}2^j\\0&2^m\end{pmatrix}=\begin{pmatrix}1&2^m-1\\0&2^m\end{pmatrix}.
```

### (iv)

```math
P=\frac12\begin{pmatrix}1&1\\1&1\end{pmatrix},\quad Q=I-P,\quad P^2=P,\ Q^2=Q,\ PQ=QP=0.
```

```math
A=3P-Q\Rightarrow\boxed{A^m=\frac12\begin{pmatrix}3^m+(-1)^m&3^m-(-1)^m\\3^m-(-1)^m&3^m+(-1)^m\end{pmatrix}.}
```

### (v)

```math
A=aI+bE_{12},\quad E_{12}^2=0\Rightarrow A^m=a^mI+ma^{m-1}bE_{12}.
```

Pour $m=1$, $A^1=A$ ; la formule vaut donc aussi lorsque $a=0$.

### (vi)

```math
A^m=\begin{pmatrix}\cos(m\theta)&-\sin(m\theta)\\\sin(m\theta)&\cos(m\theta)\end{pmatrix}.
```

### (vii)

```math
A^2=\begin{pmatrix}3&0&0&0\\0&1&1&1\\0&1&1&1\\0&1&1&1\end{pmatrix},\qquad A^3=3A.
```

```math
A^{2r+1}=3^rA\quad(r\ge0),\qquad A^{2r}=3^{r-1}A^2\quad(r\ge1).
```

### (viii)

```math
A=J_3-I_3,\quad P=J_3/3,\quad P^2=P.
```

```math
\boxed{A^m=2^mP+(-1)^m(I_3-P)=(-1)^mI_3+\frac{2^m-(-1)^m}{3}J_3.}
```

### (ix)

```math
P=J_n/n,\quad Q=I_n-P,\quad A=(a+(n-1)b)P+(a-b)Q.
```

```math
\boxed{A^m=(a-b)^mI_n+\frac{(a+(n-1)b)^m-(a-b)^m}{n}J_n.}
```

### (x)

```math
J_n^2=nJ_n\Rightarrow\boxed{J_n^m=n^{m-1}J_n.}
```

## Exercice 17

```math
\lambda=LC=\sum_{j=1}^n\ell_jc_j\in\mathbb C,\qquad(LC)^p=\lambda^p.
```

```math
(CL)^2=C(LC)L=\lambda CL\Rightarrow(CL)^p=\lambda^{p-1}CL\quad(p\ge1).
```

```math
(LC)^0=1,\qquad(CL)^0=I_n.
```

## Exercice 18

### 1

```math
Ae_1=e_2,\quad Ae_2=e_3,\quad Ae_3=e_4,\quad Ae_4=xe_1\Rightarrow A^4=xI_4.
```

### 2

```math
x=0\Rightarrow Ae_4=0\Rightarrow A\text{ non inversible}.
```

```math
x\ne0\Rightarrow A^{-1}=x^{-1}A^3.
```

### 3

```math
n=4q+r,\quad q\in\mathbb Z,\quad r\in\{0,1,2,3\}\Rightarrow\boxed{A^n=x^qA^r.}
```

```math
A^2=\begin{pmatrix}0&0&x&0\\0&0&0&x\\1&0&0&0\\0&1&0&0\end{pmatrix},\qquad A^3=\begin{pmatrix}0&x&0&0\\0&0&x&0\\0&0&0&x\\1&0&0&0\end{pmatrix}.
```

## Exercice 19

### 1

Le coefficient $(2,3)$ imprimé est $xz$. Pour $(x,y,z)=(1,0,1)$,

```math
A=\begin{pmatrix}1&0&1\\0&0&1\\1&0&1\end{pmatrix},\qquad\operatorname{rg}A=2>1.
```

La factorisation demandée est donc impossible en général. Avec $a_{23}=yz$,

```math
v=\begin{pmatrix}x\\y\\z\end{pmatrix},\qquad\widetilde A=vv^T.
```

### 2

```math
s=x^2+y^2+z^2,\qquad\boxed{\widetilde A^m=s^{m-1}\widetilde A\quad(m\ge1),\qquad\widetilde A^0=I_3.}
```

Pour la matrice imprimée, $d=z(x-y)$ :

```math
A=UV,\quad U=\begin{pmatrix}x&0\\y&1\\z&0\end{pmatrix},\quad V=\begin{pmatrix}x&y&z\\0&0&d\end{pmatrix},\quad H=VU=\begin{pmatrix}s&y\\dz&0\end{pmatrix}.
```

```math
\boxed{A^m=UH^{m-1}V\quad(m\ge1).}
```

```math
c=dyz,\quad H^2=sH+cI_2,\quad F_0=0,\ F_1=1,\ F_{r+1}=sF_r+cF_{r-1}.
```

```math
H^r=F_rH+cF_{r-1}I_2\quad(r\ge1),\qquad F_r=\sum_{j=0}^{\lfloor(r-1)/2\rfloor}\binom{r-1-j}{j}s^{r-1-2j}c^j\quad(r\ge1).
```

## Exercice 20

```math
B=\begin{pmatrix}\sin\theta&\cos\theta\\\cos\theta&-\sin\theta\end{pmatrix},\quad B^2=I_2,\quad P_\pm=\frac{I_2\pm B}2.
```

```math
P_\pm^2=P_\pm,\quad P_+P_-=0,\qquad A=xI_2+B=(x+1)P_++(x-1)P_-.
```

```math
\boxed{A^m=\frac{(x+1)^m+(x-1)^m}{2}I_2+\frac{(x+1)^m-(x-1)^m}{2}B}\quad(m\ge0).
```

Si $x\ne\pm1$, la formule vaut aussi pour $m\in\mathbb Z$.

## Exercice 21

### 1

```math
A=B+C,\quad A^2=B+2C,\quad A^3=B+3C\Rightarrow A^3-2A^2+A=0.
```

```math
A^{r+2}-2A^{r+1}+A^r=0\quad(r\ge1).
```

```math
A^{r+1}-A^r=A^2-A=C\Rightarrow A^r=A+(r-1)C=B+rC.
```

### 2

```math
B=\begin{pmatrix}1&0&0\\0&1&0\\0&0&0\end{pmatrix},\quad C=\begin{pmatrix}0&1&0\\0&0&0\\0&0&0\end{pmatrix},\quad A=B+C.
```

```math
B^2=B,\quad BC=CB=C,\quad C^2=0\Rightarrow A^r=B+rC\quad(r\ge1).
```

## Exercice 22

```math
A^p=0,\quad B^q=0,\quad AB=BA.
```

```math
(A+B)^{p+q-1}=\sum_{k=0}^{p+q-1}\binom{p+q-1}kA^kB^{p+q-1-k}=0,
```

car $k\ge p$ ou $p+q-1-k\ge q$.

```math
(AB)^p=A^pB^p=0.
```

Sans commutation :

```math
A=E_{12},\quad B=E_{21},\quad A^2=B^2=0,\quad(A+B)^2=I_2,\quad(AB)^m=E_{11}\ne0.
```

## Exercice 23

Pour $T$ strictement triangulaire supérieure,

```math
(T^r)_{ij}=\sum_{i=i_0<i_1<\cdots<i_r=j}t_{i_0i_1}\cdots t_{i_{r-1}i_r}.
```

```math
r=n\Rightarrow\{1\le i_0<\cdots<i_n\le n\}=\varnothing\Rightarrow T^n=0.
```

Le cas inférieur se déduit par transposition.

## Exercice 24

```math
A=J_3-I_3,\quad J_3^2=3J_3\Rightarrow A^2=J_3+I_3=A+2I_3.
```

```math
A\frac{A-I_3}2=I_3\Rightarrow\boxed{A^{-1}=\frac12\begin{pmatrix}-1&1&1\\1&-1&1\\1&1&-1\end{pmatrix}.}
```

## Exercice 25

```math
N=\sum_{i=1}^{n-1}E_{i,i+1},\quad N^n=0,\quad A=I+N+\cdots+N^{n-1}.
```

```math
(I-N)A=A(I-N)=I\Rightarrow\boxed{A^{-1}=I-\sum_{i=1}^{n-1}E_{i,i+1}.}
```

## Exercice 26

### 1

```math
M=(a-b)I+bJ,\quad J^2=nJ,\quad\alpha=a-b,\quad\beta=a+(n-1)b.
```

```math
\boxed{M^2=(\alpha+\beta)M-\alpha\beta I=(2a+(n-2)b)M-(a-b)(a+(n-1)b)I.}
```

### 2

```math
M\mathbf1=\beta\mathbf1,\quad M(e_1-e_2)=\alpha(e_1-e_2).
```

```math
\alpha\beta=0\Rightarrow\ker M\ne\{0\}.
```

```math
\alpha\beta\ne0\Rightarrow\boxed{M^{-1}=\frac{(\alpha+\beta)I-M}{\alpha\beta}=\frac1{a-b}I-\frac{b}{(a-b)(a+(n-1)b)}J.}
```

## Exercice 27

```math
\left(F\overline F\right)_{ij}=\sum_{k=0}^{n-1}\omega^{(i-j)k}=\begin{cases}n&i=j,\\\dfrac{1-\omega^{(i-j)n}}{1-\omega^{i-j}}=0&i\ne j.\end{cases}
```

```math
\boxed{F\overline F=nI_n,\qquad F^{-1}=\frac1n\overline F.}
```

## Exercice 28

### 1

Si la colonne $j$ de $A$ est nulle, alors, pour toute $B$, $(BA)_{ij}=\sum_kb_{ik}a_{kj}=0$. Ainsi $BA\ne I_n$.

```math
AE_{jj}=0=A0,\quad E_{jj}\ne0\Rightarrow A\text{ non simplifiable à gauche}\Rightarrow A\text{ non inversible}.
```

### 2

Si la ligne $i$ de $A$ est nulle, alors, pour toute $B$, $(AB)_{ij}=\sum_ka_{ik}b_{kj}=0$. Ainsi $AB\ne I_n$.

```math
E_{ii}A=0=0A,\quad E_{ii}\ne0\Rightarrow A\text{ non simplifiable à droite}.
```

```math
A^T\text{ possède une colonne nulle}\Rightarrow A^T\text{ non inversible}\Rightarrow A\text{ non inversible}.
```

## Exercice 29

### 1

```math
M\left(-\frac1{a_0}\sum_{k=1}^da_kM^{k-1}\right)=I_n.
```

```math
\boxed{M^{-1}=-\frac1{a_0}\sum_{k=1}^da_kM^{k-1}.}
```

### 2

```math
M=J_n-I_n,\quad M^2=(n-2)M+(n-1)I_n.
```

```math
n\ge2\Rightarrow\boxed{M^{-1}=\frac{M-(n-2)I_n}{n-1}=-I_n+\frac1{n-1}J_n.}
```

## Exercice 30

### 1

```math
(I-M)(I+M+\cdots+M^{p-1})=I-M^p=I.
```

```math
\boxed{(I-M)^{-1}=\sum_{k=0}^{p-1}M^k.}
```

### 2

```math
M=I-A=\begin{pmatrix}0&-3&1\\-3&0&2\\3&-6&0\end{pmatrix},\qquad M^2=\begin{pmatrix}12&-6&-6\\6&-3&-3\\18&-9&-9\end{pmatrix},\qquad M^3=0.
```

```math
\boxed{A^{-1}=I+M+M^2=\begin{pmatrix}13&-9&-5\\3&-2&-1\\21&-15&-8\end{pmatrix}.}
```

## Exercice 31

```math
A=L+D+U,\qquad D=\operatorname{diag}(a_{ii}).
```

$L$ strictement triangulaire inférieure, $U$ strictement triangulaire supérieure.

```math
\lambda\notin\{0,a_{11},\ldots,a_{nn}\},\qquad A=\underbrace{(U+\lambda I)}_{B}+\underbrace{(L+D-\lambda I)}_{C}.
```

```math
B,C\text{ triangulaires à diagonales non nulles}\Rightarrow B,C\in GL_n(\mathbb K).
```

