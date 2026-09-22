# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td25-fractions-rationnelles.pdf)

## Autocorrection A



```math
F(X+1)=F(X),\quad z\text{ pôle de }F\Rightarrow z+\mathbb Z\subset\mathcal P_F.
```


Une fraction rationnelle n'a qu'un nombre fini de pôles ; $F$ est donc un polynôme.


```math
\deg F=d\ge1\Rightarrow\deg(F(X+1)-F(X))=d-1,\quad\bot.
```




```math
\boxed{F\in\mathbb C.}
```



## Autocorrection B



```math
F^2=1/X\Rightarrow2\mu_0(F)=-1,
```


impossible puisque $\mu_0(F)\in\mathbb Z$.

## Exercice 1



```math
R^2=\frac{X^2}{(X+1)(X+2)}\Rightarrow2\mu_{-1}(R)=-1.
```




```math
\boxed{\text{Aucune solution}.}
```



## Exercice 2

### 1



```math
P/Q=P_1/Q_1\Rightarrow PQ_1=P_1Q\Rightarrow\mu_z(P)+\mu_z(Q_1)=\mu_z(P_1)+\mu_z(Q).
```




```math
\mu_z(P)-\mu_z(Q)=\mu_z(P_1)-\mu_z(Q_1).
```


Pour la fraction nulle, $\mu_z(0)=+\infty$.

### 2



```math
F=H+\sum_{a}\sum_{k=1}^{m_a}\frac{c_{a,k}}{(X-a)^k}\Rightarrow F'=H'-\sum_a\sum_{k=1}^{m_a}\frac{k c_{a,k}}{(X-a)^{k+1}}.
```


La dérivée n'a aucun élément simple d'ordre $1$, contrairement à $1/X$.

## Exercice 3



```math
\frac1{X^2+1}=\frac1{2i}\left(\frac1{X-i}-\frac1{X+i}\right).
```


Les résidus en $\pm i$ sont non nuls ; aucune dérivée rationnelle ne peut être égale à cette fraction.

## Exercice 4



```math
T(X)=\frac{X^2}{1+X^2}.
```


Si $a\ne1$ est un pôle de $R$, soit $z\in\mathbb C$ tel que $z^2=a/(1-a)$. Alors


```math
1+z^2=\frac1{1-a}\ne0,\quad T(z)=a\Rightarrow z\text{ pôle de }R\circ T,
```


contradiction. Si $1$ n'est pas un pôle, $R$ n'a donc aucun pôle fini : $R$ est un polynôme non constant. Mais $T$ a un pôle en $i$, et donc $R\circ T$ aussi.


```math
\boxed{1\text{ est un pôle de }R.}
```



## Exercice 5



```math
R=P/Q,\quad\gcd(P,Q)=1.
```


Pour $R$ non constante,


```math
\lambda\notin\operatorname{im}R\iff P-\lambda Q\text{ n'a aucune racine}\iff P-\lambda Q\in\mathbb C^*.
```


En effet, une racine de $P-\lambda Q$ ne peut être racine de $Q$.


```math
\lambda\ne\mu,\quad P-\lambda Q=c,\quad P-\mu Q=d\Rightarrow(\mu-\lambda)Q=c-d,
```


donc $Q$, puis $P$, serait constant. Au plus une valeur est omise.


```math
R=X\Rightarrow\operatorname{im}R=\mathbb C,
```




```math
R=a+1/X\Rightarrow\operatorname{im}R=\mathbb C\setminus\{a\},\qquad R=a\Rightarrow\operatorname{im}R=\{a\}.
```




```math
\boxed{\{\operatorname{im}R:R\in\mathbb C(X)\}=\{\mathbb C\}\cup\{\mathbb C\setminus\{a\}:a\in\mathbb C\}\cup\{\{a\}:a\in\mathbb C\}.}
```



## Exercice 6



```math
F=P/Q,\quad Q=\sum_{j=0}^dq_jX^j,\quad q_0\ne0,\quad a_n=\frac{F^{(n)}(0)}{n!}.
```


