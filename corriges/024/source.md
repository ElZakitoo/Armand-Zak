# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td24-arithmetique-polynomes.pdf)

## Autocorrection A

### 1



```math
X^4\equiv-X^2\pmod{X^4+X^2},\qquad X^5\equiv-X^3,\quad X^6\equiv X^2,\quad X^7\equiv X^3.
```


Le reste est de degré au plus $3$ et dépend linéairement du dividende.


```math
f(1)=-1-X^2,\quad f(X)=-X-X^3,\quad f(X^2)=f(X^3)=0.
```




```math
\boxed{\operatorname{Mat}(f)=\begin{pmatrix}-1&0&0&0\\0&-1&0&0\\-1&0&0&0\\0&-1&0&0\end{pmatrix}.}
```



### 2



```math
\boxed{\operatorname{rg}f=2,\quad\ker f=\operatorname{Vect}(X^2,X^3),\quad\operatorname{im}f=\operatorname{Vect}(1+X^2,X+X^3).}
```



## Exercice 1



```math
M_P=P\mathbb K[X],\qquad\lambda PU+\mu PV=P(\lambda U+\mu V).
```


Pour $P\ne0$ de degré $d$,


```math
R=PQ+S,\quad\deg S<d\Rightarrow\boxed{\mathbb K[X]=M_P\oplus\mathbb K_{d-1}[X].}
```


Pour $d=0$, le supplémentaire est $\{0\}$ ; pour $P=0$, $M_P=\{0\}$ et le supplémentaire est $\mathbb K[X]$.

## Exercice 2



```math
P(X+a_i)=\sum_{k=0}^n\frac{a_i^k}{k!}P^{(k)}(X).
```


Les polynômes $P^{(k)}/k!$ ont des degrés distincts $n,n-1,\ldots,0$ et forment une base.
La matrice des polynômes translatés dans cette base est la matrice de Vandermonde $(a_i^k)_{0\le k,i\le n}$, de déterminant


```math
\prod_{0\le i<j\le n}(a_j-a_i)\ne0.
```



## Exercice 3



```math
\sum_{j=0}^{n-k-1}b_jX^j+\sum_{i=0}^kc_iP(X+i)=0.
```


Dans le quotient par $\mathbb R_{n-k-1}[X]$, les classes de $P,P',\ldots,P^{(k)}$ sont libres par leurs degrés distincts. Taylor donne donc


```math
\sum_{i=0}^kc_ii^r=0\quad(0\le r\le k).
```


Le déterminant de Vandermonde associé à $0,1,\ldots,k$ est non nul : $c_i=0$ pour tout $i$. Alors $b_j=0$ pour tout $j$.

## Autocorrection B



```math
P(1)=P'(1)=P''(1)=0,
```




```math
P'''(1)=(2n+1)\bigl(2n(2n-1)-n(n+1)(n-1)+n(n-1)(n-2)\bigr)
```




```math
=n(n+1)(2n+1)\ne0.
```




```math
\boxed{\mu_1(P)=3.}
```



## Exercice 4



```math
S_n=\sum_{k=0}^n\frac{X^k}{k!},\quad S_n'=S_{n-1},\quad S_n-S_n'=X^n/n!.
```




```math
S_n(z)=S_n'(z)=0\Rightarrow z=0,\qquad S_n(0)=1,\quad\bot.
```


Pour $n=0$, il n'y a pas de racine.

## Exercice 5



```math
P(1)=0,\qquad P(z)=0\Rightarrow nz^n=\sum_{k=0}^{n-1}z^k.
```


Si $|z|>1$,


```math
n|z|^n\le\sum_{k=0}^{n-1}|z|^k\le n|z|^{n-1}<n|z|^n,
```


contradiction. Si $|z|=1$ et $n\ge2$, l'égalité triangulaire impose que $1,z,\ldots,z^{n-1}$ aient le même argument, donc $z=1$. Pour $n=1$, $P=X-1$.


```math
Q=(X-1)P=nX^{n+1}-(n+1)X^n+1,\quad Q'=n(n+1)X^{n-1}(X-1).
```


Une racine multiple de $P$ différente de $1$ serait racine de $Q,Q'$, donc égale à $0$, mais $Q(0)=1$.


```math
P'(1)=n^2-\sum_{k=1}^{n-1}k=\frac{n(n+1)}2\ne0.
```



## Exercice 6

Par Rolle, $P'$ est simplement scindé sur $\mathbb R$.


```math
P(z)^2+1=0,\quad2P(z)P'(z)=0\Rightarrow P'(z)=0\Rightarrow z\in\mathbb R.
```


Mais $P(z)^2+1>0$ pour $z\in\mathbb R$. Aucune racine multiple.

## Exercice 7

Pour deux indices consécutifs $k,k+1\in\{0,\ldots,\deg P\}$,


```math
[X^k]P=[X^{k+1}]P=0\Rightarrow P^{(k)}(0)=P^{(k+1)}(0)=0.
```


Or $P^{(k)}$ est simplement scindé par Rolle ; il ne peut avoir une racine commune avec sa dérivée.

## Exercice 8



```math
\mu_z(P-a)\ge3\Rightarrow P'(z)=P''(z)=0.
```


Le polynôme $P'$ est simplement scindé ; cette situation est impossible. Pour $\deg P=1$, le résultat est immédiat.

## Exercice 9



```math
P=c\prod_{i=1}^r(X-a_i)^{m_i},\quad a_1<\cdots<a_r,\quad\sum_i m_i=n.
```


