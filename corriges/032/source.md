# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td32-denombrement.pdf)



```math
F_0=0,\quad F_1=1,\quad F_{r+2}=F_{r+1}+F_r,\qquad\binom ab=0\text{ si }b\notin\{0,\ldots,a\}.
```



## Autocorrection A



```math
\text{1. }|E|=9^7;\qquad\text{2. }|E_1|=9\cdot8\cdots3=9!/2!.
```




```math
\text{3. }|E_2|=4\cdot9^6;\qquad\text{4. }|E_3|=\binom97=36.
```


Pour 3, le dernier chiffre appartient à $\{2,4,6,8\}$ ; pour 4, le choix des sept chiffres détermine leur ordre.

## Autocorrection B

Pour $n\ge1$ :


```math
\text{(i) }2^n;\qquad\text{(ii) }2^n-2;\qquad\text{(iii) }\begin{cases}\binom n{n/2}&n\text{ pair},\\0&n\text{ impair};\end{cases}\qquad\text{(iv) }2.
```


Pour (v), si $a_n$ compte les mots sans deux cafés consécutifs,


```math
a_0=1,\ a_1=2,\quad a_n=a_{n-1}+a_{n-2}\Rightarrow\boxed{a_n=F_{n+2}}.
```


Les mots se terminent par thé, ou par thé-café.
Pour (vi), les longueurs des blocs constants sont $1$ ou $2$. Leur composition ordonnée de $n$ peut être choisie de $F_{n+1}$ façons ; le premier bloc a deux choix.


```math
\boxed{2F_{n+1}\quad(n\ge1).}
```


Pour $n=0$, il y a un mot vide ; il satisfait (i), (iii), (iv), (v), (vi), mais pas (ii).

## Exercice 1



```math
\text{1. }\boxed{\binom nk};\qquad\text{2. }\boxed{2^{n-p}}.
```


Dans 1, on choisit les positions des $1$. Dans 2, les $p-1$ premiers bits sont nuls, le $p$-ième vaut $1$, les suivants sont libres.

## Exercice 2

Une colonne donne un produit $a_ib_i$ égal à $1$ dans un cas, égal à $0$ dans trois cas.


```math
N=\sum_{\substack{k=0\\k\text{ impair}}}^n\binom nk3^{n-k}=\frac{(3+1)^n-(3-1)^n}2=\boxed{\frac{4^n-2^n}2}.
```



## Exercice 3

### 1



```math
u_0=1,\ u_1=2,\qquad u_n=u_{n-1}+u_{n-2}
```


selon que le mot se termine par $b$ ou par $ba$.


```math
\boxed{u_n=F_{n+2}.}
```



### 2



```math
ab\text{ absent}\iff w=b^ka^{n-k}\quad(0\le k\le n)\Rightarrow\boxed{n+1}.
```



### 3



```math
aab\text{ absent}\iff w\in\{b,ab\}^*a^*.
```


Cette écriture est unique : avant chaque $b$, le bloc de $a$ a longueur $0$ ou $1$ ; le dernier bloc de $a$ est libre.
Pour un préfixe de longueur $m$ formé de blocs $b,ab$, il y a $F_{m+1}$ choix.


```math
\boxed{\sum_{m=0}^nF_{m+1}=F_{n+3}-1.}
```



## Autocorrection C

### (i)–(v)



```math
\text{(i) }\binom{32}5;\qquad\text{(ii) }2\binom85;\qquad\text{(iii) }\binom82\binom83;
```




```math
\text{(iv) }\binom{32}5-\binom{28}5;\qquad\text{(v) }\binom{28}5+4\binom{28}4.
```



### (vi)

Le complément comporte cinq hauteurs distinctes, avec quatre couleurs possibles pour chacune :


```math
\boxed{\binom{32}5-\binom85\cdot4^5.}
```



### (vii)

Deux paires et une carte d'une troisième hauteur, ou un full :


```math
\boxed{\binom82\binom42^2\cdot6\cdot4+8\binom43\cdot7\binom42.}
```



### (viii)

Avec l'as de cœur : un autre as, deux autres cœurs et une carte ni as ni cœur. Sans l'as de cœur : deux autres as et trois autres cœurs.


```math
\boxed{3\binom72\cdot21+\binom32\binom73.}
```



### (ix)

