# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td13-polynomes.pdf)

## Autocorrection A



```math
\begin{aligned}
PQ&=2X^5-3X^4+8X^3-6X^2+4X-1,\\
P^2&=X^6-2X^5+7X^4-8X^3+11X^2-6X+1,\\
Q^2&=4X^4-4X^3+5X^2-2X+1,\\
P\circ Q&=8X^6-12X^5+14X^4-9X^3+10X^2-4X+2,\\
Q\circ P&=2X^6-4X^5+14X^4-17X^3+23X^2-15X+4.
\end{aligned}
```



## Autocorrection B

La somme a degré $n$, coefficient dominant $2$, et terme constant $1+(-1)^n$. La différence a degré $n-1$, coefficient dominant $2n$, et terme constant $1-(-1)^n$.

## Exercice 1

(i) En $X=0$, $P(0)=P(0)-1$, impossible. (ii) $P=0$ convient. Sinon $2\deg P=\deg P+2$, donc $P=aX^2+bX+c$; comparer les coefficients dans $P(X^2)=(X^2+1)P(X)$ donne $b=0$ et $c=-a$. Ainsi $P=a(X^2-1)$. (iii) Les constantes $c$ conviennent. Si $P$ est non constant, les degrés imposent $\deg P=1$. Écrivons $P=aX+b$: $P\circ P=P$ donne $a^2=a$ et $ab=0$, donc $a=1,b=0$; la seule solution non constante est $P=X$. (iv) Si $P\ne0$, l’ordre de multiplicité de $X$ dans $XP^2$ est impair, celui dans le carré $Q^2$ pair. Donc $P=Q=0$.

## Exercice 2

La récurrence donne $P_2=4X^2-2$, $P_3=-8X^3+12X$, $P_4=16X^4-48X^2+12$. Par récurrence, $\deg P_n=n$ et le coefficient dominant est $(-2)^n$; la parité alterne avec celle de $n$. Ainsi $P_{2n+1}(0)=0$. Si $c_n=P_{2n}(0)$, alors $c_0=1$ et $c_{n+1}=-2(2n+1)c_n$, donc $P_{2n}(0)=(-1)^n(2n)!/n!$.

## Exercice 3

1. Séparer les coefficients d’indices pairs et impairs fournit $R_0(X)=\sum a_{2k}X^k$, $R_1(X)=\sum a_{2k+1}X^k$. L’unicité suit de l’unicité des coefficients. 2. Avec $P=R_0(X^2)+XR_1(X^2)$, la partie impaire de $P^2$ est $2XR_0(X^2)R_1(X^2)$. Si $\operatorname{car}K\ne2$, elle est nulle seulement si $R_0R_1=0$, donc $P=R(X^2)$ ou $P=XR(X^2)$. En caractéristique $2$, l’énoncé est faux: $P=1+X$ vérifie $P^2=1+X^2$, mais n’a aucune des deux formes demandées.

## Exercice 4

### 1

Avec $\zeta=e^{2i\pi/n}$,


```math
S_p=\sum_{k=0}^{n-1}\zeta^{kp}=\begin{cases}n,&n\mid p,\\\dfrac{1-\zeta^{np}}{1-\zeta^p}=0,&n\nmid p.\end{cases}
```


La même formule vaut pour tout entier relatif $p$, y compris $p=0$.

### 2

Choisir $N>d$. En développant le carré et en appliquant la question 1,


```math
\frac1N\sum_{z^N=1}|P(z)|^2=\sum_{k,\ell=0}^da_k\overline{a_\ell}\frac1N\sum_{z^N=1}z^{k-\ell}=\sum_{k=0}^d|a_k|^2.
```


Au moins une des valeurs moyennées est supérieure ou égale à leur moyenne. Ainsi, pour une racine $N$-ième de l'unité $z$,


```math
|P(z)|\ge\left(\sum_{k=0}^d|a_k|^2\right)^{1/2}\ge\max_k|a_k|.
```



## Exercice 5

Pour $P,Q\in\mathbb R[X]$, factoriser $P^3-Q^3=(P-Q)(P-jQ)(P-j^2Q)$. Les deux derniers facteurs sont conjugués et de degré $n$, tandis que $P-Q\ne0$; donc $\deg(P^3-Q^3)\ge2n$. Sur $\mathbb C[X]$, le résultat est faux: prendre $P=X^n$ et $Q=j^2X^n$. Alors $P\ne Q$, mais $P^3-Q^3=0$.

## Exercice 6

Pour $P(X)=\sum_{k=0}^da_kX^k$, l'identité $U^k-V^k=(U-V)\sum_{j=0}^{k-1}U^{k-1-j}V^j$ donne


```math
P(P(X))-P(X)=(P(X)-X)\sum_{k=1}^da_k\sum_{j=0}^{k-1}P(X)^{k-1-j}X^j.
```


En ajoutant $P(X)-X$,


```math
P(P(X))-X=(P(X)-X)Q(X),\qquad Q(X)=1+\sum_{k=1}^da_k\sum_{j=0}^{k-1}P(X)^{k-1-j}X^j.
```


Cette identité couvre aussi le cas $P=X$.

## Exercice 7

Alice demande d’abord $S=P(1)$, somme des coefficients. Si $S=0$, alors $P=0$. Sinon elle pose $B=S+1\ge2$ et demande $P(B)$. Écrivons $P=\sum a_kX^k$; chaque chiffre $a_k$ vérifie $0\le a_k\le S<B$. L’écriture de $P(B)=\sum a_kB^k$ en base $B$ restitue donc exactement tous les coefficients, et Alice connaît $P$. Deux tours suffisent. Un seul ne suffit pas: pour une interrogation en $k=0$, $0$ et $X$ ont même valeur; en $k=1$, $1$ et $X$; en $k\ge2$, les polynômes constants $k$ et $X$; en $k=-1$, $1$ et $X^2$; en $k\le-2$, les polynômes constants $k^2$ et $X^2$. La réponse est donc deux tours.

## Exercice 8

Tout entier $m$ s'écrit de manière unique $m=-2q+r$, avec $r\in\{0,1\}$ et $q\in\mathbb Z$ : le reste $r$ est imposé par la parité de $m$. Pour $|m|\ge2$,