Dans $P'$, chaque $a_i$ a multiplicité $m_i-1$. Rolle donne au moins une racine dans chacun des $r-1$ intervalles $(a_i,a_{i+1})$.


```math
\sum_i(m_i-1)+(r-1)=n-1=\deg P'.
```


Toutes les racines intercalées sont simples ; toute racine multiple de $P'$ appartient donc à $\{a_1,\ldots,a_r\}$.

## Exercice 10

Pour $a=0$, Rolle donne le résultat. Pour $a\ne0$, soient $r_1<\cdots<r_n$ les racines de $P$ et


```math
h(x)=\frac{P'(x)}{P(x)}+a=\sum_{j=1}^n\frac1{x-r_j}+a.
```




```math
h'(x)=-\sum_j\frac1{(x-r_j)^2}<0.
```


Sur chaque $(r_j,r_{j+1})$, $h$ décroît de $+\infty$ à $-\infty$ : une racine simple. Si $a>0$, une racine supplémentaire appartient à $(-\infty,r_1)$ ; si $a<0$, elle appartient à $(r_n,+\infty)$.


```math
P'(r_j)+aP(r_j)=P'(r_j)\ne0.
```


Ces $n$ racines simples épuisent le degré $n$ de $P'+aP$.

## Exercice 11

### 1



```math
P=\prod_{j=1}^d(X-a_j),\quad a_j\in\mathbb R\Rightarrow|P(z)|=\prod_j|z-a_j|\ge|\operatorname{Im}z|^d.
```


Réciproquement, pour toute racine $z$ de $P$,


```math
0\ge|\operatorname{Im}z|^d\Rightarrow z\in\mathbb R.
```


Le cas $d=0$, $P=1$, est immédiat.

### 2

La convergence des coefficients donne $\deg P=d$, le coefficient dominant $1$, et $P_n(z)\to P(z)$ pour chaque $z$.


```math
|P(z)|=\lim_n|P_n(z)|\ge|\operatorname{Im}z|^d.
```


La première question s'applique.

## Exercice 12



```math
F=U+iV=c\prod_{j=1}^n(X-z_j),\quad\operatorname{Im}z_j=b_j>0.
```


Pour $x\in\mathbb R$, $F(x)\ne0$. Choisissons un argument continu $\theta(x)$ de $F(x)$.


```math
\theta'(x)=\operatorname{Im}\frac{F'(x)}{F(x)}=\sum_{j=1}^n\frac{b_j}{(x-\operatorname{Re}z_j)^2+b_j^2}>0.
```


Avec $\gamma=\arg c$, on peut choisir


```math
\theta(\mathbb R)=(\gamma-n\pi,\gamma).
```


Les zéros de $U$ correspondent aux niveaux $\theta=\pi/2+k\pi$, ceux de $V$ aux niveaux $\theta=k\pi$. Chaque niveau intérieur est atteint une fois, avec une dérivée non nulle.
Si $\operatorname{Re}c\ne0$, il y a $n$ niveaux de la première sorte, donc $n$ racines réelles de $U$, de degré $n$. Si $\operatorname{Re}c=0$, il y en a $n-1$, et $\deg U\le n-1$ ; ainsi toutes les racines de $U$ sont réelles. Le raisonnement est identique pour $V$, suivant que $\operatorname{Im}c$ est nul ou non.


```math
\boxed{U\text{ et }V\text{ sont scindés, même simplement scindés}.}
```



## Exercice 13

Viète appliqué à $X^n-1$ donne


```math
\boxed{\sum_{\omega^n=1}\omega=\begin{cases}1&n=1,\\0&n\ge2,\end{cases}\qquad\prod_{\omega^n=1}\omega=(-1)^{n+1}.}
```




```math
\sum\omega^2=\left(\sum\omega\right)^2-2\sum_{i<j}\omega_i\omega_j.
```


Le coefficient de $X^{n-2}$ vaut $0$ pour $n\ge3$, et vaut $-1$ pour $n=2$.


```math
\boxed{\sum_{\omega^n=1}\omega^2=\begin{cases}1&n=1,\\2&n=2,\\0&n\ge3.\end{cases}}
```



## Exercice 14



```math
P=a_nX^n+a_{n-1}X^{n-1}+\cdots,\quad P'=na_nX^{n-1}+(n-1)a_{n-1}X^{n-2}+\cdots.
```




```math
\frac1n\sum_{P(\alpha)=0}\alpha=-\frac{a_{n-1}}{na_n}=\frac1{n-1}\sum_{P'(\beta)=0}\beta,
```


les racines étant comptées avec multiplicité.

## Exercice 15



```math
P(a)=P(b)=0,\ a\ne b\Rightarrow(X-a)(X-b)\mid P.
```


Le quotient a degré $1$, donc une racine dans $\mathbb K$ ; $P$ est scindé.

## Exercice 16

### 1



```math
\boxed{x^2+y^2+z^2=\sigma_1^2-2\sigma_2,}
```




```math
\boxed{x^3+y^3+z^3=\sigma_1^3-3\sigma_1\sigma_2+3\sigma_3.}
```



### 2

Premier système :


```math
\sigma_1=1,\quad\sigma_3=-4,\quad\sigma_2/\sigma_3=1\Rightarrow\sigma_2=-4.
```




```math
T^3-\sigma_1T^2+\sigma_2T-\sigma_3=T^3-T^2-4T+4=(T-1)(T-2)(T+2).
```


