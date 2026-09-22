# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td04-sommes-produits.pdf)

## Autocorrection A

### 1

$$a_0=S_0,\qquad a_n=S_n-S_{n-1}\quad(n\ge1).$$

### 2

$$\text{(i) }S_{n+1};\quad\text{(ii) }S_{2n}-S_n;\quad\text{(iii) }2S_n;\quad\text{(iv) }S_n-n-1;\quad\text{(v) }S_n-\frac{n(n+1)}2.$$

## Exercice 1

$$
\begin{aligned}
\text{(i)}\quad&\sum_{k=0}^n(-1)^k=\frac{1-(-1)^{n+1}}2;\\
\text{(ii)}\quad&\sum_{k=2}^{n+1}k=\frac{(n+1)(n+2)}2-1;\\
\text{(iii)}\quad&\sum_{k=1}^n2k=2\frac{n(n+1)}2=n(n+1);\\
\text{(iv)}\quad&\sum_{k=n+1}^{2n}2k=2n(2n+1)-n(n+1)=n(3n+1);\\
\text{(v)}\quad&\sum_{k=0}^n2^k=2^{n+1}-1;\\
\text{(vi)}\quad&\sum_{k=n+1}^{2n}2^k=2^{2n+1}-2^{n+1};\\
\text{(vii)}\quad&\sum_{k=0}^{2n}(-1)^kk=\sum_{j=1}^n(2j-(2j-1))=n;\\
\text{(viii)}\quad&\sum_{k=0}^n(-1)^{n-k}=\sum_{j=0}^n(-1)^j=\frac{1+(-1)^n}2.
\end{aligned}
$$

## Exercice 2

$$\sum_{k=1}^n(x_k-\xi)=0\iff\sum_{k=1}^nx_k=n\xi\iff\boxed{\xi=\frac1n\sum_{k=1}^nx_k.}$$

## Exercice 3

$$\sum_{p=1}^n\ln\left(1+\frac1p\right)=\sum_{p=1}^n(\ln(p+1)-\ln p)=\ln(n+1).$$
$$\sum_{k=0}^nkk!=\sum_{k=0}^n((k+1)!-k!)=(n+1)!-1.$$
$$\sum_{k=2}^n\frac1{k^2-1}=\frac12\sum_{k=2}^n\left(\frac1{k-1}-\frac1{k+1}\right)=\frac34-\frac1{2n}-\frac1{2(n+1)}\quad(n\ge1).$$
Pour $n=0$, la somme vide vaut $0$.

## Exercice 4

$$T_j=\sum_{k=0}^nk^j,\qquad(n+1)^4=4T_3+6T_2+4T_1+n+1.$$
$$T_1=\frac{n(n+1)}2,\qquad T_2=\frac{n(n+1)(2n+1)}6.$$
$$4T_3=(n+1)^4-n(n+1)(2n+1)-2n(n+1)-(n+1)=n^2(n+1)^2.$$
$$\boxed{T_3=\frac{n^2(n+1)^2}{4}.}$$

## Exercice 5

$$
\begin{aligned}
\text{(i)}&\quad(n^2-n)^{2001};\\
\text{(ii)}&\quad2^nn!;\\
\text{(iii)}&\quad(n!)^2;\\
\text{(iv)}&\quad\left(\frac{(2n)!}{n!}\right)^2;\\
\text{(v)}&\quad\frac{(2n+1)!}{2^nn!};\\
\text{(vi)}&\quad\exp\left(-\sum_{k=0}^nk\right)=e^{-n(n+1)/2};\\
\text{(vii)}&\quad2^{\sum_{k=0}^nk}=2^{n(n+1)/2};\\
\text{(viii)}&\quad\prod_{k=2}^n\frac{k-1}k=\frac1n\quad(n\ge1);\\
\text{(ix)}&\quad\prod_{k=2}^n\frac{k-1}k\frac{k+1}k=\frac{n+1}{2n}\quad(n\ge1);\\
\text{(x)}&\quad\frac{(n+2)!}{2n!}=\frac{(n+1)(n+2)}2;\\
\text{(xi)}&\quad\prod_{k=1}^n(2k-1)(2k+1)=\frac{(2n)!(2n+1)!}{2^{2n}(n!)^2};\\
\text{(xii)}&\quad\left(\prod_{k=1}^nk\right)\left(\prod_{k=1}^n(n+1-k)\right)=(n!)^2.
\end{aligned}
$$
Pour $n=0$, les produits (viii) et (ix) valent $1$.