La formule de Leibniz appliquée à $QF=P$ donne


```math
\forall n\ge0,\qquad\sum_{j=0}^{\min(d,n)}q_ja_{n-j}=\frac{P^{(n)}(0)}{n!}.
```




```math
\boxed{q_0a_n+q_1a_{n-1}+\cdots+q_da_{n-d}=0\quad(n\ge\max(d,1+\deg P)).}
```


Le coefficient $q_0$ est non nul.

## Autocorrection C



```math
\boxed{\frac1{(X^2+1)(X-1)^2}=\frac{X}{2(X^2+1)}-\frac1{2(X-1)}+\frac1{2(X-1)^2}.}
```




```math
A=X^2+1,\quad B=(X-1)^2\Rightarrow\boxed{\left(1-\frac X2\right)A+\frac X2B=1.}
```



## Autocorrection D

Les coefficients ci-dessous s'obtiennent par multiplication par le dénominateur puis identification. À un pôle simple $a$ de $P/Q$, le coefficient vaut $P(a)/Q'(a)$.

### (i)

Sur $\mathbb R$, la fraction donnée est déjà un élément simple. Sur $\mathbb C$, $j=e^{2i\pi/3}$ :


```math
\frac{X+1}{X^2+X+1}=\frac{j+1}{2j+1}\frac1{X-j}+\frac{j^2+1}{2j^2+1}\frac1{X-j^2}.
```



### (ii)



```math
\frac1{(X+1)^2(3-X)}=\frac1{16(X+1)}+\frac1{4(X+1)^2}-\frac1{16(X-3)}.
```



### (iii)



```math
\frac1{(X^2-1)(X+1)^2}=\frac1{8(X-1)}-\frac1{8(X+1)}-\frac1{4(X+1)^2}-\frac1{2(X+1)^3}.
```



### (iv)



```math
\frac{7X^2+4X-4}{X^4-4X^2}=-\frac1X+\frac1{X^2}+\frac2{X-2}-\frac1{X+2}.
```



### (v)



```math
\frac{X^4+1}{X^4-1}=1+\frac1{2(X-1)}-\frac1{2(X+1)}-\frac1{X^2+1}.
```


Sur $\mathbb C$,


```math
-\frac1{X^2+1}=\frac{i}{2(X-i)}-\frac{i}{2(X+i)}.
```



### (vi)



```math
\frac{3X-1}{X^2(X+1)^2}=\frac5X-\frac1{X^2}-\frac5{X+1}-\frac4{(X+1)^2}.
```



### (vii)



```math
\frac{X^3-1}{(X-2)^2}=X+4+\frac{12}{X-2}+\frac7{(X-2)^2}.
```



### (viii)

Sur $\mathbb R$, $4/(X^2+1)^2$ est déjà un élément simple. Sur $\mathbb C$,


```math
\frac4{(X^2+1)^2}=-\frac{i}{X-i}+\frac{i}{X+i}-\frac1{(X-i)^2}-\frac1{(X+i)^2}.
```



### (ix)



```math
\frac{X^2+X+1}{X^3+X^2+X+1}=\frac1{2(X+1)}+\frac{X+1}{2(X^2+1)}
```




```math
=\frac1{2(X+1)}+\frac{1-i}{4(X-i)}+\frac{1+i}{4(X+i)}.
```



### (x)



```math
\frac{3X^4+X^3+4X^2-X-3}{(X+1)(X^2+1)^2}=\frac1{X+1}+\frac{2X-1}{X^2+1}+\frac{X-3}{(X^2+1)^2}
```




```math
=\frac1{X+1}+\frac{1+5i/4}{X-i}+\frac{1-5i/4}{X+i}+\frac{3-i}{4(X-i)^2}+\frac{3+i}{4(X+i)^2}.
```



## Exercice 7

### 1



```math
\frac{1+x^3}{1+x^2}=(1+x^3)(1-x^2+x^4-x^6+o(x^7))
```




```math
\boxed{=1-x^2+x^3+x^4-x^5-x^6+x^7+o(x^7).}
```



### 2