Les solutions sont les six permutations de $(1,2,-2)$.

Second système :


```math
\sigma_1=2,\quad\sigma_2=(4-14)/2=-5,\quad20=8-3\cdot2\cdot(-5)+3\sigma_3\Rightarrow\sigma_3=-6.
```




```math
T^3-2T^2-5T+6=(T-1)(T-3)(T+2).
```


Les solutions sont les six permutations de $(1,3,-2)$.

## Exercice 17

### 1

La variable dans la formule est $\cot^2t$.


```math
\sin((2n+1)t)=\operatorname{Im}(\cos t+i\sin t)^{2n+1}
```




```math
=\sum_{j=0}^n(-1)^j\binom{2n+1}{2j+1}\cos^{2n-2j}t\sin^{2j+1}t.
```




```math
\boxed{P_n(Y)=\sum_{j=0}^n(-1)^j\binom{2n+1}{2j+1}Y^{n-j},\qquad P_n(\cot^2t)=\frac{\sin((2n+1)t)}{\sin^{2n+1}t}.}
```



### 2



```math
r_k=\cot^2\frac{k\pi}{2n+1}\quad(1\le k\le n)
```


sont $n$ racines distinctes. Viète donne


```math
\boxed{\sum_{k=1}^nr_k=\frac{\binom{2n+1}3}{2n+1}=\frac{n(2n-1)}3.}
```



### 3



```math
\sin t\le t\le\tan t\quad(0<t<\pi/2)\Rightarrow\cot^2t\le\frac1{t^2}\le1+\cot^2t.
```




```math
\frac{n(2n-1)}3\le\frac{(2n+1)^2}{\pi^2}\sum_{k=1}^n\frac1{k^2}\le n+\frac{n(2n-1)}3.
```




```math
\boxed{\zeta(2)=\pi^2/6.}
```



## Autocorrection C

### (i)–(ii)

Les deux polynômes de gauche s'annulent en $-1$, tandis que les seconds membres valent respectivement $1$ et $2$.


```math
\boxed{\text{Aucune solution dans les deux cas}.}
```



### (iii)



```math
U=X^2+2X+3,\quad V=X^2-X-3.
```


Une racine commune vérifierait $3X+6=0$, donc serait $-2$, mais $U(-2)=3\ne0$. Ainsi $\gcd(U,V)=1$.


```math
UA=-VB\Rightarrow U\mid B\Rightarrow\boxed{A=-VT,\quad B=UT,\quad T\in\mathbb R[X].}
```



### (iv)



```math
X^2\cdot6+(2X+1)(2-3X)=X+2.
```




```math
\gcd(X^2,2X+1)=1\Rightarrow\boxed{A=6+(2X+1)T,\quad B=2-3X-X^2T,\quad T\in\mathbb R[X].}
```



## Autocorrection D



```math
(X+1)^n-nX-1=\sum_{k=2}^n\binom nkX^k\in X^2\mathbb K[X].
```


Autre méthode : si $F=(X+1)^n-nX-1$, alors $F(0)=F'(0)=0$, donc $X^2\mid F$.

## Exercice 18

### 1

Pour tous $U,V$, $U-V\mid P(U)-P(V)$. Avec $U=P(X)$ et $V=X$,


```math
P(X)-X\mid P(P(X))-P(X).
```


En ajoutant $P(X)-X$,


```math
\boxed{P-X\mid P\circ P-X.}
```



### 2



```math
P=X^2+3X+1,\qquad P(P(X))-X=(X+1)^2(X^2+4X+5).
```




```math
\boxed{z\in\{-1,-2+i,-2-i\}.}
```



## Exercice 19

### (i)



```math
X^{100}=1+100(X-1)+4950(X-1)^2+O((X-1)^3).
```


Le reste a la forme $R=1+100(X-1)+4950(X-1)^2+c(X-1)^3$. La condition $R(-1)=1$ donne $-200+19800-8c=0$, donc $c=2450$.


```math
\boxed{R=1+100(X-1)+4950(X-1)^2+2450(X-1)^3.}
```



### (ii)



```math
X^{2n}=(-1+(X^2+1))^n\equiv(-1)^n+n(-1)^{n-1}(X^2+1)\pmod{(X^2+1)^2}.
```


Pour $n=0$, $R=1$.

### (iii)



```math
X^3\equiv1,\quad X+1\equiv-X^2\pmod{X^2+X+1}.
```




```math
m=2n+1:\qquad (X+1)^m-X^m\equiv-X^{2m}-X^m.
```




```math
\boxed{R=\begin{cases}-2&n\equiv1\pmod3,\\1&n\not\equiv1\pmod3.\end{cases}}
```



## Exercice 20



```math
X^4+X^3+\lambda X^2+\mu X+2\equiv(6-2\lambda)+(\mu-2)X\pmod{X^2+2}.
```




```math
\boxed{\lambda=3,\quad\mu=2.}
```



## Exercice 21



```math
X^2\equiv aX-1\Rightarrow X^4-X+a\equiv(a^3-2a-1)X+(1+a-a^2).
```




```math
a^2-a-1=0\Rightarrow a^3=2a+1.
```




```math
\boxed{a=\frac{1+\sqrt5}2\quad\text{ou}\quad a=\frac{1-\sqrt5}2.}
```



## Exercice 22