Avec l'as de carreau, puis avec l'un des trois autres as :


```math
\boxed{\sum_{j=2}^4\binom7j\binom{21}{4-j}+3\sum_{j=3}^4\binom7j\binom{21}{4-j}.}
```



### (x)

$h$ indique la présence du roi de cœur, $k$ compte les autres rois et $t$ les cœurs non rois.


```math
\boxed{\sum_{h=0}^1\sum_{t=0}^{1-h}\sum_{k=2-h}^3\binom3k\binom7t\binom{21}{5-h-k-t}.}
```



## Autocorrection D



```math
k=0:\quad\{A:\operatorname{diam}A=0\}=\{\{1\},\ldots,\{n\}\}\Rightarrow\boxed n.
```




```math
1\le k<n:\quad\min A=a,\ \max A=a+k,\quad1\le a\le n-k.
```


Les $k-1$ éléments intermédiaires sont libres.


```math
\boxed{(n-k)2^{k-1}\quad(1\le k<n),\qquad0\quad(k\ge n).}
```



## Exercice 4



```math
n=|E|.
```




```math
\text{1. }(\mathbf1_A(x),\mathbf1_B(x))\in\{(0,0),(1,0),(0,1)\}\Rightarrow\boxed{3^n}.
```




```math
\text{2. }(\mathbf1_A(x),\mathbf1_B(x))\in\{(0,0),(0,1),(1,1)\}\Rightarrow\boxed{3^n}.
```




```math
\text{3. }(\mathbf1_A(x),\mathbf1_B(x))\in\{(1,0),(0,1),(1,1)\}\Rightarrow\boxed{3^n}.
```




```math
\text{4. }x\in C\Rightarrow x\in A\cap B;\quad x\notin C\Rightarrow\text{trois choix}\Rightarrow\boxed{3^{n-|C|}}.
```



## Exercice 5

Le produit cartésien visé est $\mathcal P(E)^3$.


```math
X\subset Y\subset Z\Rightarrow E=X\sqcup(Y\setminus X)\sqcup(Z\setminus Y)\sqcup(E\setminus Z).
```




```math
\boxed{4^n.}
```



## Exercice 6

On choisit l'unique élément de $X\cap Y$, puis, pour chaque autre élément, l'une des trois situations $(0,0),(1,0),(0,1)$.


```math
\boxed{n3^{n-1}\quad(n\ge1).}
```


Pour $n=0$, le nombre est nul.

## Exercice 7

Pour une partie de taille $k$, écrivons


```math
1\le a_1<\cdots<a_k\le n,\qquad a_{j+1}\ge a_j+2.
```




```math
b_j=a_j-j+1\Rightarrow1\le b_1<\cdots<b_k\le n-k+1.
```




```math
\boxed{\sum_{k=0}^{\lfloor(n+1)/2\rfloor}\binom{n-k+1}k=F_{n+2}.}
```


La dernière égalité résulte aussi de la récurrence $u_n=u_{n-1}+u_{n-2}$, suivant que $n$ appartient ou non à la partie.

## Exercice 8

### 1



```math
\mathcal A_k=\{A\subset\{1,\ldots,n\}:|A|=k\},\qquad|\mathcal A_k|=\binom nk
```


est une antichaîne pour tout $0\le k\le n$. Une famille réduite à une seule partie est aussi une antichaîne, de cardinal $1$.

### 2(a)



```math
\sigma\in S_n\longmapsto\bigl(\varnothing,\{\sigma(1)\},\ldots,\{\sigma(1),\ldots,\sigma(n)\}\bigr)
```


est une bijection avec les chaînes complètes.


```math
\boxed{n!.}
```



### 2(b)



```math
|X|=k\Rightarrow\boxed{k!(n-k)!}
```


chaînes : les éléments de $X$ sont ajoutés d'abord, puis ceux de son complément.

### 3

Chaque chaîne complète rencontre une antichaîne en au plus une partie. En comptant les couples $(A,\mathcal C)$ avec $A\in\mathcal A\cap\mathcal C$,


```math
\boxed{\sum_{A\in\mathcal A}|A|!(n-|A|)!\le n!.}
```



### 4



```math
\sum_{A\in\mathcal A}\frac1{\binom n{|A|}}\le1,\quad\binom n{|A|}\le\binom n{\lfloor n/2\rfloor}.
```