```math
\boxed{\frac{X^3+1}{X^8(X^2+1)}=\frac1{X^8}-\frac1{X^6}+\frac1{X^5}+\frac1{X^4}-\frac1{X^3}-\frac1{X^2}+\frac1X+\frac{1-X}{X^2+1}.}
```



## Exercice 8

### (i)



```math
\frac{X^2+X+1}{X^n}=X^{2-n}+X^{1-n}+X^{-n}.
```


Pour $n=2$, le premier terme est la partie entière $1$.

### (ii)



```math
\frac{X^{2n}}{(X^2+1)^n}=\left(1-\frac1{X^2+1}\right)^n=\boxed{1+\sum_{k=1}^n\frac{(-1)^k\binom nk}{(X^2+1)^k}.}
```



### (iii)



```math
Q=\prod_{j=0}^n(X-j),\qquad Q'(k)=\prod_{j\ne k}(k-j)=(-1)^{n-k}k!(n-k)!.
```




```math
\boxed{\frac1Q=\frac1{n!}\sum_{k=0}^n\frac{(-1)^{n-k}\binom nk}{X-k}.}
```



### (iv)



```math
\frac1{(1-X)^n}=\sum_{j=0}^{n-1}\binom{n+j-1}jX^j+O(X^n).
```


La symétrie $X\mapsto1-X$ donne la partie polaire en $1$ :


```math
\boxed{\frac1{X^n(1-X)^n}=\sum_{k=1}^n\binom{2n-k-1}{n-k}\left(\frac1{X^k}+\frac1{(1-X)^k}\right).}
```



## Exercice 9



```math
\mu_n=\{\zeta\in\mathbb C:\zeta^n=1\}.
```



### (i)



```math
\frac{X^{n-1}}{X^n-1}=\frac1n\frac{(X^n-1)'}{X^n-1}=\boxed{\frac1n\sum_{\zeta\in\mu_n}\frac1{X-\zeta}.}
```



### (ii)



```math
\boxed{\left(\frac{nX^{n-1}}{X^n-1}\right)'=-\sum_{\zeta\in\mu_n}\frac1{(X-\zeta)^2}.}
```



### (iii)



```math
\frac{X^n-1}{X^n+1}=1-\frac2{X^n+1},\qquad\eta^n=-1\Rightarrow-\frac2{n\eta^{n-1}}=\frac{2\eta}n.
```




```math
\boxed{\frac{X^n-1}{X^n+1}=1+\frac2n\sum_{\eta^n=-1}\frac\eta{X-\eta}.}
```



### (iv)



```math
X^n-1=n(X-1)+\frac{n(n-1)}2(X-1)^2+O((X-1)^3).
```




```math
\boxed{\frac1{(X-1)(X^n-1)}=\frac1{n(X-1)^2}-\frac{n-1}{2n(X-1)}+\frac1n\sum_{\substack{\zeta\in\mu_n\\\zeta\ne1}}\frac{\zeta}{(\zeta-1)(X-\zeta)}.}
```



## Exercice 10



```math
\frac1{X^n-1}=\frac1n\sum_{\zeta\in\mu_n}\frac\zeta{X-\zeta}\Rightarrow\boxed{\left(\frac1{X^n-1}\right)'=-\frac1n\sum_{\zeta\in\mu_n}\frac\zeta{(X-\zeta)^2}.}
```




```math
\frac1{(X^n-1)^2}=-\frac1n\left(\frac X{X^n-1}\right)'-\frac{n-1}{n(X^n-1)}.
```




```math
\boxed{\frac1{(X^n-1)^2}=\frac1{n^2}\sum_{\zeta\in\mu_n}\left(\frac{\zeta^2}{(X-\zeta)^2}-\frac{(n-1)\zeta}{X-\zeta}\right).}
```



## Exercice 11



```math
T_0=1,\quad T_1=X,\quad T_{n+1}=2XT_n-T_{n-1}.
```




```math
\cos((n+1)\theta)=2\cos\theta\cos(n\theta)-\cos((n-1)\theta)
```