Si $P\ne0$, le degré $d$ vérifie $d\ge2$ et $d=2d-3$, donc $d=3$. Le coefficient dominant $c$ vérifie $c=18c^2$, donc $c=1/18$.
Après translation,


```math
P=\frac1{18}(Y^3+bY+c_0),\qquad P'P''=\frac1{18}Y^3+\frac b{54}Y.
```




```math
P=P'P''\Rightarrow b=c_0=0.
```




```math
\boxed{P=0\quad\text{ou}\quad P=\frac{(X-a)^3}{18},\quad a\in\mathbb R.}
```



## Exercice 23

Le sens direct résulte de $Q=AP\Rightarrow Q(X^m)=A(X^m)P(X^m)$.
Réciproquement, si $P\ne0$, divisons $Q=AP+R$, $\deg R<\deg P$.


```math
P(X^m)\mid Q(X^m)\Rightarrow P(X^m)\mid R(X^m).
```




```math
R\ne0\Rightarrow\deg R(X^m)=m\deg R<m\deg P,
```


impossible. Donc $R=0$. Le cas $P=0$ se réduit, des deux côtés, à $Q=0$.

## Exercice 24

### 1



```math
a\mid b,\ b=aq\Rightarrow X^b-1=(X^a-1)\sum_{j=0}^{q-1}X^{aj}.
```


Réciproquement, si $P_a\mid P_b$, $\zeta=e^{2i\pi/a}$ vérifie $\zeta^b=1$, donc $a\mid b$.

### 2

Les racines de $P_a,P_b$ sont simples et appartiennent aux racines de $P_{ab}$. Leur intersection vaut $\mathbb U_{\gcd(a,b)}$.
Le polynôme $(X-1)P_{ab}$ n'a qu'une racine double, $1$.


```math
P_aP_b\mid(X-1)P_{ab}\iff\mathbb U_{\gcd(a,b)}=\{1\}\iff\boxed{\gcd(a,b)=1.}
```



## Exercice 25

Les conditions donnent $P'(\pm1)=P''(\pm1)=0$. Donc


```math
P'=c(X^2-1)^2\Rightarrow P=c\left(\frac{X^5}5-\frac{2X^3}3+X\right)+d.
```




```math
P(1)=-1,\quad P(-1)=1\Rightarrow d=0,\quad\frac{8c}{15}=-1.
```




```math
\boxed{P=-\frac38X^5+\frac54X^3-\frac{15}8X.}
```



## Exercice 26

### 1



```math
P-y=c\prod_{j=1}^r(X-a_j)^{m_j},\qquad\gcd(P-y,P')=\prod_{j=1}^r(X-a_j)^{m_j-1}
```


à normalisation unitaire près. Ainsi


```math
\boxed{|P^{-1}(\{y\})|=r=d-\deg\gcd(P-y,P').}
```



### 2

Les pgcd associés à des valeurs distinctes de $y$ sont deux à deux premiers entre eux, et leur produit divise $P'$.


```math
\sum_{y\in V}\deg\gcd(P-y,P')\le d-1.
```




```math
\boxed{d(|V|-1)<|P^{-1}(V)|\le d|V|.}
```


Avec $P=X^d$, si $0\notin V$, le cardinal vaut $d|V|$ ; si $0\in V$, il vaut $d(|V|-1)+1$.

## Exercice 27

Pour $P\ne0$ non constant, $P'\mid P$ implique


```math
P=(uX+v)P',\qquad u\ne0.
```


Avec $Y=X+v/u$ et $P=\sum_jc_jY^j$,


```math
\sum_jc_jY^j=u\sum_jjc_jY^j\Rightarrow(1-uj)c_j=0.
```


En caractéristique nulle, un seul indice $j=n\ge1$ est possible et $u=1/n$.


```math
\boxed{P=0\quad\text{ou}\quad P=c(X-a)^n,\quad c\in\mathbb K^*,\ a\in\mathbb K,\ n\ge1.}
```



## Exercice 28

### 1



```math
P\text{ irréductible},\quad0\ne P',\quad\deg P'<\deg P\Rightarrow\gcd(P,P')=1.
```


Ainsi $P$ n'a aucune racine multiple.

### 2

Dans la factorisation irréductible de $P$ sur $\mathbb Q$, un facteur $R$ apparaît au moins deux fois.


```math
2\deg R\le5\Rightarrow\deg R=1\text{ ou }2.
```


Si $\deg R=1$, sa racine est rationnelle. Si $\deg R=2$, le quotient $P/R^2$ a degré $1$ et fournit une racine rationnelle.

## Exercice 29

### 1



```math
\boxed{\Phi_p=1+X+\cdots+X^{p-1},\qquad X^p-1=(X-1)\Phi_p.}
```



### 2



```math
\Phi_p(X+1)=\frac{(X+1)^p-1}{X}=\sum_{j=1}^p\binom pjX^{j-1}.
```


Le coefficient dominant vaut $1$, tous les autres sont divisibles par $p$, et le coefficient constant $p$ n'est pas divisible par $p^2$. Le critère d'Eisenstein donne l'irréductibilité de $\Phi_p(X+1)$, donc celle de $\Phi_p$.

### 3

Pour $p$ impair,


```math
\boxed{X^{2p}-1=(X-1)(X+1)\Phi_p(X)\Phi_p(-X).}
```


Les quatre facteurs sont irréductibles : les deux derniers se déduisent par les changements de variable $X\mapsto X$ et $X\mapsto-X$.
Pour $p=2$,