```math
|q|\le\frac{|m|+1}{2}<|m|.
```


Pour $m=1$, le quotient vaut $0$ ; pour $m=-1$, il vaut $1$, puis $0$ à l'étape suivante. L'itération termine donc et donne $m=\sum_{k=0}^d\epsilon_k(-2)^k$, $\epsilon_k\in\{0,1\}$.

Pour l'unicité, si deux polynômes distincts donnent la même valeur, soit $r$ le plus petit indice où leurs coefficients diffèrent. Après division de la différence par $(-2)^r$, on obtient un entier impair égal à $0$, contradiction. Pour $m=0$, l'unique polynôme est le polynôme nul.

## Exercice 9

Les opérations usuelles préservent les coefficients dans $A$, et $A[X]\subset K[X]$ est intègre. Si $FG=1$, $\deg F+\deg G=0$, donc $F,G$ sont constants. Ainsi $A[X]^\times=A^\times$.

## Exercice 10

1. Comparer le coefficient de $X^n$ dans $(1+X)^p(1+X)^q=(1+X)^{p+q}$ donne $\sum_{k=0}^n\binom pk\binom q{n-k}=\binom{p+q}n$. 2. Prendre $p=q=n$ donne $\sum_{k=0}^n\binom nk^2=\binom{2n}n$.

## Exercice 11

Posons $a_k=\binom nk-\binom n{k-1}$, en convenant que les coefficients hors $0,\ldots,n$ sont nuls. On a $a_{n+1-k}=-a_k$, donc $\sum_{k=0}^{\lfloor n/2\rfloor}a_k^2=\frac12\sum_{k=0}^{n+1}a_k^2$. Or, par Vandermonde,


```math
\sum_{k=0}^{n+1}a_k^2
=2\sum_{k=0}^n\binom nk^2-2\sum_{k=0}^{n-1}\binom nk\binom n{k+1}
=2\binom{2n}n-2\binom{2n}{n-1}
=\frac{2}{n+1}\binom{2n}n.
```


La formule demandée suit.

## Exercice 12

### 1

Pour $r=n+k$,


```math
k\binom{2n}{n+k}=n\left(\binom{2n-1}{n+k-1}-\binom{2n-1}{n+k}\right).
```


La somme télescope :


```math
\boxed{\sum_{k=0}^nk\binom{2n}{n+k}=n\binom{2n-1}n}.
```



### 2

Poser $w_{k,\ell}=\binom nk\binom n\ell$. Les identités $\sum_k\binom nk=2^n$ et $\sum_k k\binom nk=n2^{n-1}$ donnent


```math
\sum_{k,\ell}(k+\ell)w_{k,\ell}=2\cdot n2^{n-1}\cdot2^n=n4^n.
```


Pour $d\ge0$, la convolution de Vandermonde donne


```math
\sum_{\ell=0}^{n-d}\binom n{\ell+d}\binom n\ell=\binom{2n}{n+d}.
```


Donc, par la question 1,


```math
\sum_{k,\ell}|k-\ell|w_{k,\ell}=2\sum_{d=1}^nd\binom{2n}{n+d}=2n\binom{2n-1}n=n\binom{2n}n.
```


Avec $\max(k,\ell)=(k+\ell+|k-\ell|)/2$ et $\min(k,\ell)=(k+\ell-|k-\ell|)/2$,


```math
\boxed{\sum_{k,\ell}\max(k,\ell)w_{k,\ell}=n2^{2n-1}+\frac n2\binom{2n}n},
```




```math
\boxed{\sum_{k,\ell}\min(k,\ell)w_{k,\ell}=n2^{2n-1}-\frac n2\binom{2n}n}.
```



## Autocorrection C

$P-X^3$ s’annule en tout entier naturel. Un polynôme non nul n’ayant qu’un nombre fini de racines, $P=X^3$.

## Exercice 13

Soit $P\in\mathbb R[X]$ de degré impair. Son terme dominant implique que $P(x)\to+\infty$ quand $x\to+\infty$ et $P(x)\to-\infty$ quand $x\to-\infty$, ou l’inverse. Le théorème des valeurs intermédiaires donne une racine réelle.

## Exercice 14

Séparer les puissances paires et impaires : $P(X)=A(X^2)+XB(X^2)$ avec $A,B\in\mathbb Q[X]$. L'égalité $P(\sqrt2)=0$ s'écrit


```math
A(2)+\sqrt2\,B(2)=0.
```


Comme $A(2),B(2)\in\mathbb Q$ et $\sqrt2\notin\mathbb Q$, on a $A(2)=B(2)=0$. Donc


```math
P(-\sqrt2)=A(2)-\sqrt2\,B(2)=0.
```



## Exercice 15

1. Si $P$ est non constant de degré $d$ et coefficient dominant $a$, alors $P(X+1)-P(X)$ a degré $d-1$ et coefficient dominant $ad\ne0$, contradiction avec la périodicité. Donc $P$ est constant. 2. Une solution est $P=X(X-1)/2$, car $P(X+1)-P(X)=X$. Toute différence de deux solutions est périodique, donc constante par 1. Ainsi $P=X(X-1)/2+c$, $c\in\mathbb C$.

## Exercice 16

Écrivons $P=A+iB$, avec $A,B\in\mathbb R[X]$. Pour chaque réel $\alpha$ de l’énoncé, $B(\alpha)=0$. Le polynôme $B$ a une infinité de racines, donc $B=0$ et $P\in\mathbb R[X]$.

## Exercice 17

Le polynôme nul convient. Pour une solution non nulle, l’identité avec $y=1$ donne $P(1)=1$. Avec $x=0$, $P(0)=P(0)P(y)$; si $P(0)=1$, alors $P\equiv1$. Sinon $P(0)=0$. Écrivons $P(X)=\sum a_kX^k$. L’identité $P(XY)=P(X)P(Y)$ donne $a_k=a_k^2$ et $a_ia_j=0$ pour $i\ne j$. Les coefficients sont donc $0$ ou $1$, et exactement l’un d’eux vaut $1$. Comme $P(1)=1$, les solutions sont $P=X^n$, $n\in\mathbb N$, y compris $P=1$ pour $n=0$, ainsi que $P=0$.