donne $T_n(\cos\theta)=\cos(n\theta)$. Deux tels polynômes coïncident sur $[-1,1]$, donc sont égaux.


```math
\deg T_n=n,\quad\theta_k=\frac{(2k-1)\pi}{2n},\quad a_k=\cos\theta_k,\quad T_n(a_k)=0\quad(1\le k\le n).
```




```math
-\sin\theta\,T_n'(\cos\theta)=-n\sin(n\theta)\Rightarrow T_n'(a_k)=\frac{n(-1)^{k-1}}{\sin\theta_k}.
```




```math
\boxed{\frac1{T_n(X)}=\frac1n\sum_{k=1}^n\frac{(-1)^{k-1}\sin\theta_k}{X-\cos\theta_k}.}
```



## Autocorrection E



```math
\frac1{k(k+1)}=\frac1k-\frac1{k+1}\Rightarrow\sum_{k=1}^n\frac1{k(k+1)}=1-\frac1{n+1}.
```




```math
\frac1{k(k+1)(k+2)}=\frac12\left(\frac1{k(k+1)}-\frac1{(k+1)(k+2)}\right),
```




```math
\sum_{k=1}^n\frac1{k(k+1)(k+2)}=\frac14-\frac1{2(n+1)(n+2)}.
```



## Exercice 12



```math
\frac{k+3}{k(k+1)(k+2)}=\frac3{2k}-\frac2{k+1}+\frac1{2(k+2)}.
```




```math
\sum_{k=1}^n\frac{k+3}{k^3+3k^2+2k}=\frac54-\frac3{2(n+1)}+\frac1{2(n+2)}\longrightarrow\boxed{\frac54}.
```




```math
k^4+k^2+1=(k^2-k+1)(k^2+k+1),
```




```math
\frac{k}{k^4+k^2+1}=\frac12\left(\frac1{k^2-k+1}-\frac1{k^2+k+1}\right).
```




```math
\sum_{k=0}^n\frac{k}{k^4+k^2+1}=\frac12\left(1-\frac1{n^2+n+1}\right)\longrightarrow\boxed{\frac12}.
```



## Exercice 13

### 1



```math
P\ne0,\quad\deg P=n\ge1,\quad P'\mid P\Rightarrow P=(aX+b)P',\quad a\ne0.
```




```math
P=c\prod_{j=1}^r(X-z_j)^{m_j}\Rightarrow\frac{P'}P=\sum_{j=1}^r\frac{m_j}{X-z_j}=\frac1{aX+b}.
```




```math
r=1\Rightarrow P=c(X-z)^n.
```


Réciproquement, $P'=nc(X-z)^{n-1}\mid P$. Les constantes non nulles ne conviennent pas, car $0\nmid c$ ; $P=0$ convient.


```math
\boxed{P=0\quad\text{ou}\quad P=c(X-z)^n,\quad c\ne0,\ z\in\mathbb C,\ n\ge1.}
```



### 2



```math
P\in\mathbb R[X]\setminus\{0\}\Rightarrow c\in\mathbb R^*,\quad z\in\mathbb R
```


par invariance des racines par conjugaison. La même classification vaut avec des paramètres réels.

## Exercice 14

### 1



```math
R=H+\sum_{a,k}\frac{c_{a,k}}{(X-a)^k}\Rightarrow\operatorname{res}_a(R')=0.
```


Réciproquement, si


```math
F=H+\sum_a\sum_{k=2}^{m_a}\frac{b_{a,k}}{(X-a)^k},
```


alors, pour $G\in\mathbb C[X]$ tel que $G'=H$,


```math
F=\left(G-\sum_a\sum_{k=2}^{m_a}\frac{b_{a,k}}{(k-1)(X-a)^{k-1}}\right)'.
```



### 2



```math
F\in\mathbb R(X),\quad F=R',\ R\in\mathbb C(X)\Rightarrow\overline R'=F.
```




```math
S=\frac{R+\overline R}2\in\mathbb R(X),\qquad S'=F.
```


L'inclusion réciproque est immédiate par dérivation.

## Exercice 15

### (i)