## Exercice 6

$$A=\prod_{i=1}^ku_i,\quad B=\prod_{j=k+1}^nu_j,\qquad u_i\le u_j\quad(i\le k<j).$$
$$\prod_{i=1}^k\prod_{j=k+1}^nu_i\le\prod_{i=1}^k\prod_{j=k+1}^nu_j\Rightarrow A^{n-k}\le B^k.$$
$$A^n\le A^kB^k=(AB)^k.$$

## Exercice 7

$$\frac{a^n-1}{a-1}=\sum_{k=0}^{n-1}a^k\le\sum_{k=0}^{n-1}a^{n-1}=na^{n-1}.$$

## Exercice 8

### 1

$$S_{n+1}=S_n+(n+1)q^{n+1},$$
$$S_{n+1}=q\sum_{j=0}^n(j+1)q^j=qS_n+q\frac{1-q^{n+1}}{1-q}.$$
$$\boxed{S_n=\frac{q-(n+1)q^{n+1}+nq^{n+2}}{(1-q)^2}.}$$

### 2

$$(q-1)S_n=nq^{n+1}-\sum_{k=1}^nq^k=nq^{n+1}-\frac{q-q^{n+1}}{1-q}.$$
La division par $q-1$ donne la même expression.

### 3

$$\sigma(x)=\frac{1-x^{n+1}}{1-x},\qquad\sigma'(x)=\frac{1-(n+1)x^n+nx^{n+1}}{(1-x)^2}.$$
$$S_n=q\sigma'(q)=\frac{q-(n+1)q^{n+1}+nq^{n+2}}{(1-q)^2}.$$

## Autocorrection B

$$\sum_{k=0}^n(-1)^k\binom nk=(1-1)^n=\begin{cases}1&n=0,\\0&n\ge1,\end{cases}$$
$$\sum_{k=0}^n\frac{(-1)^k}{2^k}\binom nk=(1-\tfrac12)^n=2^{-n},\qquad\sum_{k=0}^n2^{2k}\binom nk=(1+4)^n=5^n.$$

## Exercice 9

$$P(X)=\frac{X^5}5+\frac{X^4}2+\frac{X^3}3-\frac X{30},\qquad P(0)=0,$$
$$P(n)-P(n-1)=n^4\Rightarrow P(n)=\sum_{k=1}^nk^4\in\mathbb N.$$

## Exercice 10

$$E+O=\sum_{k=0}^n\binom nk=2^n,\qquad E-O=\sum_{k=0}^n(-1)^k\binom nk=0.$$
$$\boxed{E=O=2^{n-1}.}$$

## Exercice 11

$$\binom nk\binom{n-k}{p-k}=\frac{n!}{k!(p-k)!(n-p)!}=\binom np\binom pk.$$
$$\boxed{\sum_{k=0}^p\binom nk\binom{n-k}{p-k}=2^p\binom np.}$$
Il manque $\binom np$ dans la première égalité imprimée : $n=2,p=1$ donne $4\ne2$.
$$p\ge1\Rightarrow\sum_{k=0}^p(-1)^k\binom nk\binom{n-k}{p-k}=\binom np(1-1)^p=0.$$

## Exercice 12

$$A_n=\sum_{k\ge0}\binom{n-k}{k},\qquad\binom ab=0\quad\text{si }(a,b)\in\mathbb Z^2\text{ et }0\le b\le a\text{ est faux}.$$
$$A_0=A_1=1,\qquad A_n=\sum_{k\ge0}\binom{n-1-k}{k}+\sum_{k\ge1}\binom{n-1-k}{k-1}=A_{n-1}+A_{n-2}\quad(n\ge2).$$
$$\boxed{A_n=F_{n+1}.}$$

## Exercice 13

$$S_0=S_1=1,$$
$$S_n=\sum_{k\ge0}(-1)^k\binom{n-1-k}{k}+\sum_{k\ge1}(-1)^k\binom{n-1-k}{k-1}=S_{n-1}-S_{n-2}\quad(n\ge2).$$
$$S_{n+3}=-S_n,\qquad S_{n+6}=S_n.$$
$$\boxed{(S_{6m},\ldots,S_{6m+5})=(1,1,0,-1,-1,0).}$$

## Exercice 14

### 1