```math
|\mathcal A|\le\binom n{\lfloor n/2\rfloor}.
```


L'antichaîne $\mathcal A_{\lfloor n/2\rfloor}$ atteint cette borne.

## Exercice 9



```math
n=|E|.
```




```math
\text{(i)}\quad\sum_A|A|=\sum_{x\in E}\#\{A:x\in A\}=\boxed{n2^{n-1}}.
```




```math
\text{(ii)}\quad\sum_{A,B}|A\cap B|=\sum_{x\in E}\#\{(A,B):x\in A\cap B\}=\boxed{n4^{n-1}}.
```




```math
\text{(iii)}\quad\sum_{A,B}|A\cup B|=\sum_{x\in E}\#\{(A,B):x\in A\cup B\}=\boxed{3n4^{n-1}}.
```


Pour $n=0$, les trois sommes valent $0$.

## Exercice 10



```math
\sum_{X\cap Y=\varnothing}(|X|+|Y|)=\sum_{i=1}^n\#\{(X,Y):X\cap Y=\varnothing,\ i\in X\cup Y\}.
```


Pour $i$ : deux choix ; pour chaque autre élément : trois choix.


```math
\boxed{2n3^{n-1}\quad(n\ge1).}
```



## Exercice 11

### 1

L'image d'une application strictement croissante détermine l'application.


```math
\boxed{\binom np.}
```



### 2(a)



```math
c_j=\#f^{-1}(j),\quad c_j\ge0,\quad\sum_{j=1}^nc_j=p.
```


La suite $(c_j)$ détermine l'application croissante. Les $p$ étoiles et $n-1$ barres donnent


```math
\boxed{\binom{n+p-1}{n-1}=\binom{n+p-1}p.}
```



### 2(b)



```math
g(i)=f(i)+i-1\Rightarrow1\le g(1)<\cdots<g(p)\le n+p-1.
```


L'inverse est $f(i)=g(i)-i+1$, d'où le même nombre.

## Exercice 12

### 1



```math
\boxed{S(n,p)=0\ (p>n),\quad S(n,n)=n!,\quad S(n,1)=1,\quad S(n,2)=2^n-2.}
```



### 2

Une unique fibre a taille $2$, les autres taille $1$.


```math
\boxed{S(n+1,n)=\binom{n+1}2n!.}
```



### 3

Distinguons le dernier élément du domaine. Si son image possède un autre antécédent, la restriction est surjective : $pS(n-1,p)$ possibilités. Si sa fibre est un singleton, on choisit son image puis une surjection sur les $p-1$ autres valeurs : $pS(n-1,p-1)$.


```math
\boxed{S(n,p)=p[S(n-1,p)+S(n-1,p-1)].}
```



### 4



```math
T(n,p)=\sum_{k=0}^p(-1)^{p-k}\binom pk k^n.
```


L'identité $k\binom pk=p\binom{p-1}{k-1}$, puis Pascal, donne


```math
T(n,p)=p[T(n-1,p)+T(n-1,p-1)].
```


Les valeurs initiales $T(n,1)=1$, $T(1,p)=\mathbf1_{p=1}$ coïncident avec celles de $S$ ; récurrence :


```math
\boxed{S(n,p)=\sum_{k=0}^p(-1)^{p-k}\binom pk k^n.}
```



## Exercice 13



```math
p^2=p\iff p|_{\operatorname{im}p}=\operatorname{id}.
```


Pour $|\operatorname{im}p|=k$, on choisit cette image de $\binom nk$ façons, puis l'image de chacun des $n-k$ autres éléments parmi les $k$ points fixes.


```math
\boxed{\sum_{k=1}^n\binom nk k^{n-k}\quad(n\ge1).}
```


Pour $n=0$, il existe une application vide.

## Exercice 14



```math
\sigma[A]=A\iff A\text{ est une réunion de cycles de }\sigma.
```


Si $\sigma$ possède $r$ cycles, points fixes compris,


```math
\boxed{2^r.}
```



## Exercice 15

### 1



```math
P_n(X)=\sum_{\sigma\in S_n}X^{o(\sigma)},\quad P_0=1.
```


À partir de $\sigma\in S_n$, l'élément $n+1$ forme un nouveau cycle, ou s'insère après l'un des $n$ éléments d'un cycle existant.