```math
\boxed{X^4-1=(X-1)(X+1)(X^2+1).}
```



### 4



```math
\boxed{\Phi_{p^2}=1+X^p+\cdots+X^{p(p-1)},\qquad X^{p^2}-1=(X-1)\Phi_p\Phi_{p^2}.}
```



### 4(a)



```math
\boxed{\Phi_{p^2}(X)=\prod_{\substack{1\le k\le p^2\\p\nmid k}}(X-e^{2i\pi k/p^2}).}
```



### 4(b)

Dans $\mathbb F_p[X]$,


```math
\Phi_{p^2}(X+1)\equiv X^{p(p-1)}.
```


En effet, $(X+1)^{p^2}-1\equiv X^{p^2}$ et $(X+1)^p-1\equiv X^p$, et leur quotient est $\Phi_{p^2}(X+1)$.
Son coefficient constant vaut $\Phi_{p^2}(1)=p$. Eisenstein en $p$ donne l'irréductibilité.

### 5



```math
\Phi_{p^r}(X)=\sum_{j=0}^{p-1}X^{jp^{r-1}},\qquad\boxed{X^{p^k}-1=(X-1)\prod_{r=1}^k\Phi_{p^r}(X).}
```




```math
\Phi_{p^r}(X+1)\equiv X^{p^{r-1}(p-1)}\pmod p,\qquad\Phi_{p^r}(1)=p.
```


Chaque facteur est irréductible par Eisenstein après translation.

### 6

Les entiers $2,3,4,5,7,8,9,11$ sont des puissances de nombres premiers ; $6$ et $10$ sont deux fois un nombre premier. Le premier cas nouveau est $12$.


```math
\boxed{X^{12}-1=(X-1)(X+1)(X^2+1)(X^2+X+1)(X^2-X+1)(X^4-X^2+1).}
```


Le dernier facteur n'a pas de racine rationnelle. Une factorisation quadratique sur $\mathbb Q$, par le lemme de Gauss, serait


```math
(X^2+aX+b)(X^2-aX+d),\quad a,b,d\in\mathbb Z,\quad bd=1.
```


Donc $b=d=\pm1$ et $2b-a^2=-1$, soit $a^2=3$ ou $a^2=-1$, impossible.

## Exercice 30



```math
\boxed{\begin{array}{c|l}
\deg&\text{polynômes irréductibles unitaires sur }\mathbb F_2\\\hline
1&X,\ X+1\\
2&X^2+X+1\\
3&X^3+X+1,\ X^3+X^2+1\\
4&X^4+X+1,\ X^4+X^3+1,\ X^4+X^3+X^2+X+1
\end{array}}
```


Aux degrés $2,3$, l'irréductibilité équivaut à l'absence des racines $0,1$. Au degré $4$, on exclut aussi la divisibilité par l'unique irréductible quadratique $X^2+X+1$. Parmi les quatre quartiques sans racine, seul $X^4+X^2+1=(X^2+X+1)^2$ est éliminé.

## Exercice 31

Dans $\mathbb F_p$, $2$ est inversible et


```math
4(X^2+bX+c)=(2X+b)^2-(b^2-4c).
```




```math
X^2+bX+c\text{ a une racine}\iff b^2-4c\text{ est un carré}.
```


Un polynôme de degré $2$ est réductible si et seulement s'il possède une racine.

## Exercice 32

### 1(a)



```math
s:\mathbb F_p^*\to\mathbb F_p^*,\quad x\mapsto x^2
```


est un morphisme, donc son image est un sous-groupe. Son noyau est $\{1\}$ si $p=2$, et $\{1,-1\}$ si $p$ est impair.


```math
\boxed{|\operatorname{im}s|=1\ (p=2),\qquad|\operatorname{im}s|=(p-1)/2\ (p\text{ impair}).}
```



### 1(b)

Pour $p=2$, $-1=1$ est un carré. Pour $p$ impair, le sous-groupe des carrés a indice $2$. Si $-1$ et $2$ sont tous deux non carrés, leur produit $-2$ appartient à ce sous-groupe.

### 2



```math
(X+1)^4+1=X^4+4X^3+6X^2+4X+2
```


est Eisenstein en $2$, donc $X^4+1$ est irréductible sur $\mathbb Q$.
Sur $\mathbb F_2$, $X^4+1=(X+1)^4$. Pour $p$ impair, l'une des factorisations suivantes existe :


```math
s^2=-1:\quad X^4+1=(X^2+s)(X^2-s),
```




```math
t^2=2:\quad X^4+1=(X^2+tX+1)(X^2-tX+1),
```




```math
u^2=-2:\quad X^4+1=(X^2+uX-1)(X^2-uX-1).
```



## Autocorrection E

### (i)



```math
j=e^{2i\pi/3},\qquad X^2+X+1=(X-j)(X-j^2).
```


Le polynôme est irréductible sur $\mathbb R$.

### (ii)



```math
X^4-4=(X-\sqrt2)(X+\sqrt2)(X-i\sqrt2)(X+i\sqrt2)
```




```math
=(X-\sqrt2)(X+\sqrt2)(X^2+2).
```



### (iii)



```math
X^4+1=\prod_{k=0}^3(X-e^{i(2k+1)\pi/4})=(X^2-\sqrt2X+1)(X^2+\sqrt2X+1).
```



### (iv)



```math
X^6+27=\prod_{k=0}^5(X-\sqrt3e^{i(2k+1)\pi/6})
```