$$\binom{2p+2}{p+1}=\frac{2p+2}{p+1}\binom{2p+1}{p+1}=2\binom{2p+1}{p+1}.$$

### 2

$$S_{n+1}=\sum_{k=0}^{n+1}\frac{\binom{n+k}{k}+\binom{n+k}{k-1}}{2^k}$$
$$=S_n+\frac{\binom{2n+1}{n+1}}{2^{n+1}}+\frac12\left(S_{n+1}-\frac{\binom{2n+2}{n+1}}{2^{n+1}}\right)=S_n+\frac12S_{n+1}.$$
$$S_{n+1}=2S_n,\quad S_0=1\Rightarrow\boxed{S_n=2^n.}$$

## Exercice 15

### 1

$$\frac{\binom n{k+1}}{\binom nk}=\frac{n-k}{k+1}.$$
$$\binom n{k+1}\begin{cases}>\binom nk&2k<n-1,\\=\binom nk&2k=n-1,\\<\binom nk&2k>n-1.\end{cases}$$

### 2

$$2^{2n}=\sum_{k=0}^{2n}\binom{2n}k\le(2n+1)\binom{2n}n\Rightarrow\binom{2n}n\ge\frac{2^{2n}}{2n+1}.$$

## Exercice 16

$$m\ge1\Rightarrow\prod_{j=0}^{k-1}(m+j)=k!\binom{m+k-1}k.$$
Si un facteur est nul, le produit est nul. Si tous sont négatifs,
$$\prod_{j=0}^{k-1}(m+j)=(-1)^k\prod_{j=0}^{k-1}(-m-j),$$
un produit de $k$ entiers positifs consécutifs au signe près.

## Exercice 17

### 1

$$\frac nk\binom{n-1}{k-1}=\frac{n!}{k!(n-k)!}=\binom nk.$$

### 2

$$n\ge1:\qquad\sum_{k=0}^nk\binom nk=n\sum_{j=0}^{n-1}\binom{n-1}j=n2^{n-1}.$$
La deuxième somme imprimée comporte $\binom{k}{n}$ :
$$\sum_{k=0}^nk2^k\binom{k}{n}=n2^n.$$
Avec $\binom nk$, la formule serait
$$\sum_{k=0}^nk2^k\binom nk=2n\sum_{j=0}^{n-1}2^j\binom{n-1}j=2n3^{n-1}.$$
Les deux sommes pondérées sont nulles pour $n=0$.
$$\sum_{k=0}^n\frac1{k+1}\binom nk=\frac1{n+1}\sum_{j=1}^{n+1}\binom{n+1}j=\frac{2^{n+1}-1}{n+1}.$$

## Exercice 18

### 1

$$\sum_{k=0}^n\binom nkx^k=(1+x)^n\Rightarrow\sum_{k=1}^nk\binom nkx^{k-1}=n(1+x)^{n-1}.$$
$$x=1\Rightarrow\sum_{k=0}^nk\binom nk=n2^{n-1}.$$

### 2

$$n\ge2:\qquad\sum_{k=0}^nk(k-1)\binom nk=n(n-1)2^{n-2}.$$
$$\sum_{k=0}^nk^2\binom nk=n(n-1)2^{n-2}+n2^{n-1}=\boxed{n(n+1)2^{n-2}}.$$
Pour $n=1$, la somme et la formule valent $1$.

## Exercice 19

### 1

$$\binom kp=\binom{k+1}{p+1}-\binom k{p+1}\Rightarrow\sum_{k=p}^n\binom kp=\binom{n+1}{p+1}.$$

### 2

$$\sum_{k=1}^nk(k+1)(k+2)=6\sum_{k=1}^n\binom{k+2}3=6\binom{n+3}4=\frac{n(n+1)(n+2)(n+3)}4.$$
$$k^3=6\binom k3+6\binom k2+\binom k1,$$
$$\sum_{k=0}^nk^3=6\binom{n+1}4+6\binom{n+1}3+\binom{n+1}2=\frac{n^2(n+1)^2}4.$$

## Exercice 20