```math
P_{n+1}(X)=(X+n)P_n(X)\Rightarrow\boxed{P_n(X)=X(X+1)\cdots(X+n-1).}
```



### 2



```math
\sum_\sigma o(\sigma)=P_n'(1),\qquad\frac{P_n'(1)}{P_n(1)}=\sum_{k=0}^{n-1}\frac1{1+k}.
```




```math
\boxed{\frac1{n!}\sum_\sigma o(\sigma)=\sum_{k=1}^n\frac1k.}
```



## Exercice 16

### 1



```math
\boxed{D_0=1,\quad D_1=0,\quad D_2=1,\quad D_3=2.}
```



### 2

On choisit les $k$ points fixes, puis un dérangement du complément.


```math
\boxed{\binom nkD_{n-k}.}
```



### 3



```math
n!=\sum_{k=0}^n\binom nkD_{n-k}=\boxed{\sum_{k=0}^n\binom nkD_k.}
```



### 4



```math
D_4=24-(1+6+8)=\boxed9,
```




```math
D_5=120-(1+10+20+45)=\boxed{44}.
```



### 5



```math
\sum_{k=0}^n(-1)^{n-k}\binom nk k!=\sum_{k=0}^n(-1)^{n-k}\binom nk\sum_{j=0}^k\binom kjD_j
```




```math
=\sum_{j=0}^n\binom njD_j\sum_{k=j}^n(-1)^{n-k}\binom{n-j}{k-j}=D_n.
```




```math
\boxed{D_n=n!\sum_{j=0}^n\frac{(-1)^j}{j!}.}
```



## Exercice 17

L'ordre est le ppcm des longueurs des cycles. Pour un ordre premier $p$, les cycles ont longueur $1$ ou $p$, avec un ou deux cycles de longueur $p$.


```math
\boxed{\binom{2p}p(p-1)!+\frac12\binom{2p}p((p-1)!)^2.}
```


Le facteur $1/2$ identifie les échanges des deux cycles.

## Exercice 18

Une permutation de $2n$ éléments possède au plus un cycle de longueur $k>n$.


```math
\#\{\sigma:\text{cycle de longueur }k\}=\binom{2n}k(k-1)!(2n-k)!=\frac{(2n)!}{k}.
```




```math
\boxed{a_n=(2n)!\left(1-\sum_{k=n+1}^{2n}\frac1k\right).}
```




```math
\sum_{k=n+1}^{2n}\frac1k\to\ln2\Rightarrow\boxed{\frac{a_n}{(2n)!}\to1-\ln2.}
```



## Autocorrection E

### 1

On choisit $n$ éléments dans deux ensembles disjoints de taille $n$ :


```math
\binom{2n}n=\sum_{k=0}^n\binom nk\binom n{n-k}=\boxed{\sum_{k=0}^n\binom nk^2.}
```



### 2

Pour des tailles $n_i\in\mathbb N$, dans une réunion disjointe de $p$ ensembles de tailles $n_i$, une partie de taille $q$ a des intersections de tailles $k_i$ telles que $\sum k_i=q$.


```math
\boxed{\binom{n_1+\cdots+n_p}q=\sum_{k_1+\cdots+k_p=q}\prod_{i=1}^p\binom{n_i}{k_i}.}
```



## Exercice 19



```math
\binom ni\binom{n-i}{k-i}=\binom nk\binom ki.
```




```math
\sum_{i=0}^k\binom ni\binom{n-i}{k-i}=\binom nk\sum_{i=0}^k\binom ki=\boxed{2^k\binom nk.}
```


Les deux membres comptent les couples $(K,I)$ avec $|K|=k$ et $I\subset K$ : soit on choisit $K$ puis $I$, soit $I$ puis $K\setminus I$.

## Exercice 20

Pour des $i_j\ge1$ de somme $n$, le produit $i_1\cdots i_p$ compte les choix d'un élément distingué dans chacun de $p$ blocs consécutifs de tailles $i_j$.
En séparant, dans chaque bloc, les éléments avant et après l'élément distingué,


```math
i_j=u_j+1+v_j,\quad u_j,v_j\ge0,\quad\sum_{j=1}^p(u_j+v_j)=n-p.
```


Le nombre de ces $2p$-uplets est


```math
\binom{n-p+2p-1}{2p-1}=\boxed{\binom{n+p-1}{2p-1}.}
```