```math
=(X^2+3)(X^2-3X+3)(X^2+3X+3).
```



### (v)



```math
(X^2-X+1)^2+1=(X-i)(X+i)(X-1-i)(X-1+i)
```




```math
=(X^2+1)((X-1)^2+1).
```



### (vi)



```math
X^5-10X^4+25X^3-25X^2+10X-1=(X-1)^3(X^2-7X+1)
```




```math
=\boxed{(X-1)^3\left(X-\frac{7+3\sqrt5}2\right)\left(X-\frac{7-3\sqrt5}2\right)}.
```


Cette factorisation est valable sur $\mathbb R$ et $\mathbb C$.

### (vii)

Si $\alpha+\beta=\gamma$, Viète donne $2\gamma=8$, donc $\gamma=4$.


```math
X^3-8X^2+23X-28=(X-4)(X^2-4X+7)
```




```math
=(X-4)(X-2-i\sqrt3)(X-2+i\sqrt3).
```



### (viii)

Deux racines de somme $2$ donnent un facteur $X^2-2X+u$. L'autre facteur est $X^2+2X+v$. Identification :


```math
u+v=4,\quad2(u-v)=12,\quad uv=-5\Rightarrow u=5,\ v=-1.
```




```math
X^4+12X-5=(X^2-2X+5)(X^2+2X-1)
```




```math
=(X-1-2i)(X-1+2i)(X+1-\sqrt2)(X+1+\sqrt2).
```



## Exercice 33

### 1



```math
w=\frac{1-z^2}{2z},\quad w^3=-1\Rightarrow w\in\{-1,e^{i\pi/3},e^{-i\pi/3}\}.
```




```math
z^2+2wz-1=0\Rightarrow z=-w\pm\sqrt{w^2+1}.
```


Avec $a=(\sqrt3-1)/2$, $b=(\sqrt3+1)/2$, les six solutions sont


```math
\boxed{1\pm\sqrt2,\quad a(1+i),\ a(1-i),\quad-b(1+i),\ -b(1-i).}
```



### 2

Le coefficient dominant de $P$ vaut $-1$.


```math
\boxed{P=-(X-1-\sqrt2)(X-1+\sqrt2)\prod_{\varepsilon=\pm1}(X-a(1+\varepsilon i))(X+b(1+\varepsilon i)).}
```


Sur $\mathbb R$,


```math
\boxed{P=-(X-1-\sqrt2)(X-1+\sqrt2)\bigl(X^2+(1-\sqrt3)X+2-\sqrt3\bigr)\bigl(X^2+(1+\sqrt3)X+2+\sqrt3\bigr).}
```



## Exercice 34

Pour $n=0$, le polynôme est nul. Pour $n\ge1$,


```math
X^{2n}-2\cos(na)X^n+1=(X^n-e^{ina})(X^n-e^{-ina}).
```




```math
\theta_k=a+\frac{2k\pi}n\quad(0\le k<n).
```




```math
\boxed{P=\prod_{k=0}^{n-1}(X-e^{i\theta_k})(X-e^{-i\theta_k})=\prod_{k=0}^{n-1}(X^2-2\cos\theta_kX+1).}
```


Chaque facteur réel est irréductible sauf lorsque $\theta_k\in\pi\mathbb Z$ ; il vaut alors $(X-1)^2$ ou $(X+1)^2$.

## Exercice 35

Les constantes possibles sont $0$ et $1$. Pour $P$ non constant, le coefficient dominant vérifie $c=c^2$, donc $c=1$.
Soit $S$ l'ensemble fini non vide de ses racines.


```math
z\in S\Rightarrow z^2\in S,\qquad(z+1)^2\in S.
```


L'itération du carré impose $|z|\le1$. Si $|z|<1$, la suite $z^{2^k}$ tend vers $0$ et prend ses valeurs dans $S$, donc $0\in S$. Alors $1\in S$, puis $4\in S$, contradiction. Ainsi $|z|=1$ pour toute racine.


```math
|(z+1)^2|=1\Rightarrow|z+1|=1\Rightarrow2+2\operatorname{Re}z=1.
```




```math
S\subset\{j,j^2\},\qquad j=e^{2i\pi/3}.
```


Le carré échange $j,j^2$, donc ils sont tous deux racines. Si leurs multiplicités sont $r,s$, l'identité en $X=j$ impose $s=r$, car $j-1$ n'est pas une racine et $X\mapsto X^2$ a dérivée non nulle en $j$.


```math
\boxed{P=0\quad\text{ou}\quad P=(X^2+X+1)^m,\quad m\in\mathbb N.}
```


Réciproquement,


```math
(X^2+X+1)(X^2-X+1)=X^4+X^2+1.
```



## Exercice 36

### 1



```math
v_P(0)=+\infty,\qquad v_P(F)=\max\{r\ge0:P^r\mid F\}\quad(F\ne0).
```


La factorisation unique donne $v_P(FG)=v_P(F)+v_P(G)$ ; la divisibilité donne


```math
v_P(F+G)\ge\min(v_P(F),v_P(G)).
```




```math
v_P(P^r)=r
```


assure la surjectivité.

### 2



```math
\nu(1)=0,\quad a\in\mathbb K^*\Rightarrow\nu(a)+\nu(a^{-1})=0\Rightarrow\nu(a)=0.
```




```math
\mathfrak p=\{F:\nu(F)\ge1\}
```