```math
\frac1P=\sum_{k=1}^n\frac1{P'(x_k)(X-x_k)}.
```




```math
X\to\infty:\quad\frac XP\to0\Rightarrow\boxed{\sum_{k=1}^n\frac1{P'(x_k)}=0.}
```



### (ii)

Évaluation de la même identité en $0$ :


```math
\frac1{P(0)}=-\sum_{k=1}^n\frac1{x_kP'(x_k)}.
```



### (iii)



```math
\frac{P''}P=\sum_{k=1}^n\frac{P''(x_k)}{P'(x_k)(X-x_k)},\qquad\frac{XP''}P\to0.
```




```math
\boxed{\sum_{k=1}^n\frac{P''(x_k)}{P'(x_k)}=0.}
```



## Exercice 16

### 1



```math
\deg P<\deg Q,\qquad Q'(k)=(-1)^{n-k}k!(n-k)!.
```




```math
\boxed{\frac PQ=\sum_{k=0}^n\frac{P(k)}{Q'(k)(X-k)}=\frac1{n!}\sum_{k=0}^n\frac{(-1)^{n-k}\binom nkP(k)}{X-k}.}
```



### 2



```math
\frac{XP(X)}{Q(X)}\longrightarrow1\Rightarrow\boxed{\sum_{k=0}^n(-1)^{n-k}\binom nkP(k)=n!.}
```



### 3



```math
n!\le\sum_{k=0}^n\binom nk|P(k)|\le2^n\max_{0\le k\le n}|P(k)|.
```



## Exercice 17

### 1



```math
P=c\prod_{k=1}^n(X-a_k),\quad P'=nc\prod_{j=1}^{n-1}(X-b_j),\qquad a_j<b_j<a_{j+1}.
```




```math
\frac{P'}P=\sum_{i=1}^n\frac1{X-a_i}.
```


Le résidu en $a_i$ vaut aussi


```math
n\frac{\prod_{j=1}^{n-1}(a_i-b_j)}{\prod_{k\ne i}(a_i-a_k)}=1.
```



### 2



```math
n=\prod_{j<i}\frac{a_i-a_j}{a_i-b_j}\prod_{j\ge i}\frac{a_{j+1}-a_i}{b_j-a_i}.
```


Chaque facteur est supérieur à $1$ ; en isolant celui d'indice $j=i$,


```math
n\ge\frac{a_{i+1}-a_i}{b_i-a_i}\Rightarrow b_i\ge a_i+\frac{a_{i+1}-a_i}{n}.
```


La même identité en $a_{i+1}$, en isolant le facteur d'indice $j=i$, donne


```math
n\ge\frac{a_{i+1}-a_i}{a_{i+1}-b_i}\Rightarrow b_i\le a_{i+1}-\frac{a_{i+1}-a_i}{n}.
```



## Exercice 18

### 1

L'énoncé est faux pour une algèbre quelconque : $A=\mathbb K[T]$, $a=T$ est transcendant, mais $T$ n'est pas inversible.

Condition exacte :


```math
\boxed{\operatorname{ev}_a\text{ s'étend à }\mathbb K(X)\iff\forall Q\in\mathbb K[X]\setminus\{0\},\quad Q(a)\in A^\times.}
```


Nécessité : l'image de $1/Q$ est l'inverse de $Q(a)$. Suffisance :


```math
\Phi(P/Q)=P(a)Q(a)^{-1}.
```


Les $P(a),Q(a)$ et leurs inverses commutent ; $PQ_1=P_1Q$ assure que $\Phi$ est bien définie et c'est un morphisme.
Si $A$ est un corps,


```math
Q(a)\in A^\times\iff Q(a)\ne0,
```


et la condition est exactement la transcendance de $a$.

### 2

Si $a\in L$ était transcendant sur $\mathbb C$, la famille


```math
\left(\frac1{a-z}\right)_{z\in\mathbb C}
```


serait libre sur $\mathbb C$. En effet,


```math
\sum_{j=1}^r\frac{c_j}{a-z_j}=0\Rightarrow\sum_{j=1}^rc_j\prod_{\ell\ne j}(X-z_\ell)=0
```