Les termes avec un $i_j=0$ contribuent $0$ ; si $n<p$, les deux membres sont nuls.

## Exercice 21

### 1



```math
\boxed{\binom{n+m}n=\binom{n+m}m}
```


chemins : on choisit les positions des $n$ pas $E$.

### 2

Tout chemin de $(0,0)$ à $(n,n)$ passe après $n$ pas par un unique $(k,n-k)$.
Le nombre de préfixes est $\binom nk$, celui de suffixes est $\binom n{n-k}$.


```math
\binom{2n}n=\sum_{k=0}^n\binom nk\binom n{n-k}=\sum_{k=0}^n\binom nk^2.
```



## Exercice 22

### 0



```math
\frac1{2n+1}\binom{2n+1}n=\frac{(2n)!}{n!(n+1)!}=\frac1{n+1}\binom{2n}n.
```



### 1(a)

À un chemin de $(1,0)$ touchant la diagonale, associons le chemin obtenu en échangeant $E,N$ jusqu'au premier contact avec la diagonale. Son départ devient $(0,1)$ et son extrémité reste $(a,b)$.
Tout chemin de $(0,1)$ à $(a,b)$, avec $a>b$, touche la diagonale ; la même opération est inverse.


```math
\boxed{\#\text{chemins touchant la diagonale}=\binom{a+b-1}a.}
```



### 1(b)



```math
\binom{a+b-1}b-\binom{a+b-1}a=\frac a{a+b}\binom{a+b}a-\frac b{a+b}\binom{a+b}a
```




```math
=\boxed{\frac{a-b}{a+b}\binom{a+b}a.}
```



### 1(c)

Translater un chemin de Catalan de $(1,0)$ donne un chemin de $(1,0)$ à $(n+1,n)$ ne touchant pas la diagonale, et réciproquement.


```math
\boxed{C_n=\frac1{2n+1}\binom{2n+1}{n+1}=\frac1{n+1}\binom{2n}n.}
```



### 2(a)

Les indices cycliques sont modulo $2n+1$, et non $2n$.
Si un mot a une période propre $d\mid2n+1$, il est composé de $r=(2n+1)/d$ répétitions. Alors $r$ divise à la fois $n$ et $n+1$, donc $r=1$.


```math
\boxed{\text{Chaque classe a }2n+1\text{ éléments}.}
```



### 2(b)

La condition imprimée « plus de $E$ que de $N$ », jusqu'au préfixe entier, est impossible puisqu'il y a $n+1$ lettres $N$. Condition corrigée : chaque préfixe non vide contient strictement plus de $N$ que de $E$.

Associons $+1$ à $N$, $-1$ à $E$, et notons $S_0=0,S_1,\ldots,S_{2n+1}=1$ les sommes partielles. Soit $m$ le dernier indice de minimum parmi $S_0,\ldots,S_{2n}$.
La rotation commençant après $m$ a des sommes partielles strictement positives : avant le retour au début,


```math
S_j-S_m>0\quad(j>m),
```


et après ce retour,


```math
1-S_m+S_j\ge1\quad(j\le m).
```


Réciproquement, une rotation dont toutes les sommes partielles sont positives impose $S_j>S_m$ pour $j>m$ et $S_j\ge S_m$ pour $j<m$ ; elle commence donc après le dernier minimum. Unicité.

### 2(c)

Le mot positif commence par $N$. En retirant ce $N$, on obtient un chemin équilibré restant dans $y\ge x$ ; l'échange $E\leftrightarrow N$ donne un chemin de Catalan. Cette construction est bijective.


```math
\boxed{C_n=\frac{|\mathcal A|}{2n+1}=\frac1{2n+1}\binom{2n+1}n.}
```



## Exercice 23

### 1(a)



```math
f(x)=(1-4x)^{-1/2},\quad f^{(k)}(0)=4^k\frac12\frac32\cdots\frac{2k-1}2=\frac{(2k)!}{k!}.
```




```math
\boxed{f(x)=\sum_{k=0}^n\binom{2k}kx^k+o(x^n).}
```



### 1(b)



```math
f(x)^2=(1-4x)^{-1}=\sum_{k=0}^n4^kx^k+o(x^n).
```


Identification du coefficient d'ordre $n$ :