est un idéal propre premier et non nul, par surjectivité. Ainsi $\mathfrak p=(P)$ pour un irréductible unitaire $P$.


```math
F=P^rU,\quad P\nmid U\Rightarrow\nu(U)=0\Rightarrow\nu(F)=r\nu(P).
```


La valeur $1$ étant atteinte, $\nu(P)=1$ ; donc $\nu=v_P$.

### 3



```math
P=X-z.
```


Si $z\in\mathbb R$, la restriction est $v_{X-z}$. Si $z\notin\mathbb R$, pour tout $F\in\mathbb R[X]$,


```math
\mu_z(F)=\mu_{\overline z}(F)=v_Q(F),\qquad Q=(X-z)(X-\overline z)\in\mathbb R[X].
```


$Q$ est irréductible réel et $v_Q(Q)=1$ ; la restriction est donc bien une valuation surjective.

## Exercice 37

Tous les polynômes constants conviennent. Pour $P$ non constant, soit $S$ son ensemble de racines.


```math
S=P^{-1}(S),\quad z\in S\Rightarrow P(z)=0\Rightarrow P(0)=0\Rightarrow0\in S.
```


Si $a\in S\setminus\{0\}$, il existe $z$ tel que $P(z)=a$. Alors $P(P(z))=0$, donc $z\in S$ ; mais cela impose $P(z)=0\ne a$. Contradiction.


```math
S=\{0\}\Rightarrow P=cX^n.
```




```math
\boxed{P\text{ constant}\quad\text{ou}\quad P=cX^n,\ c\in\mathbb C^*,\ n\ge1.}
```


Ces polynômes vérifient effectivement la condition.

## Exercice 38

Si $Q=0$, nécessairement $P=0$. Sinon, toute racine de $Q$ est racine de $P$ avec une multiplicité au moins égale : sinon $P/Q$ serait non borné au voisinage de cette racine.


```math
Q\mid P,\qquad P=RQ,\qquad|R(z)|\le1\text{ hors d'un ensemble fini}.
```


Un polynôme non constant est non borné à l'infini ; donc $R=c$, $|c|\le1$.


```math
\boxed{P=cQ,\quad Q\in\mathbb C[X],\quad c\in\mathbb C,\ |c|\le1.}
```



## Exercice 39

### 1



```math
(A^2+B^2)(C^2+D^2)=(AC-BD)^2+(AD+BC)^2.
```



### 2

Le sens direct est immédiat. Si $P\ge0$ sur $\mathbb R$ et $P\ne0$, son coefficient dominant est positif et chacune de ses racines réelles a multiplicité paire.


```math
P=c\prod_i(X-r_i)^{2m_i}\prod_j((X-a_j)^2+b_j^2)^{e_j},\quad c>0,\ b_j>0.
```


Chaque facteur est une somme de deux carrés ; la stabilité par produit donne $P\in S$. Le polynôme nul appartient aussi à $S$.

## Exercice 40

Le sens direct de $P=A^2+XB^2\Rightarrow P(x)\ge0$ pour $x\ge0$ est immédiat.
Les polynômes de la forme $A^2+XB^2$ sont stables par produit :


```math
(A^2+XB^2)(C^2+XD^2)=(AC-XBD)^2+X(AD+BC)^2.
```


Si $P\ge0$ sur $[0,+\infty)$, ses racines strictement positives ont multiplicité paire. Ses autres facteurs réels, avec un coefficient dominant positif, sont de la forme


```math
X=0^2+X\cdot1^2,\qquad X+a=(\sqrt a)^2+X\cdot1^2\quad(a>0),
```




```math
X^2-2uX+u^2+v^2=(X-r)^2+X\bigl(\sqrt{2(r-u)}\bigr)^2,\quad r=\sqrt{u^2+v^2}>|u|.
```


Les facteurs de multiplicité paire et le coefficient positif sont des carrés. La stabilité donne la représentation demandée, y compris $P=0$.

## Exercice 41



```math
\gcd_{\mathbb Q[X]}(P,Q)=1\Rightarrow\exists U,V\in\mathbb Z[X],\ N\in\mathbb N^*,\quad UP+VQ=N.
```




```math
d_n=\gcd(P(n),Q(n))\mid N\Rightarrow d_n=\gcd(P(n),Q(n),N).
```




```math
P(n+N)\equiv P(n),\quad Q(n+N)\equiv Q(n)\pmod N.
```




```math
\boxed{d_{n+N}=d_n.}
```



## Exercice 42

### 1

Tout diviseur commun de $A,B$ divise $C=-A-B$, donc leur pgcd vaut $1$. Même conclusion pour les deux autres paires.

### 2(a)



```math
A=(X-z)^mU,\quad U(z)\ne0\Rightarrow(X-z)^{m-1}\mid A,\ A'.
```




```math
P=AB'-A'B\Rightarrow\boxed{\mu_z(P)\ge m-1.}
```



### 2(b)



```math
P=AB'-A'B=BC'-B'C=CA'-C'A.
```


Les ensembles de racines de $A,B,C$ sont disjoints. La première question appliquée successivement à ces trois expressions donne


```math
\prod_{z:ABC(z)=0}(X-z)^{\mu_z(ABC)-1}\mid P.
```


De plus, $P\ne0$ : sinon $(A/B)'=0$, donc $A/B$ serait constant ; la coprimalité rendrait $A,B,C$ constants, contradiction.


```math
\boxed{\deg P\ge\deg(ABC)-(n_A+n_B+n_C).}
```