## Exercice 18

En $X=0$, l’équation donne $P(0)=0$. En $X=-1$, elle donne $P(1)=0$. Pour tout entier $k\ge1$, si $P(k)=0$, l’équation en $k$ donne $kP(k+2)=0$, donc $P(k+2)=0$. Comme $P(1)=0$, tous les entiers positifs impairs sont racines. Ainsi $P=0$, qui est bien solution.

## Exercice 19

### 1

Si $P(a)=0$, évaluer l'identité en $a$ puis en $a+1$ donne


```math
P(a^2)=P(a)P(a-1)=0,\qquad P((a+1)^2)=P(a+1)P(a)=0.
```



### 2

Le nombre $0$ n'est pas racine. Sinon, la suite $u_0=0$, $u_{k+1}=(u_k+1)^2$ serait entièrement formée de racines et strictement croissante, donnant une infinité de racines au polynôme non nul $P$.

Pour toute racine $a\ne0$, les $a^{2^k}$ sont encore des racines. Si $0<|a|<1$, leurs modules sont strictement décroissants ; si $|a|>1$, ils sont strictement croissants. La finitude de l'ensemble des racines impose donc $|a|=1$.

Le nombre $(a+1)^2$ est aussi une racine ; le résultat précédent lui donne $|(a+1)^2|=1$, donc $|a+1|=1$. Ainsi


```math
1=|a+1|^2=|a|^2+1+2\operatorname{Re}a=2+2\operatorname{Re}a,
```




```math
\operatorname{Re}a=-\frac12,\qquad\operatorname{Im}a=\pm\frac{\sqrt3}{2}.
```


Toutes les racines appartiennent donc à $\{j,j^2\}$, où $j=e^{2i\pi/3}$.

## Exercice 20

### 1–2

Poser $T_0=1$, $T_1=X$ et $T_{n+2}=2XT_{n+1}-T_n$. L'identité


```math
\cos((n+2)\theta)=2\cos\theta\cos((n+1)\theta)-\cos(n\theta)
```


donne par récurrence $T_n(\cos\theta)=\cos(n\theta)$. Deux polynômes ayant cette propriété coïncident sur $[-1,1]$, donc sont égaux. La relation de récurrence est ainsi établie pour la famille définie dans l'énoncé.

### 3

$T_0$ a degré $0$ et coefficient dominant $1$. Pour $n\ge1$, la récurrence donne $\deg T_n=n$ et un coefficient dominant $2^{n-1}$.

Pour $n\ge1$,


```math
T_n\left(\cos\frac{(2k-1)\pi}{2n}\right)=0\qquad(1\le k\le n).
```