```math
\boxed{4^n=\sum_{i+j=n}\binom{2i}i\binom{2j}j.}
```



### 2(a)

Pour $n=0$, le chemin vide est unique. Pour $n\ge1$, les chemins ne revenant pas à la diagonale restent strictement d'un même côté. Comptons ceux avec $x>y$ et extrémité $(n+k,n-k)$, $1\le k\le n$.
Le premier pas est $E$ ; la réflexion au premier retour donne


```math
\binom{2n-1}{n+k-1}-\binom{2n-1}{n+k}
```


chemins admissibles. En sommant sur $k$,


```math
\sum_{k=1}^n\left(\binom{2n-1}{n+k-1}-\binom{2n-1}{n+k}\right)=\binom{2n-1}n.
```


La réflexion échange les deux côtés de la diagonale.


```math
\boxed{2\binom{2n-1}n=\binom{2n}n.}
```



### 2(b)

Un chemin arbitraire de longueur $2n$ a un dernier contact avec la diagonale au temps $2i$, pour un unique $0\le i\le n$.
Son préfixe se termine en $(i,i)$ : $\binom{2i}i$ choix. Son suffixe de longueur $2(n-i)$ ne revient plus à la diagonale : $\binom{2(n-i)}{n-i}$ choix.


```math
2^{2n}=\sum_{i=0}^n\binom{2i}i\binom{2(n-i)}{n-i}.
```



## Exercice 24

Deux points sur chaque droite déterminent exactement une intersection intérieure : celle des diagonales du quadrilatère. Réciproquement, chaque intersection intérieure détermine ces deux paires ; l'absence de concours triple assure l'injectivité.


```math
\boxed{\binom p2\binom q2.}
```



## Exercice 25



```math
\sigma^2=\operatorname{id}\Rightarrow\text{longueurs des cycles }1\text{ ou }2.
```




```math
|E|=\#\operatorname{Fix}(\sigma)+2r\text{ impair}\Rightarrow\#\operatorname{Fix}(\sigma)\text{ impair}\Rightarrow\#\operatorname{Fix}(\sigma)\ge1.
```



## Exercice 26



```math
E_0=\{\lfloor n/2\rfloor+1,\ldots,n\},\qquad|E_0|=\lceil n/2\rceil.
```


La somme de deux éléments de $E_0$ dépasse $n$, donc $E_0$ est sans somme.
Pour une partie sans somme non vide $E$, posons $m=\max E$. Dans chaque paire $\{x,m-x\}$, $1\le x<m/2$, au plus un élément appartient à $E$ ; si $m$ est pair, $m/2\notin E$.


```math
|E|\le1+\left\lfloor\frac{m-1}2\right\rfloor=\left\lceil\frac m2\right\rceil\le\left\lceil\frac n2\right\rceil.
```




```math
\boxed{\max|E|=\lceil n/2\rceil.}
```



## Exercice 27



```math
\Phi:S\to\{0,1\}^m,\quad x\mapsto(\mathbf1_{A_1}(x),\ldots,\mathbf1_{A_m}(x)).
```


L'hypothèse signifie que $\Phi$ est injective.


```math
n\le2^m\Rightarrow\boxed{m\ge\log_2n.}
```



## Exercice 28

### 1

Après $k$ vecteurs libres, leur espace engendré a $q^k$ éléments ; le vecteur suivant a $q^n-q^k$ choix.


```math
\boxed{N_{n,\ell}=\prod_{k=0}^{\ell-1}(q^n-q^k)=q^{\ell(\ell-1)/2}\prod_{k=0}^{\ell-1}(q^{n-k}-1).}
```


Le facteur $q^{\ell(\ell-1)/2}$ manque dans l'énoncé. Pour $q=2,n=\ell=2$, on obtient $6$, et non $3$.

### 2

Les colonnes d'une matrice inversible constituent une base ordonnée.


```math
\boxed{|GL_n(\mathbb K)|=\prod_{k=0}^{n-1}(q^n-q^k).}
```



### 3



```math
\det:GL_n(\mathbb K)\to\mathbb K^*
```


est surjective, car $\det\operatorname{diag}(a,1,\ldots,1)=a$, et son noyau est $SL_n(\mathbb K)$.


```math
\boxed{|SL_n(\mathbb K)|=\frac1{q-1}\prod_{k=0}^{n-1}(q^n-q^k).}
```