### 3



```math
\deg P\le\deg A+\deg B-1\Rightarrow\deg C\le n_A+n_B+n_C-1.
```


Par permutation de $A,B,C$,


```math
\boxed{n_{ABC}\ge1+\max(\deg A,\deg B,\deg C).}
```



### 4

Pour une solution non identiquement nulle, divisons $x,y,z$ par leur pgcd $g$ :


```math
x=gu,\quad y=gv,\quad z=gw,\quad\gcd(u,v,w)=1,\quad u^n+v^n=w^n.
```


Si l'un est nul, les deux autres sont constants par coprimalité. Sinon,


```math
D=\max(\deg u,\deg v,\deg w).
```


Pour $D\ge1$, Mason–Stothers donne


```math
nD\le n_{uvw}-1\le\deg u+\deg v+\deg w-1\le3D-1,
```


impossible pour $n\ge3$. Ainsi $u,v,w$ sont constants.


```math
\boxed{(x,y,z)=(ag,bg,cg),\quad g\in\mathbb C[X],\quad a,b,c\in\mathbb C,\quad a^n+b^n=c^n.}
```



## Exercice 43

### 1



```math
Q=P^{(j-1)}
```


est simplement scindé par Rolle. Hors de ses racines,


```math
\frac{(Q')^2-QQ''}{Q^2}=\sum_{Q(a)=0}\frac1{(X-a)^2}>0.
```


À une racine $a$, $(Q'(a))^2>0$. Ainsi


```math
P^{(j)}(x)^2>P^{(j-1)}(x)P^{(j+1)}(x).
```



### 2

Si $Q(a)=0$, l'inégalité donne $Q'(a)^2>0$ : toute racine réelle est simple.
Si $Q$ n'avait aucune racine réelle, $h=Q'/Q$ serait définie sur $\mathbb R$ et vérifierait $h'<0$. Mais


```math
h(x)\sim\frac{\deg Q}{x}\quad(|x|\to\infty),
```


donc $h(-R)<0<h(R)$ pour $R$ assez grand, contradiction. Le polynôme $Q$ n'est pas constant, puisque l'inégalité serait alors $0>0$.
Soient $a_1<\cdots<a_r$ ses racines réelles. Sur chaque $(a_i,a_{i+1})$, $h$ décroît de $+\infty$ à $-\infty$ : une unique racine de $Q'$. Sur $(-\infty,a_1)$, $h<0$ ; sur $(a_r,+\infty)$, $h>0$ ; aucune autre racine réelle de $Q'$.


```math
\boxed{Q'\text{ possède exactement }r-1\text{ racines réelles, une dans chaque }(a_i,a_{i+1}).}
```



### 3

Récurrence sur $n$. Pour $n=1$, tout polynôme réel de degré $1$ est simplement scindé. Pour $n\ge2$, les inégalités d'indices $2,\ldots,n-1$ impliquent par récurrence que $P'$ est simplement scindé de degré $n-1$. L'inégalité d'indice $1$ et la deuxième question donnent alors $n$ racines réelles simples pour $P$.

## Exercice 44

### 1



```math
5\cdot6\cdot6=180\not\equiv0\pmod8,\qquad1\cdot2\cdot4=8.
```


Un pavage disjoint imposerait que $8$ divise $180$.

### 2



```math
\sum_{i=1}^AX^i=X\frac{X^A-1}{X-1}.
```




```math
\boxed{w(\mathcal P)=X^3(X^A-1)(X^B-1)(X^C-1).}
```



### 3

Pour une brique de coin minimal $(r,s,t)$, ses longueurs étant une permutation de $(a,b,c)$,


```math
w(\mathcal B)=X^{r+s+t}(X^a-1)(X^b-1)(X^c-1).
```


L'additivité du poids sur une union disjointe donne


```math
\boxed{(X^a-1)(X^b-1)(X^c-1)\mid w(\mathcal P).}
```



### 4



```math
i^4=1,\qquad i^{10}=-1.
```


Le facteur $X^4-1$ s'annule en $i$, mais $X^3(X^{10}-1)^3$ ne s'y annule pas : aucun pavage.

### 5



```math
\mu_{-1}((X-1)(X^2-1)(X^4-1))=2,
```




```math
\mu_{-1}(X^3(X^7-1)(X^8-1)(X^9-1))=1.
```


La divisibilité nécessaire est impossible.

### 6

Supposons $a\mid b\mid c$ et un pavage existant. À une racine primitive $c$-ième de l'unité, le diviseur précédent s'annule au moins une fois ; l'une des dimensions, notée $C$ après permutation, est divisible par $c$.
À une racine primitive $b$-ième, sa multiplicité dans le diviseur est au moins $2$ : au moins deux dimensions sont divisibles par $b$. Comme $b\mid C$, une autre dimension, notée $B$, est divisible par $b$.
À une racine primitive $a$-ième, sa multiplicité est $3$ : toutes les dimensions sont divisibles par $a$, notamment la dimension restante $A$.


```math
a\mid A,\qquad b\mid B,\qquad c\mid C.
```


Réciproquement, ces trois divisibilités permettent de découper chaque axe en intervalles de longueurs respectives $a,b,c$ ; leurs produits cartésiens pavent le grand pavé.


```math
\boxed{\mathcal P\text{ est }(a,b,c)\text{-pavable}\iff\exists\text{ une permutation des dimensions telle que }a\mid A,\ b\mid B,\ c\mid C.}
```