$$A=\sum_{k=1}^nk=\frac{n(n+1)}2,\qquad B=\sum_{k=1}^nk^2=\frac{n(n+1)(2n+1)}6.$$
$$
\begin{aligned}
\text{(i)}&\quad\sum_{j=1}^nj=A;\\
\text{(ii)}&\quad nA=\frac{n^2(n+1)}2;\\
\text{(iii)}&\quad\sum_{j=1}^n\frac{j(j+1)}2=\frac{B+A}2=\frac{n(n+1)(n+2)}6;\\
\text{(iv)}&\quad\sum_{j=1}^n\left(\frac{j(j+1)}2+j^2\right)=\frac{3B+A}2=\frac{n(n+1)^2}2;\\
\text{(v)}&\quad2nB+2A^2=\frac{n^2(n+1)(7n+5)}6;\\
\text{(vi)}&\quad\frac12\left(A^2+B\right)=\frac{n(n+1)(n+2)(3n+1)}{24};\\
\text{(vii)}&\quad nA-nA=0;\\
\text{(viii)}&\quad\sum_{j=1}^n\left(j^2-\frac{j(j+1)}2\right)=\frac{B-A}2=\frac{n(n^2-1)}6;\\
\text{(ix)}&\quad2\sum_{1\le i\le j\le n}(j-i)=\frac{n(n^2-1)}3;\\
\text{(x)}&\quad\sum_{j=1}^n\left(\sum_{i=0}^j\binom ji-1\right)=\sum_{j=1}^n(2^j-1)=2^{n+1}-n-2;\\
\text{(xi)}&\quad\sum_{j=1}^n\frac1j\frac{j(j+1)}2=\frac{A+n}2=\frac{n(n+3)}4;\\
\text{(xii)}&\quad\sum_{j=1}^n\frac1j\frac{j(j+1)(2j+1)}6=\frac{2B+3A+n}6=\frac{n(4n^2+15n+17)}{36};\\
\text{(xiii)}&\quad\sum_{k=1}^nk(2k-1)=2B-A=\frac{n(n+1)(4n-1)}6;\\
\text{(xiv)}&\quad\sum_{k=1}^nk(2(n-k)+1)=(2n+1)A-2B=\frac{n(n+1)(2n+1)}6;\\
\text{(xv)}&\quad\left(\sum_{i=1}^n3^i\right)^2=\frac{9(3^n-1)^2}{4}.
\end{aligned}
$$

## Exercice 21

$$\text{(i)}\quad\prod_{1\le i,j\le n}x^{i+j}=x^{\sum_{i,j}(i+j)}=x^{n^2(n+1)}\quad(n\ge1).$$
$$\text{(ii)}\quad\prod_{j=1}^n\prod_{i=1}^ni^j=\prod_{j=1}^n(n!)^j=(n!)^{n(n+1)/2}.$$
$$\text{(iii)}\quad\prod_{i,j}ij=\left(\prod_i i^n\right)\left(\prod_jj^n\right)=(n!)^{2n}.$$
Pour $n=0$, les trois produits vides valent $1$.

## Exercice 22

$$m\in\{1,\ldots,n\}\Rightarrow m=\sum_{r=1}^n\mathbf1_{r\le m}.$$
$$\min(i,\max(j,k))\ge r\iff i\ge r\text{ et }(j\ge r\text{ ou }k\ge r).$$
$$\sum_{i,j,k=1}^n\min(i,\max(j,k))=\sum_{r=1}^n(n-r+1)(n^2-(r-1)^2).$$
$$=\sum_{s=0}^{n-1}(n-s)(n^2-s^2)=\frac{n^3(n+1)}2-\frac{n^2(n-1)(2n-1)}6+\frac{n^2(n-1)^2}4$$
$$\boxed{=\frac{n^2(n+1)(5n+1)}{12}.}$$

## Exercice 23

### 1

$$\sum_{0\le i<j\le n}i^p=\sum_{i=0}^n(n-i)i^p=nS_n^{(p)}-S_n^{(p+1)},$$
$$\sum_{0\le i<j\le n}i^p=\sum_{j=1}^n\sum_{i=0}^{j-1}i^p=\sum_{k=0}^{n-1}S_k^{(p)}.$$

### 2

$$nS_n^{(3)}-S_n^{(4)}=\frac14\sum_{k=0}^{n-1}(k^4+2k^3+k^2).$$
$$4nS_n^{(3)}-4S_n^{(4)}=S_n^{(4)}-n^4+2S_n^{(3)}-2n^3+S_n^{(2)}-n^2.$$
$$5S_n^{(4)}=(4n-2)\frac{n^2(n+1)^2}4+n^4+2n^3+n^2-\frac{n(n+1)(2n+1)}6.$$
$$\boxed{S_n^{(4)}=\frac{n(n+1)(2n+1)(3n^2+3n-1)}{30}.}$$