Ces $n$ nombres sont distincts et appartiennent à $]-1,1[$ ; ils épuisent les racines complexes du polynôme de degré $n$, et sont tous simples. $T_0=1$ n'a aucune racine.

## Exercice 21

1. Si $Q\circ P=R\circ P$ et $P$ non constant, l’image de $P:\mathbb C\to\mathbb C$ est infinie. Le polynôme $Q-R$ s’annule sur cette image, donc est nul. 2. Pour $P=0,Q=0,R=X$, les compositions coïncident sans que $Q=R$.

## Exercice 22

### 1

Pour $P\in\mathbb R[X]$, l'identité $|P(x)|=1$ sur $[0,1]$ donne $P(x)^2-1=0$ sur une infinité de points, donc $(P-1)(P+1)=0$ dans $\mathbb R[X]$. Par intégrité,


```math
\boxed{P=1\quad\text{ou}\quad P=-1}.
```



### 2

Pour $P=\sum a_kX^k\in\mathbb C[X]$, poser $\overline P=\sum\overline{a_k}X^k$. Pour $x$ réel, $P(x)\overline P(x)=|P(x)|^2$. Donc $P\overline P=1$ par identité polynomiale. Comme $P\ne0$,


```math
2\deg P=\deg(P\overline P)=0.
```


Les solutions sont exactement $\boxed{P=c,\quad c\in\mathbb C,\ |c|=1}$.

## Exercice 23

Si $P\ne0$ est de degré $d$, pour $P(X)=\sum_{k=0}^da_kX^k$, posons $P^*(X)=\sum_{k=0}^d\overline{a_k}X^{d-k}$. Sur $|z|=1$, $|P(z)|=1$ donne $P(z)P^*(z)=z^d$; l’identité vaut donc dans $\mathbb C[X]$. Toute racine non nulle de $P$ annulerait le membre gauche mais pas $z^d$; les racines de $P$ sont toutes nulles. Ainsi $P=cX^d$, et $|c|=1$. Les constantes solutions sont incluses pour $d=0$.

## Exercice 24

Posons $Q=P-X^2$. On aurait $Q(n)=(-1)^n$, donc $Q(n+1)-Q(n)=-2(-1)^n$. Or la différence d’un polynôme est un polynôme; un polynôme qui vaut alternativement $2$ et $-2$ sur tous les entiers ne peut exister: s’il est non constant, son signe est fixe à partir d’un certain rang; s’il est constant, il ne peut alterner. Aucun $P$ ne convient.

## Exercice 25

1. $\exp$ n’est pas constante. Pour tout polynôme non constant, $|P(x)|\to+\infty$ lorsque $x\to-\infty$, tandis que $e^x\to0$ ; aucun polynôme ne représente donc $\exp$. 2. Si un polynôme $P$ représentait la conjugaison, alors $P(x)=x$ pour tout réel $x$, donc $P=X$. Mais $P(i)=i\ne-i=\overline i$, contradiction. 3. (a) $\cos$ est bornée et non constante, donc non polynomiale. (b) Sur $\pi\mathbb Z$, ses valeurs alternent $1,-1$; un polynôme non constant est non borné sur cette suite et une constante ne convient pas. (c) L’égalité sur $[0,2\pi]$ imposerait l’égalité des fonctions et de toutes leurs dérivées sur l’intérieur; or un polynôme a une dérivée d’ordre supérieur identiquement nulle, contrairement au cosinus. (d) Oui: $E=2\pi\mathbb Z$, où la restriction est la constante $1$.

## Exercice 26

Si $P$ est constant, il ne peut égaler $\ln x$ sur une demi-droite. Si son degré $d\ge1$, $P(x)/x^d$ tend vers son coefficient dominant non nul, tandis que $\ln x/x^d\to0$; contradiction.

## Exercice 27

(i) Un polynôme qui tend vers $0$ en $+\infty$ est nul, alors que $1/k\ne0$. (ii) $P(k)^2=k^2+1$ pour tout entier positif entraînerait l’identité $P(X)^2=X^2+1$, puisque le polynôme différence a une infinité de racines; Cette identité imposerait $\deg P=1$, donc $P$ aurait une racine réelle, tandis que $X^2+1$ n'en a aucune. Contradiction. (iii) Pour $d=\deg P\ge0$, $P(k+1)/P(k)\to1$ si $P\ne0$, tandis que $2^{k+1}/2^k=2$.

## Exercice 28

$R=Q-P\ne0$. Le terme dominant de $R$ fixe son signe sur une demi-droite $[A,+\infty[$. Ainsi $P<Q$ partout à partir de $A$, ou $P>Q$ partout à partir de $A$.

## Exercice 29

1. Pour une racine $\zeta$, $\zeta^n=-\sum_{k<n}a_k\zeta^k$, donc $r^n\le\sum_{k<n}|a_k|r^k$, où $r=|\zeta|$. Si $r>0$, diviser par $r^{n-1}$ donne $r\le\sum_{\ell=0}^{n-1}|a_{n-1-\ell}|/r^\ell$. 2. Si $r>1$, chaque $r^{k-n+1}\le1$, donc $r\le\sum|a_k|$; si $r\le1$, la borne est immédiate. 3. Posons $M=\max_{k<n}|a_k|$. Si $r>1+M$, alors


```math
r^n\le M\sum_{k=0}^{n-1}r^k=M\frac{r^n-1}{r-1}<r^n,
```


contradiction. Ainsi $r\le1+M$.

## Exercice 30

L'hypothèse doit inclure $a_n>0$. Sans elle, $P=1-2X$ satisfait $a_0>0$ et $a_0\ge a_1$, mais possède la racine $1/2$.

### 1

Supposer donc $a_0\ge\cdots\ge a_n>0$. Si $P(z)=0$ et $\rho=|z|<1$, l'identité


```math
(1-z)P(z)=a_0-\sum_{k=1}^n(a_{k-1}-a_k)z^k-a_nz^{n+1}
```


entraîne


```math
a_0\le\sum_{k=1}^n(a_{k-1}-a_k)\rho^k+a_n\rho^{n+1}<\sum_{k=1}^n(a_{k-1}-a_k)+a_n=a_0.
```


La stricte inégalité provient notamment de $a_n>0$ et $\rho^{n+1}<1$. Contradiction ; toutes les racines ont un module au moins égal à $1$.

### 2

Pour tous les $a_k>0$, poser $r=\min_{0\le k<n}a_k/a_{k+1}>0$. Alors $a_kr^k\ge a_{k+1}r^{k+1}$, donc les coefficients de $P(rX)$ décroissent. La question 1 donne $|z|\ge r$ pour toute racine $z$ de $P$.

Appliquer cette borne au polynôme réciproque $X^nP(1/X)$, dont les racines sont les $1/z$ et dont les rapports successifs ont pour minimum $1/R$, avec $R=\max_k a_k/a_{k+1}$. Alors $|1/z|\ge1/R$, soit $|z|\le R$.



```math
\boxed{r\le|z|\le R}.
```



## Exercice 31

### 1

Si $M-\lambda I$ est singulière, choisir $v\ne0$ tel que $Mv=\lambda v$, puis un indice $i$ où $|v_i|=\max_j|v_j|>0$. La ligne $i$ donne


```math
|\lambda-m_{ii}|\,|v_i|\le\sum_{j\ne i}|m_{ij}|\,|v_j|\le R_i|v_i|.
```


Donc $\lambda\in D(m_{ii},R_i)$. La contraposition donne l'inversibilité demandée.

### 2

Travailler avec la transposée $C(P)^T$, qui est singulière en même temps que $C(P)$. Les $n-1$ premières équations de $C(P)^Tv=\lambda v$ donnent $v_{k+1}=\lambda v_k$. Ainsi $v=v_1(1,\lambda,\ldots,\lambda^{n-1})^T$, et $v_1\ne0$ si $v\ne0$.

La dernière équation devient


```math
-\sum_{k=0}^{n-1}a_k\lambda^k=\lambda^n\iff P(\lambda)=0.
```


Réciproquement, si $P(\lambda)=0$, le vecteur $(1,\lambda,\ldots,\lambda^{n-1})^T$ est propre pour $C(P)^T$. Donc


```math
C(P)-\lambda I\text{ singulière}\iff P(\lambda)=0.
```



### 3

La conclusion imprimée est fausse pour $n\ge3$. Pour $P=X^3-\frac34X-1$, les deux disques imprimés sont $D(0,1)$, mais $P(1)=-3/4<0$ et $P(3/2)=5/4>0$. Le polynôme a donc une racine réelle dans $]1,3/2[$, hors de ces disques.

Les lignes de la matrice compagnon donnent en revanche, pour $n\ge2$,


```math
Z(P)\subset D(-a_{n-1},1)\ \cup\ D\left(0,1+\max_{0\le k\le n-2}|a_k|\right).
```


En effet, la première ligne a pour rayon $|a_0|$, les lignes intermédiaires ont pour rayons $1+|a_k|$, et la dernière ligne a pour centre $-a_{n-1}$ et rayon $1$.

L'application à la transposée donne également


```math
Z(P)\subset D(0,1)\ \cup\ D\left(-a_{n-1},\sum_{k=0}^{n-2}|a_k|\right).
```


Pour $n=1$, l'unique racine est $-a_0$.

## Autocorrection D

Le reste affine $R$ prend en $a,b$ les valeurs $P(a),P(b)$. L’interpolation donne


```math
R(X)=\frac{P(a)(X-b)-P(b)(X-a)}{a-b}.
```



## Exercice 32

(i) Le reste est affine et vaut $1$ en $1$, $2^n$ en $2$; il est $(2^n-1)X+2-2^n$. (ii) Modulo $(X-1)^2$, $X^n=1+n(X-1)+(X-1)^2S$, donc le reste est $nX+1-n$. (iii) Dans le quotient par $X^2+1$, $X^2=-1$; le reste est $\cos(nt)+X\sin(nt)$, puisque $(\cos t+X\sin t)^n=\cos(nt)+X\sin(nt)$.

## Exercice 33

Modulo $X^2+X+1$, $X^3=1$. Les exposants $42,1729,11111$ sont congrus à $0,1,2$ modulo $3$; la somme est donc congrue à $1+X+X^2=0$. Le reste est nul.

## Exercice 34

La factorisation exacte est


```math
P_1=(X-i)(X-2-i)(X-1+3i),\qquad
P_2=(X+3)(X-3i)(X-2+i)(X-1+2i).
```


Les racines sont respectivement $i,2+i,1-3i$ et $-3,3i,2-i,1-2i$.

## Exercice 35

$A-I=\frac12\begin{pmatrix}1&1\\-1&-1\end{pmatrix}$, donc $(A-I)^2=0$. Modulo $(X-1)^2$, $X^{100}=1+100(X-1)=100X-99$. Alors


```math
A^{100}=I+100(A-I)=\begin{pmatrix}51&50\\-50&-49\end{pmatrix}.
```



## Exercice 36

Posons $D=x^2+2x+3$. Si $D\mid x^3$, l’identité $x^3=(x-2)D+x+6$ donne $D\mid x+6$. Pour $x\le-7$ ou $x\ge2$, $D>|x+6|$, donc c’est impossible. Il reste $x=-6,\ldots,1$; le test donne seulement $x=-6$, pour lequel $y=-8$, et $x=0$, pour lequel $y=0$. Les points sont $(-6,-8),(0,0)$.

## Exercice 37

Si $B=0$, l'hypothèse impose $A=0$ et le quotient $0$ convient. Pour $B\ne0$, la division de $A$ par $B$ dans $K[X]$ donne $A=BQ_0+R$, $\deg R<\deg B$. Dans $L[X]$, $B\mid A$, donc $B\mid R$; comme $\deg R<\deg B$, $R=0$. Le quotient $Q_0$ appartient à $K[X]$.

## Exercice 38

Diviser successivement par le terme dominant unitaire de $B$ soustrait à chaque étape un multiple de $B$ à coefficients entiers; on obtient $Q,R\in\mathbb Z[X]$, $\deg R<\deg B$. L’unicité résulte de l’unicité de la division dans $\mathbb Q[X]$.

## Autocorrection E

$P_0=X^k$. Si $P_n=c_nX^k$, la récurrence donne $c_{n+1}=kc_n$, donc


```math
P_n=k^nX^k\quad(n\ge1).
```


En particulier, pour $k=0$, $P_0=1$ et $P_n=0$ pour tout $n\ge1$.

## Exercice 39

Si $\operatorname{car}K=0$, prendre $H=XK[X]$: la dérivation y est injective car ses seules constantes sont nulles dans $H$, et surjective car toute polynôme a une primitive nulle en $0$. Si $\operatorname{car}K=p>0$, aucune partie $H$ ne convient: $X^{p-1}$ n’est la dérivée d’aucun polynôme, car le coefficient de $X^{p-1}$ dans une dérivée vaut $p c_p=0$.

## Exercice 40

En caractéristique $0$, la somme est finie puisque $P^{(k)}=0$ pour $k>\deg P$. Poser


```math
F(X)=\sum_{k\ge0}\frac{(-1)^k}{(k+1)!}P^{(k)}(X)X^{k+1}.
```


Alors


```math
F'=\sum_{k\ge0}\frac{(-1)^k}{(k+1)!}P^{(k+1)}X^{k+1}+\sum_{k\ge0}\frac{(-1)^k}{k!}P^{(k)}X^k=P,
```


les termes d'indice positif s'annulant après réindexation de la première somme. Chaque terme de $F$ s'annule en $0$. Deux primitives diffèrent d'une constante, donc $F$ est l'unique primitive nulle en $0$.

En caractéristique positive, les factorielles ne sont pas toutes inversibles et une primitive peut ne pas exister ; la formule nécessite donc cette restriction.

## Exercice 41

En caractéristique $0$.

(i) En caractéristique nulle, un polynôme non constant a une dérivée de degré strictement inférieur; une constante égale à sa dérivée doit être nulle. Donc $P=0$. (ii) Si $P\ne0$ est de degré $d$, les degrés donnent $2d-2=d$, donc $d=2$. Écrire $P=aX^2+bX+c$ et comparer dans $(2aX+b)^2=4(aX^2+bX+c)$ donne $a=1,c=b^2/4$. Ainsi $P=(X+b/2)^2$; ajouter la solution $P=0$.

## Exercice 42

En caractéristique $0$, $P=0$ convient et aucune constante non nulle ne convient. Si $\deg P=1$, $P''=0$, donc l'équation est impossible. Pour $d=\deg P\ge2$, les degrés donnent $d=(d-1)+(d-2)$, donc $d=3$.

Écrire $P=aX^3+bX^2+cX+e$, avec $a\ne0$. L'identification dans $P(2X)=P'P''$ donne


```math
18a^2=8a,\quad18ab=4b,\quad6ac+4b^2=2c,\quad2bc=e.
```


La première relation impose $a=4/9$. La deuxième devient $8b=4b$, donc $b=0$. La troisième devient $(8/3)c=2c$, donc $c=0$, puis $e=0$.



```math
\boxed{P=0\quad\text{ou}\quad P=\frac49X^3}.
```


La substitution directe vérifie ces deux solutions.

## Exercice 43

En caractéristique $0$. Pour $P=\sum a_kX^k$, le coefficient de $X^k$ dans $X(X+1)P''+(X+2)P'-P$ vaut


```math
(k+1)(k+2)a_{k+1}+(k^2-1)a_k.
```


À $k=0$, $a_1=a_0/2$; à $k=1$, $a_2=0$; puis $a_k=0$ pour $k\ge2$. Les solutions sont $P=c(1+X/2)$.

## Exercice 44

Taylor en $0$ et en $1$ donne


```math
P(X+1)-P(X)=\sum_{k=0}^{n-1}\frac{P^{(k)}(1)-P^{(k)}(0)}{k!}X^k,
```


le terme d’ordre $n$ s’annulant aussi car $P^{(n)}$ est constant. Par hypothèse la différence est nulle. Un polynôme périodique de période $1$ est constant (sinon sa différence $P(X+1)-P(X)$ aurait degré $n-1$); c’est incompatible avec $\deg P=n\ge1$. Aucun.

## Exercice 45

En caractéristique $0$, l'identité $AB'-BA'=1$ impose $A\ne0$ et $B\ne0$. Si leurs degrés $r,s$ diffèrent, le coefficient dominant du membre gauche est le produit des coefficients dominants multiplié par $s-r\ne0$. Donc


```math
\deg(AB'-BA')=r+s-1=0,\qquad r+s=1.
```



Si $r=s=d$, soustraire à $B$ un multiple scalaire de $A$ annulant son terme dominant : $C=B-cA$, avec $\deg C<d$. L'identité devient $AC'-CA'=1$, donc $C\ne0$. Les degrés de $A,C$ étant distincts, le cas précédent impose $d+\deg C=1$, d'où $d\le1$.

Les deux polynômes sont donc affines. Pour $A=aX+b$, $B=cX+d$,


```math
AB'-BA'=bc-ad.
```


Ainsi


```math
\boxed{(A,B)=(aX+b,cX+d),\qquad bc-ad=1}.
```


Cette classification nécessite la caractéristique $0$ : en caractéristique $p>0$, le couple $(1,X+X^p)$ est aussi solution.

## Exercice 46

Si $F'=P$, la condition équivaut à $F(k+1)-F(k)=k+1$ pour tout entier $k$, donc l’identité polynomiale $F(X+1)-F(X)=X+1$. Une solution est $F=X(X+1)/2$, à une constante près; ainsi $P=X+1/2$.

## Exercice 47

1. La moyenne de $aX+b$ sur $[x-1,x+1]$ vaut $ax+b$, donc $H\cap\mathbb R_1[X]=\mathbb R_1[X]$. Pour $aX^2+bX+c$, la moyenne est $aX^2+bX+c+a/3$; l’égalité impose $a=0$, donc $H\cap\mathbb R_2[X]=\mathbb R_1[X]$. 2. Dériver l’identité donne $P'(x)=\frac12(P(x+1)-P(x-1))$, qui est également la moyenne de $P'$; ainsi $P'\in H$. 3. Si $\deg P=d\ge2$, la moyenne de $P$ est $P+P''/3!+P^{(4)}/5!+\cdots$; son terme de degré $d-2$, provenant de $P''/6$, ne peut s’annuler. Donc $H=\mathbb R_1[X]$.

## Exercice 48

1. Par récurrence, $\deg A_n=2n$, coefficient dominant $1$. 2. $A_{n+1}(0)=A_n(0)$, donc $A_n(0)=0$. 3. Il existe alors un unique $B_n$ tel que $A_n=XB_n$. 4. $B_1=X+1$; la récurrence devient $B_{n+1}=(X^2+2)B_n+XB_n'$. 5. $B_{n+1}(0)=2B_n(0)$, donc $B_n(0)=2^{n-1}$; comme $A_n'(0)=B_n(0)$, $A_n'(0)=2^{n-1}$.

## Exercice 49

La fonction tangente est $C^\infty$ sur tout intervalle où elle est définie. $P_0=X$ et, si $\tan^{(n)}=P_n(\tan)$, alors $\tan^{(n+1)}=(1+\tan^2)P_n'(\tan)$; poser $P_{n+1}=(1+X^2)P_n'$. La récurrence donne des coefficients dans $\mathbb N$ et $\deg P_n=n+1$.

## Exercice 50

### 1

Poser $H_0=1$ et $H_{n+1}=H_n'-2XH_n$. La règle de dérivation du produit donne


```math
(H_ne^{-x^2})'=(H_n'-2xH_n)e^{-x^2}=H_{n+1}e^{-x^2}.
```


Par récurrence, $g$ est indéfiniment dérivable et $g^{(n)}=H_ne^{-x^2}$. L'unicité vient de ce que $e^{-x^2}$ ne s'annule pas : deux polynômes convenant coïncideraient sur $\mathbb R$.

### 2

Si $H_n$ a degré $n$ et coefficient dominant $(-2)^n$, le terme $-2XH_n$ a degré $n+1$, tandis que $H_n'$ a degré inférieur. Donc $H_{n+1}$ a coefficient dominant $(-2)^{n+1}$. Les deux termes de la récurrence ont la parité opposée à celle de $H_n$. Ainsi $\deg H_n=n$ et $H_n(-X)=(-1)^nH_n(X)$.

### 3

Dériver $g'=-2xg$ exactement $n$ fois. La formule de Leibniz donne, pour $n\ge1$,


```math
H_{n+1}=-2XH_n-2nH_{n-1}.
```


Comparer avec $H_{n+1}=H_n'-2XH_n$ donne $H_n'=-2nH_{n-1}$. En remplaçant $n$ par $n+1$,


```math
\boxed{H_{n+1}'=-2(n+1)H_n}.
```



### 4

L'égalité précédente et la récurrence donnent $H_{n+1}(0)=-2nH_{n-1}(0)$, avec $H_0(0)=1$ et $H_1(0)=0$. Donc


```math
\boxed{g^{(2m)}(0)=(-1)^m\frac{(2m)!}{m!},\qquad g^{(2m+1)}(0)=0}.
```



## Exercice 51

Si $P'$ est nul, $P$ est constant. Sinon le terme dominant de $P'$ impose un signe fixe sur $[A,+\infty[$ pour $A$ assez grand; $P$ y est monotone.

## Exercice 52

Le polynôme n'est pas constant. Puisque $P(n)\ge0$ pour tout $n\in\mathbb N$, son coefficient dominant est positif.

Si $d=\deg P\ge2$, alors $P(n+1)-P(n)\to+\infty$. Choisir $N$ tel que $P$ soit strictement croissant sur les entiers $n\ge N$ et que $P(n+1)-P(n)>1$. Choisir ensuite $m\ge N$ tel que $P(m)>\max_{0\le k<N}P(k)$. L'entier $P(m)+1$ n'est atteint ni par les indices $k\le m$, ni par les indices $k\ge m+1$, contradiction à la surjectivité.

Donc $P=aX+b$. Comme $P(0)$ et $P(1)$ sont entiers, $a,b\in\mathbb Z$, avec $a>0$, $b\ge0$. La valeur $0$ doit être atteinte, donc $b=0$, puis la valeur $1$ impose $a=1$.



```math
\boxed{P=X}.
```



## Exercice 53

Pour $x\ge a$, la formule de Taylor, exacte pour un polynôme, donne $P(x)=\sum_{k=0}^{d}P^{(k)}(a)(x-a)^k/k!$. Chaque terme est positif ou nul et le terme constant $P(a)$ est strictement positif; ainsi $P(x)>0$.

## Autocorrection F

Les notations $z_k$ et $x_k$ désignent les mêmes nœuds distincts. Le polynôme $\sum_{k=0}^nL_k-1$, de degré au plus $n$, s'annule en chacun des $n+1$ nœuds. Donc


```math
\boxed{\sum_{k=0}^nL_k=1}.
```


Pour $n\ge1$, le polynôme $\sum_{k=0}^nx_kL_k-X$ a aussi degré au plus $n$ et s'annule aux mêmes nœuds, donc


```math
\boxed{\sum_{k=0}^nx_kL_k=X}.
```


Pour $n=0$, la deuxième somme vaut la constante $x_0$.

## Exercice 54

Pour $n\ge1$, les nœuds $k/n$, $0\le k\le n$, sont distincts. Poser


```math
L_k(t)=\prod_{j\ne k}\frac{t-j/n}{k/n-j/n},\qquad\lambda_k=\int_0^1L_k(t)\,dt.
```


L'interpolation de Lagrange donne, pour tout $P\in\mathbb R_n[X]$,


```math
P(t)=\sum_{k=0}^nP(k/n)L_k(t).
```


En intégrant,


```math
\boxed{\int_0^1P(t)\,dt=\sum_{k=0}^n\lambda_kP(k/n)}.
```


Pour $n=0$, l'expression $k/n$ imprimée n'est pas définie ; la version pour les constantes est $\int_0^1P=P(0)$, avec $\lambda_0=1$.

## Exercice 55

$Q=(X+1)P-X$ a degré au plus $n+1$, et $Q(k)=0$ pour $k=0,\ldots,n$; donc $Q=c\prod_{k=0}^n(X-k)$. À $X=-1$, $Q(-1)=1$, d’où $c=(-1)^{n+1}/(n+1)!$. Puis $Q(n+1)=(-1)^{n+1}$, donc


```math
P(n+1)=\frac{n+1+(-1)^{n+1}}{n+2}.
```



## Exercice 56

Pour $n\ge1$, l'interpolation en $1,\ldots,n$ donne


```math
P(n+1)=\sum_{k=1}^nr^k\prod_{\substack{1\le j\le n\\j\ne k}}\frac{n+1-j}{k-j}.
```


Le produit vaut


```math
\frac{n!/(n+1-k)}{(k-1)!(-1)^{n-k}(n-k)!}=(-1)^{n-k}\binom n{k-1}.
```


Donc, en posant $j=k-1$,


```math
P(n+1)=r(-1)^{n-1}\sum_{j=0}^{n-1}\binom nj(-r)^j=r(-1)^{n-1}\bigl((1-r)^n-(-r)^n\bigr).
```


Ainsi


```math
\boxed{P(n+1)=r^{n+1}-r(r-1)^n}.
```



## Exercice 57

Le polynôme $Q=XP-1$ a degré au plus $n+1$ et s'annule en $1,\ldots,n+1$. Comme $Q(0)=-1$,


```math
Q(X)=\frac{(-1)^n}{(n+1)!}\prod_{k=1}^{n+1}(X-k).
```


La dérivation du produit en $0$ donne


```math
P(0)=Q'(0)=Q(0)\sum_{k=1}^{n+1}\frac1{-k}=\boxed{\sum_{k=1}^{n+1}\frac1k}.
```



## Exercice 58

Le cas $P=0$ est immédiat. Sinon, soit $d=\deg P$. Choisissons $d+1$ éléments distincts $x_0,\ldots,x_d\in K$, possible car $K$ est infini. Les valeurs $P(x_i)$ appartiennent à $K$; la formule de Lagrange écrit $P$ comme combinaison de polynômes de $K[X]$ avec coefficients $P(x_i)\in K$. Donc $P\in K[X]$.

## Exercice 59

Divisons $P=(X^q-X)Q+R$, $\deg R<q$. Pour $x\in K$, $x^q=x$, donc $P(x)=R(x)$. Si (i) est vraie, $R$ prend des valeurs dans $K$; interpoler sur les $q$ éléments de $K$ montre $R\in K[X]$, d’où (ii). Réciproquement, (ii) donne $P(x)=R(x)\in K$ pour tout $x\in K$.

## Exercice 60

Si $K=\mathbb F_q$, pour $q>2$ la fonction est représentée par $X^{q-2}$; pour $q=2$, elle est représentée par $X$. Si $K$ est infini et $P(0)=0,\ P(x)=1/x$ pour $x\ne0$, le polynôme $XP(X)-1$ s’annule en tout $x\in K^\times$, donc serait nul, mais sa valeur en $0$ est $-1$. Impossible. La condition est donc que $K$ soit fini.

## Exercice 61

Modulo $2$, tout entier est congru à $0$ ou $1$, et $P(0),P(1)$ sont impairs. Ainsi $P(n)$ est impair pour tout entier $n$, donc ne peut être nul.

## Exercice 62

Si $P$ est non constant, fixons $a\in\mathbb Z$; $P(a)$ est premier. Pour $t=a+mP(a)$, $P(t)\equiv P(a)\equiv0\pmod{P(a)}$. Le polynôme non constant $P$ est non borné sur cette progression dans au moins une direction; on peut choisir $m$ tel que $P(t)>P(a)$. Cette valeur, supposée première, est divisible par $P(a)$ et strictement plus grande, contradiction. Donc $P$ est constant (sa valeur est un nombre premier).

## Exercice 63

### 0

Dans $\mathbb F_7^\times$,


```math
3^0,3^1,3^2,3^3,3^4,3^5\equiv1,3,2,6,4,5\pmod7.
```


Ces puissances épuisent les six éléments ; $3$ est d'ordre $6$. Les générateurs sont $3^k$ avec $\gcd(k,6)=1$, donc exactement $3$ et $5$.

### 1

Un élément d'ordre divisant $s$ vérifie $x^s=1$. Le polynôme non nul $X^s-1$ a au plus $s$ racines dans le corps $K$.

### 2

Le théorème de Lagrange donne $\operatorname{ord}(g)\mid|G|=n$ pour chaque $g\in G$, donc $S_G\subset D(n)$.

### 3(a)

L'ordre de $x_s^k$ vaut $s/\gcd(k,s)$. Il vaut $s$ exactement pour les $\varphi(s)$ classes d'entiers $k$ premiers à $s$. Le sous-groupe $\langle x_s\rangle$ a donc $\varphi(s)$ générateurs.

### 3(b)

Les $s$ éléments distincts de $\langle x_s\rangle$ sont racines de $X^s-1$. Par 1, ils constituent toutes les racines de ce polynôme dans $K$. Si l'ordre de $g$ divise $s$, alors $g^s=1$, donc $g\in\langle x_s\rangle$.

### 3(c)

Un générateur de $\langle x_s\rangle$ est d'ordre $s$. Réciproquement, un élément de $G$ d'ordre $s$ appartient à ce sous-groupe par 3(b) et, ayant même ordre que le sous-groupe, l'engendre.

### 3(d)

Les ensembles d'éléments d'ordre $s$, pour $s\in S_G$, forment une partition de $G$. Chacun a cardinal $\varphi(s)$ par 3(a)–(c), donc


```math
n=\sum_{s\in S_G}\varphi(s).
```



### 3(e)

Appliquer 3(d) au sous-groupe $\mu_n(\mathbb C)$ des racines $n$-ièmes de l'unité. Il est cyclique, engendré par $e^{2i\pi/n}$, et possède un élément de chaque ordre $s\mid n$, à savoir $e^{2i\pi/s}$. Son ensemble d'ordres est donc exactement $D(n)$, d'où


```math
n=\sum_{s\mid n}\varphi(s).
```



### 4

Comme $S_G\subset D(n)$ et que chaque $\varphi(s)>0$,


```math
\sum_{s\in S_G}\varphi(s)=n=\sum_{s\mid n}\varphi(s)\Longrightarrow S_G=D(n).
```


En particulier $n\in S_G$. Il existe donc $g\in G$ d'ordre $n$, et $G=\langle g\rangle$ est cyclique.

## Exercice 64

L'énoncé nécessite $P$ non constant, ou $P=0$. Pour une constante non nulle $P=c$, les premiers donnant une racine sont exactement les diviseurs premiers de $c$, en nombre fini ; pour $P=0$, tous les premiers conviennent.

Supposer $P$ non constant et, par l'absurde, que seuls les premiers $p_1,\ldots,p_r$ divisent une valeur entière non nulle de $P$. S'il existe une racine entière de $P$, tous les premiers conviennent déjà ; on peut donc supposer qu'aucune valeur entière n'est nulle.

Choisir $a\in\mathbb Z$ et poser $c=P(a)\ne0$, $m=\prod_{j=1}^rp_j$ (produit vide égal à $1$). Le polynôme


```math
Q(T)=\frac{P(a+cmT)}c
```


a des coefficients entiers : son terme constant vaut $1$ et tous les autres coefficients sont divisibles par $m$, par développement de chaque monôme de $P$. Il est non constant et vérifie $Q(t)\equiv1\pmod{p_j}$ pour tout $j$ et tout entier $t$.

Choisir $t\in\mathbb Z$ avec $|Q(t)|>1$. Un diviseur premier $q$ de $Q(t)$ n'appartient pas à $\{p_1,\ldots,p_r\}$, puisque $Q(t)\equiv1$ modulo chacun d'eux. Mais $q\mid cQ(t)=P(a+cmt)$, contradiction.

Il existe donc une infinité de premiers modulo lesquels $P$ possède une racine.

## Exercice 65

Supposer $P(\mathbb Q)=\mathbb Q$. Le polynôme n'est pas constant. En interpolant aux $d+1$ rationnels $0,1,\ldots,d$, où $d=\deg P$, on obtient $P\in\mathbb Q[X]$.

Choisir $D\in\mathbb N^*$ tel que $A=DP=\sum_{k=0}^da_kX^k\in\mathbb Z[X]$, $a_d\ne0$, puis un premier $p$ ne divisant pas $Da_d$. Par surjectivité, il existe une fraction réduite $u/v$, $v>0$, telle que $P(u/v)=1/p$. En multipliant par $pv^d$,


```math
p\sum_{k=0}^da_ku^kv^{d-k}=Dv^d.
```


Modulo $p$, cette égalité impose $p\mid v$, puisque $p\nmid D$. Comme $\gcd(u,v)=1$, $p\nmid u$. Le nombre entier


```math
N=\sum_{k=0}^da_ku^kv^{d-k}
```


vérifie alors $N\equiv a_du^d\not\equiv0\pmod p$.

Si $d\ge2$, $p^2\mid Dv^d=pN$, d'où $p\mid N$, contradiction. Donc $d=1$.

Réciproquement, tout polynôme $aX+b$ avec $a,b\in\mathbb Q$, $a\ne0$, envoie bijectivement $\mathbb Q$ sur $\mathbb Q$, d'inverse $x\mapsto(x-b)/a$.



```math
\boxed{P=aX+b,\qquad a,b\in\mathbb Q,\ a\ne0}.
```