par transcendance. L'évaluation en $z_j$ donne $c_j=0$.
Cette famille libre non dénombrable contredit la dimension au plus dénombrable de $L$. Ainsi tout $a\in L$ est algébrique sur $\mathbb C$, donc appartient à $\mathbb C$ puisque celle-ci est algébriquement close.


```math
\boxed{L=\mathbb C.}
```



## Exercice 19

### 1



```math
Q=P^{(k-1)}.
```


Si $Q$ est constant ou nul, $QQ''\le(Q')^2$ est immédiat. Sinon, $Q$ est scindé par le théorème de Rolle avec multiplicités. Hors de ses racines,


```math
\frac{Q'}Q=\sum_j\frac{m_j}{X-a_j}\Rightarrow\left(\frac{Q'}Q\right)'=-\sum_j\frac{m_j}{(X-a_j)^2}\le0.
```




```math
QQ''-(Q')^2\le0.
```


L'inégalité s'étend aux racines par continuité.

### 2

Tel qu'imprimé, le critère est faux : pour $k>n$, il impose $0<0$.

Critère corrigé, pour $n\ge1$ :


```math
\boxed{P\text{ simplement scindé}\iff\forall k\in\{1,\ldots,n\},\ \forall x\in\mathbb R,\quad P^{(k-1)}(x)P^{(k+1)}(x)<P^{(k)}(x)^2.}
```


Sens direct : chaque $Q=P^{(k-1)}$ est simplement scindé ; hors de ses racines, la somme précédente est strictement positive. À une racine $a$, $(Q'(a))^2>0$.

Réciproque par récurrence sur $n$. Pour $n=1$, le résultat est immédiat. Les inégalités d'indices $2,\ldots,n$ assurent que $P'$ est simplement scindé. Soient $b_1<\cdots<b_{n-1}$ ses racines.


```math
P(b_i)P''(b_i)<0.
```


Si $c$ est le coefficient dominant de $P$,


```math
\operatorname{sgn}P''(b_i)=\operatorname{sgn}(c)(-1)^{n-1-i},\qquad\operatorname{sgn}P(b_i)=\operatorname{sgn}(c)(-1)^{n-i}.
```


Ces signes alternent ; ils sont opposés aux signes de $P$ à $-\infty$ et $+\infty$ aux deux extrémités. Le théorème des valeurs intermédiaires donne une racine dans chacun des $n$ intervalles séparés par les $b_i$. Elles sont distinctes.

## Exercice 20

### 1

Avec la définition imprimée, $1\notin\mathcal O_\infty$ : ce n'est pas une sous-algèbre unitaire. C'est une algèbre sans unité, car


```math
\deg(F+G)\le\max(\deg F,\deg G)<0,\quad\deg(FG)=\deg F+\deg G<0,
```




```math
\deg(\lambda F)=\deg F\quad(\lambda\ne0).
```



### 2

Posons $v(F)=-\deg F$ et


```math
V_m=\{0\}\cup\{F:v(F)\ge m\}\quad(m\ge1).
```


Les idéaux d'algèbre, donc $\mathbb K$-linéaires, sont


```math
\boxed{\{0\}\quad\text{et}\quad V_m\ (m\ge1).}
```


En effet, pour $I\ne0$, soit $m=\min v(I\setminus\{0\})$ et $f\in I$ tel que $v(f)=m$.


```math
g\in V_{m+1}\Rightarrow v(g/f)\ge1\Rightarrow g=f(g/f)\in I.
```


Si $g\in V_m$ et $v(g)=m$, soit $c\in\mathbb K$ le quotient des coefficients dominants à l'infini de $g$ et $f$ ; alors $g-cf\in V_{m+1}\subset I$, donc $g\in I$.

Pour les idéaux d'anneau sans condition de $\mathbb K$-linéarité, la classification exacte est


```math
\boxed{I_{m,H}=\{F\in V_m:\lim_{X\to\infty}X^mF(X)\in H\},}
```


où $m\ge1$ et $H\ne\{0\}$ est un sous-groupe additif de $\mathbb K$, ainsi que l'idéal nul. La « limite » désigne le coefficient de $X^{-m}$, y compris sur un corps abstrait.
Le raisonnement précédent donne $V_{m+1}\subset I\subset V_m$ ; le quotient $I/V_{m+1}$ est précisément $H$. Réciproquement, $\mathcal O_\infty I_{m,H}\subset V_{m+1}\subset I_{m,H}$.

Avec la définition unitaire usuelle $\deg F\le0$, les idéaux sont $\{0\}$ et $V_m$ pour $m\ge0$.

## Exercice 21

### 1



```math
v_P(A/B)=\operatorname{ord}_P(A)-\operatorname{ord}_P(B),\qquad|F|_P=2^{-v_P(F)}\ (F\ne0),\quad|0|_P=0.
```




```math
v_P(FG)=v_P(F)+v_P(G),\quad v_P(F+G)\ge\min(v_P(F),v_P(G)).
```




```math
|FG|_P=|F|_P|G|_P,\qquad|F+G|_P\le\max(|F|_P,|G|_P).
```




```math
|P|_P=1/2\ne1.
```


Si $P\ne Q$ sont irréductibles unitaires,


```math
|P|_P=1/2,\qquad|P|_Q=1,
```


ce qui interdit leur équivalence.

### 2



```math
|F|_\infty=2^{\deg F}\quad(F\ne0),\qquad|0|_\infty=0.
```


L'additivité du degré sur les produits et sa majoration sur les sommes donnent les axiomes et même l'inégalité ultramétrique.


```math
P\text{ non constant}\Rightarrow|P|_\infty=2^{\deg P}>1.
```



### 3

D'abord, pour tout entier $N\ge1$,


```math
|F+G|^N=|(F+G)^N|\le\sum_{k=0}^N\left|\binom Nk\right||F|^k|G|^{N-k}\le(N+1)\max(|F|,|G|)^N.
```


Les coefficients non nuls appartiennent à $\mathbb K^*$ et ont valeur absolue $1$.


```math
N\to\infty\Rightarrow|F+G|\le\max(|F|,|G|).
```



Si $r=|X|>1$, pour $A=a_dX^d+\cdots+a_0$, $a_d\ne0$,


```math
|a_dX^d|=r^d>\max_{k<d}|a_kX^k|\Rightarrow|A|=r^d.
```




```math
|A/B|=r^{\deg(A/B)}=|A/B|_\infty^{\log_2r}.
```



Si $|X|\le1$, tout polynôme a valeur absolue au plus $1$. Posons


```math
\mathfrak p=\{A\in\mathbb K[X]:|A|<1\}.
```


C'est un idéal propre ; il est premier, car $|AB|<1$ avec $|A|,|B|\le1$ implique $|A|<1$ ou $|B|<1$. Il est non nul : sinon tous les polynômes non nuls, donc toutes les fractions non nulles, auraient valeur absolue $1$.


```math
\mathfrak p=(P),\qquad P\text{ irréductible unitaire},\quad c=|P|\in(0,1).
```




```math
A=P^mU,\quad P\nmid U\Rightarrow|U|=1\Rightarrow|A|=c^m.
```




```math
|F|=c^{v_P(F)}=|F|_P^{-\log_2c},\qquad-\log_2c>0.
```



### 4



```math
|\mathbb K|=q,\quad a\in\mathbb K^*\Rightarrow a^{q-1}=1\Rightarrow|a|^{q-1}=1\Rightarrow|a|=1.
```



### 5

Soit $t\in\mathbb R$ transcendant sur $\mathbb Q$.


```math
|P/Q|_t=\left|\frac{P(t)}{Q(t)}\right|_{\mathbb R}
```


est une valeur absolue sur $\mathbb Q(X)$, car l'évaluation en $t$ est un morphisme de corps injectif.


```math
|2|_t=2,\qquad|2|_P=|2|_\infty=1.
```


Elle n'est équivalente à aucune des valeurs absolues précédentes.