## Exercice 24

### 1

$$[1,n+1]^2=[1,n]^2\sqcup([1,n]\times\{n+1\})\sqcup(\{n+1\}\times[1,n])\sqcup\{(n+1,n+1)\},$$
où les intervalles désignent des intervalles d'entiers. La somme sur cette partition donne l'égalité demandée.

### 2

$$S_n=\left(\sum_{k=1}^nk\right)^2,$$
$$S_{n+1}-S_n=2(n+1)\sum_{k=1}^nk+(n+1)^2=n(n+1)^2+(n+1)^2=(n+1)^3.$$
$$S_0=0\Rightarrow S_n=\sum_{k=1}^nk^3=\left(\sum_{k=1}^nk\right)^2.$$

## Exercice 25

$$\left(\sum_ix_i\right)\left(\sum_jx_j^{-1}\right)-n^2=\sum_{i<j}\left(\frac{x_i}{x_j}+\frac{x_j}{x_i}-2\right)=\sum_{i<j}\frac{(x_i-x_j)^2}{x_ix_j}\ge0.$$
Égalité si et seulement si $x_1=\cdots=x_n$.

## Exercice 26

$$2n\sum_ka_kb_k-2\left(\sum_ia_i\right)\left(\sum_jb_j\right)=\sum_{i,j}(a_i-a_j)(b_i-b_j)\ge0.$$
$$\boxed{\frac1n\sum_ka_kb_k\ge\left(\frac1n\sum_ia_i\right)\left(\frac1n\sum_jb_j\right)}\qquad(n\ge1).$$

## Exercice 27

$$S(n+1)-S(n)=a_{n+1}\ge0.$$
$$S\text{ injective}\iff\forall n\ge1,\ a_n\ge1.$$
$$S\text{ surjective}\Rightarrow a_0=S(0)=0,\quad a_n\in\{0,1\}\ (n\ge1),\quad S(n)\to+\infty.$$
Réciproquement, ces conditions interdisent tout entier manquant entre deux valeurs consécutives de $S$, et $S$ est non bornée.
$$S\text{ surjective}\iff a_0=0,\quad\forall n\ge1,\ a_n\in\{0,1\},\quad\#\{n\ge1:a_n=1\}=+\infty.$$
$$\boxed{S\text{ bijective}\iff a_0=0\text{ et }\forall n\ge1,\ a_n=1.}$$

## Exercice 28

### 1(a)

$$\psi(A)=1\Rightarrow w_0=1.$$
$$T_k=\sum_{j=0}^kw_j,\qquad w_{k+1}>T_k+1\Rightarrow T_k+1\notin\psi(\mathcal P_f(\mathbb N)).$$
En effet, une somme utilisant un indice $>k$ dépasse $T_k+1$ ; les autres sont au plus $T_k$.

### 1(b)

$$\{0,1\}\subset\psi(\mathcal P(\{0\})).$$
$$[0,T_k]\cap\mathbb N\subset\psi(\mathcal P(\{0,\ldots,k\}))$$
$$\Rightarrow\bigl([0,T_k]\cup[w_{k+1},w_{k+1}+T_k]\bigr)\cap\mathbb N\subset\psi(\mathcal P(\{0,\ldots,k+1\})).$$
$$w_{k+1}\le T_k+1\Rightarrow[0,T_{k+1}]\cap\mathbb N\subset\psi(\mathcal P(\{0,\ldots,k+1\})).$$
$$T_k\ge k+1\to+\infty\Rightarrow\psi\text{ surjective}.$$

### 2

$$w_{k+1}\le T_k\Rightarrow\exists A\subset\{0,\ldots,k\},\quad\psi(A)=w_{k+1}=\psi(\{k+1\}),$$
ce qui contredit l'injectivité. Ainsi
$$w_{k+1}=T_k+1,\quad w_0=1\Rightarrow w_k=2^k.$$
Réciproquement, si $A\ne B$, soit $m=\max(A\triangle B)$ ; quitte à échanger $A,B$, $m\in A\setminus B$.
$$\psi(A)-\psi(B)\ge2^m-\sum_{j=0}^{m-1}2^j=1>0.$$
$$\boxed{\psi\text{ bijective}\iff\forall k,\ w_k=2^k.}$$
