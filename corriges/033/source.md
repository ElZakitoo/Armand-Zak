# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td33-probabilites-I.pdf)

## Autocorrection A



```math
A=(A\setminus B)\sqcup(A\cap B),\qquad \mathbb P(A\setminus B)=\mathbb P(A)-\mathbb P(A\cap B).
```



## Autocorrection B



```math
\mathbb P(A\cap B)=\frac7{10}+\frac12-\frac9{10}=\frac3{10},
```




```math
\mathbb P(A\triangle B)=\mathbb P(A)+\mathbb P(B)-2\mathbb P(A\cap B)=\frac35.
```



## Autocorrection C



```math
\mathbb P(\{k\})=ck,\qquad 1=c\sum_{k=1}^n k=c\frac{n(n+1)}2,\qquad \mathbb P(\{k\})=\frac{2k}{n(n+1)}.
```



## 1

Les complémentaires des quatre unions sont les quatre régions disjointes $A\cap B$, $A\cap\bar B$, $\bar A\cap B$, $\bar A\cap\bar B$. Leur somme de probabilités vaut $1$; celle des unions vaut $4-1=3$.

## 2



```math
p_1=1-y,\qquad p_2=x+y-1,\qquad p_3=1-x.
```


Ces nombres sont de somme $1$ et sont positifs ou nuls exactement lorsque


```math
0\leq x,y\leq1,\qquad x+y\geq1.
```



## 3

En posant $r=\mathbb P(A\cap B)$, les quatre régions ont pour probabilités


```math
r,\quad p-r,\quad q-r,\quad 1-p-q+r.
```


Leur positivité équivaut à


```math
\max(0,p+q-1)\leq r\leq\min(p,q).
```


Réciproquement, ces quatre masses définissent un exemple sur un univers à quatre éléments pour chaque $r$ de cet intervalle.

## 4

Pour deux événements $E,F$, poser $p=\mathbb P(E)$, $q=\mathbb P(F)$ et $c=\mathbb P(E\cap F)$. Alors


```math
\mathbb P(E)\mathbb P(F)-\mathbb P(E\cup F)\mathbb P(E\cap F)=(p-c)(q-c)\geq0.
```


Remplacer deux événements voisins par leur union et leur intersection ne fait donc pas augmenter le produit des probabilités. Pour chaque $\omega$, cette opération trie les deux indicatrices en ordre décroissant, sans changer leur somme.

Appliquer aux $n$ événements un tri par comparaisons voisines, avec le même ordre de comparaisons pour tout $\omega$. À la fin, la $k$-ième indicatrice vaut $1$ exactement lorsque la somme initiale est au moins $k$ : le $k$-ième événement est $C_k$. Ainsi


```math
\prod_{k=1}^n\mathbb P(C_k)\leq\prod_{k=1}^n\mathbb P(A_k).
```



## 5



```math
\mathbf1_{\cup_i A_i}\leq\sum_i\mathbf1_{A_i}\quad\Longrightarrow\quad\mathbb P\!\left(\bigcup_iA_i\right)\leq\sum_i\mathbb P(A_i).
```



## 6

1. Si $m=\sum_i\mathbf1_{A_i}(\omega)$,


```math
\sum_i\mathbf1_{A_i}(\omega)-\sum_{i<j}\mathbf1_{A_i\cap A_j}(\omega)=m-\binom m2\leq\mathbf1_{m\geq1}.
```


Pour $m=0$, les deux côtés sont nuls; pour $m\geq1$, la différence avec $1$ vaut $-(m-1)(m-2)/2\leq0$. L'espérance donne l'inégalité de Bonferroni.

2. Pour $j$ fixé,


```math
\mathbf1_{\cup_i A_i}\leq\sum_i\mathbf1_{A_i}-\sum_{i\ne j}\mathbf1_{A_i\cap A_j}.
```


Si $\omega\in A_j$, le membre droit vaut $1$; sinon, il vaut le nombre d'événements réalisés. Prendre l'espérance.

## 7



```math
\{N=k\}=A_{n-k+1}\setminus A_{n-k}\quad(1\leq k\leq n),
```




```math
\mathbb P(N=k)=\frac1n,\qquad \mathbb P(N=0)=1-\mathbb P(A_n)=0.
```


Donc $N\sim\mathcal U(\{1,\ldots,n\})$.

## 8

Sur $\Omega'=\Omega\times\{-1,1\}$, prendre la probabilité produit, $Y(\omega,e)=|X(\omega)|$ et $\varepsilon(\omega,e)=e$, le second facteur étant uniforme. Alors $Y$ et $\varepsilon$ sont indépendantes, et pour $x>0$,


```math
\mathbb P'(\varepsilon Y=x)=\tfrac12\mathbb P(|X|=x)=\mathbb P(X=x).
```


Même égalité pour $x<0$ et pour $x=0$.

L'univers initial ne suffit pas toujours. Prendre $\Omega=\{-1,0,1\}$ et $X(\omega)=\omega$, de masses $1/4,1/2,1/4$. Une factorisation indépendante imposerait $Y\in\{0,1\}$ presque sûrement, $\mathbb P(Y=0)=\mathbb P(Y=1)=1/2$ et $\mathbb P(\varepsilon=\pm1)=1/2$. Les quatre couples $(Y,\varepsilon)$ auraient une probabilité $1/4$, impossible sur trois atomes.

## 9

1. 

```math
\mathbb P_C(A\cap B)>\mathbb P_C(A)\mathbb P_C(B)\iff\mathbb P(A\cap B\cap C)\mathbb P(C)>\mathbb P(A\cap C)\mathbb P(B\cap C).
```



2. Prendre $\mathbb P(C)=\mathbb P(\bar C)=1/2$ et les tables conditionnelles suivantes, dans l'ordre $(A\cap B,A\cap\bar B,\bar A\cap B,\bar A\cap\bar B)$ :


```math
\mathbb P_C:\ (0.80,0.10,0.10,0),\qquad\mathbb P_{\bar C}:\ (0,0.10,0.10,0.80).
```


Dans $C$, $0.80<0.90^2$; dans $\bar C$, $0<0.10^2$. Globalement, $\mathbb P(A)=\mathbb P(B)=1/2$ et $\mathbb P(A\cap B)=0.40>1/4$.

## 10



```math
\mathbb P(A\cap B\mid A\cup B)=\frac{\mathbb P(A\cap B)}{\mathbb P(A\cup B)}\leq\frac{\mathbb P(A\cap B)}{\mathbb P(A)}=\mathbb P(A\cap B\mid A).
```



## 11

Coder pile par $1$, face par $0$. Chaque $A_k$, y compris $A_0$, a probabilité $1/2$. Les $n$ bits déterminent entièrement leur parité : la famille complète n'est pas indépendante. Plus précisément, l'intersection de tous les $A_k$ a probabilité $2^{-n}$ si $n$ est pair, et $0$ si $n$ est impair, au lieu de $2^{-(n+1)}$.

Une sous-famille sans $A_0$ est indépendante par construction. Une sous-famille avec $A_0$ laisse au moins un bit non imposé. Pour chaque choix des bits imposés et de la parité, exactement la moitié des choix des bits restants convient. Chaque configuration d'une sous-famille de $r$ événements a donc probabilité $2^{-r}$.

## 12

Poser $p=\mathbb P(A)$, $q=\mathbb P(B)$ et $r=\mathbb P(A\cap B)$. L'égalité des produits s'écrit


```math
r(1-p-q+r)=(p-r)(q-r)\iff r=pq,
```


soit l'indépendance.

## 13

1. 

```math
A\subseteq B\Longrightarrow\mathbb P(A)=\mathbb P(A\cap B)=\mathbb P(A)\mathbb P(B)\Longrightarrow\mathbb P(A)(1-\mathbb P(B))=0.
```


2. 

```math
A\perp A\iff\mathbb P(A)=\mathbb P(A)^2\iff\mathbb P(A)\in\{0,1\}.
```



## 14

Sous indépendance, $A=uv^{\mathsf T}$ avec $u_i=\mathbb P(X=i)$, $v_j=\mathbb P(Y=j)$ : son rang est $1$.

Réciproquement, si $\operatorname{rg}A=1$, toutes ses colonnes sont proportionnelles. Diviser la colonne $j$ par sa somme strictement positive $v_j$ donne une même colonne $u$. Puis $\sum_jv_j=1$ et $\sum_ju_iv_j=u_i=\mathbb P(X=i)$. Ainsi $A_{ij}=u_iv_j$.

## 15

Avec $a=|A|$, $b=|B|$, $c=|A\cap B|$, l'indépendance équivaut à $nc=ab$.
Si $n$ est premier, elle impose $n\mid a$ ou $n\mid b$, impossible pour deux événements non triviaux. Pour $n=1$, aucun événement n'est non trivial.

Si $n=rs$ avec $r,s\geq2$, identifier l'univers à $\{1,\ldots,r\}\times\{1,\ldots,s\}$ et prendre $A=\{1\}\times\{1,\ldots,s\}$, $B=\{1,\ldots,r\}\times\{1\}$. Ils sont indépendants, de probabilités $1/r$ et $1/s$. Condition : $n$ composé.

## 16



```math
1-\mathbb P\!\left(\bigcup_{i=1}^nA_i\right)=\mathbb P\!\left(\bigcap_{i=1}^n\bar A_i\right)=(1-p)^n>0.
```


La réunion ne peut pas être $\Omega$.

## 17

Pour chaque $\varepsilon\in\{0,1\}^n$, l'atome formé en choisissant $A_i$ si $\varepsilon_i=1$, $\bar A_i$ sinon, a probabilité


```math
\prod_i p_i^{\varepsilon_i}(1-p_i)^{1-\varepsilon_i}>0.
```


Les $2^n$ atomes sont disjoints et non vides; $|\Omega|\geq2^n$.

## 18

Écrire les probabilités de $r$ événements indépendants non triviaux sous forme irréductible $a_i/b_i$, avec $0<a_i<b_i$. Poser $B=\prod_i b_i$. Le cardinal de chaque atome est


```math
\frac nB\prod_i c_i\in\mathbb N,\qquad c_i\in\{a_i,b_i-a_i\}.
```


Comme $\gcd(a_i,b_i-a_i)=1$, Bézout puis multiplication donnent une combinaison entière égale à $1$ des $2^r$ produits $\prod_i c_i$. Ainsi $B\mid n$. Chaque $b_i\geq2$ apporte au moins un facteur premier, donc $r\leq\Omega(n)$.

Réciproquement, si $n=p_1\cdots p_s$ avec $s=\Omega(n)$, identifier l'univers à $\prod_{i=1}^s\{1,\ldots,p_i\}$. Les événements « la coordonnée $i$ vaut $1$ » sont indépendants et non triviaux. Maximum : $\Omega(n)$; pour $n=1$, il vaut $0$.

## Autocorrection D



```math
\text{(i)}\quad1-\left(\frac56\right)^3=\frac{91}{216},\qquad\text{(ii)}\quad3\frac16\left(\frac56\right)^2=\frac{25}{72}.
```




```math
\text{(iii)}\quad1-\frac{6\cdot5\cdot4}{6^3}=\frac49.
```


Pour (iv), un triple convient si sa valeur est paire : $3$ cas. Pour exactement une paire, la valeur isolée doit être paire : $6\cdot3-3=15$ choix des deux valeurs et $3$ positions de la valeur isolée. Donc


```math
\text{(iv)}\quad\frac{3+3\cdot15}{216}=\frac29.
```



## 19



```math
\text{(i)}\quad\frac{\binom{13}2^2}{\binom{52}4}.
```


Pour (ii), chaque main non ordonnée correspond à $4!$ tirages ordonnés, d'où la même probabilité. Avec remise, choisir les deux positions des trèfles :


```math
\text{(iii)}\quad\binom42\left(\frac14\right)^4=\frac3{128}.
```



## 20

Tous les appariements des $2n$ boules sont équiprobables; leur nombre est $(2n-1)!!=(2n)!/(2^nn!)$.

1. Un appariement bicolore correspond à une bijection des $n$ boules blanches vers les $n$ rouges :


```math
\mathbb P(\text{tous bicolores})=\frac{n!}{(2n-1)!!}=\frac{2^n(n!)^2}{(2n)!}.
```


2. Si $n$ est impair, probabilité nulle. Si $n$ est pair, apparier séparément chaque couleur :


```math
\mathbb P(\text{tous unicolores})=\frac{((n-1)!!)^2}{(2n-1)!!}.
```



## 21

Pour $r\geq1$, les positions des rouges forment une partie uniforme de taille $r$ de $\{1,\ldots,b+r\}$. Ainsi


```math
\mathbb P(N=k)=\frac{\binom{b+r-k}{r-1}}{\binom{b+r}r}\quad(1\leq k\leq b+1).
```


Pour $r=0$, aucune première rouge n'existe.

## 22

1. Échanger pile et face échange les deux majorités; aucune égalité n'est possible en $2n+1$ lancers. Probabilité : $1/2$.
2. Pour $n+1\leq k\leq2n+1$, il faut $n$ piles parmi les $k-1$ premiers lancers, puis pile :


```math
\mathbb P(\text{$(n+1)$-ième pile au rang $k$})=2^{-k}\binom{k-1}n.
```


Pour $k\leq n$, cette probabilité est nulle.
3. Ces événements disjoints partitionnent la majorité pile, donc


```math
\sum_{k=n+1}^{2n+1}2^{-k}\binom{k-1}n=\frac12.
```



## 23

L'absence de deux cartes consécutives de même couleur impose l'une des deux alternances. Chaque mot de $26$ rouges et $26$ noires est équiprobable :


```math
\mathbb P(\text{deux voisines de même couleur})=1-\frac2{\binom{52}{26}}.
```


Les quatre positions des rois sont uniformes parmi les $\binom{52}4$ parties. Les parties sans positions consécutives sont au nombre de $\binom{49}4$ (envoyer $i_1<i_2<i_3<i_4$ sur $i_1,i_2-1,i_3-2,i_4-3$). Donc


```math
\mathbb P(\text{deux rois voisins})=1-\frac{\binom{49}4}{\binom{52}4}.
```



## 24

Sous l'hypothèse de dates indépendantes et uniformes sur $365$ jours,


```math
\mathbb P(\text{au moins une date commune})=1-\prod_{k=0}^{29}\left(1-\frac{k}{365}\right)\simeq0.7063.
```



## 25



```math
\mathbb P(Z_1=Z_2)=4^{-n}\sum_{k=0}^n\binom nk^2=4^{-n}\binom{2n}n.
```


La dernière identité compte les parties de taille $n$ de deux ensembles disjoints de taille $n$.

## 26



```math
X_1^2=X_1\sim\mathcal B(p_1),\qquad1-X_1\sim\mathcal B(1-p_1).
```




```math
X_1X_2=1\iff X_1=X_2=1\quad\Longrightarrow\quad X_1X_2\sim\mathcal B(p_1p_2).
```



## 27

1. Le produit est impair exactement lorsque chaque facteur est impair : probabilité du produit pair $1-2^{-n}$.
2. Pour $n\geq1$, conditionner par les $n-1$ premiers résultats laisse une dernière parité uniforme. Probabilité de la somme paire : $1/2$.

## 28

1. 

```math
\mathbb P(\text{paire})=\frac6{36}=\frac16.
```


2. Pour deux lancers indépendants de même loi $(p_1,\ldots,p_6)$,


```math
\mathbb P(\text{paire})=\sum_{i=1}^6p_i^2\geq\frac{(\sum_i p_i)^2}6=\frac16,
```


avec égalité exactement pour le dé équilibré.

## 29



```math
\mathbb P(N=k)=\left(\prod_{i=1}^{k-1}\frac1i\right)\left(1-\frac1k\right)=\frac{k-1}{k!}\quad(2\leq k\leq n),
```




```math
\mathbb P(N=1)=0,\qquad\mathbb P(N=0)=\prod_{i=1}^n\frac1i=\frac1{n!}.
```


La somme vaut $1$ car $(k-1)/k!=1/(k-1)!-1/k!$.

## 30

Pour $0<p<1$ et $0\leq k<n$,


```math
\frac{\mathbb P(X=k+1)}{\mathbb P(X=k)}=\frac{n-k}{k+1}\frac p{1-p}\geq1\iff k+1\leq(n+1)p.
```


Si $(n+1)p$ n'est pas entier, le seul mode est $\lfloor(n+1)p\rfloor$. Si $(n+1)p=m$ est entier, les deux modes sont $m-1,m$. Pour $p=0$, le mode est $0$; pour $p=1$, il est $n$; pour $n=0$, il est $0$.

## 31



```math
\begin{array}{c|cc}
&Y=0&Y=1\\\hline
X=0&1-p-q+r&q-r\\
X=1&p-r&r
\end{array}
```


Toutes les lois possibles sont données par $\max(0,p+q-1)\leq r\leq\min(p,q)$.

## 32

Construire une suite de Bernoulli indépendantes $(B_i)$ de paramètre $p$ et poser $S_n=\sum_{i=1}^nB_i$. Alors $S_n\sim\mathcal B(n,p)$ et $S_n\leq S_{n+1}$, d'où


```math
\mathbb P(X_n\geq k)=\mathbb P(S_n\geq k)\leq\mathbb P(S_{n+1}\geq k).
```



## 33

1. 

```math
\mathbb P(\text{au moins un 6})=1-(9/10)^n\longrightarrow1.
```


2. Considérer les blocs disjoints de deux lancers. Chacun vaut $66$ avec probabilité $1/100$, indépendamment des autres :


```math
\mathbb P(\text{aucun $66$})\leq(99/100)^{\lfloor n/2\rfloor}\longrightarrow0.
```


3. Pour un mot fixé de longueur $\ell$ sur un alphabet de $q$ symboles uniformes, la même méthode donne une probabilité d'absence au plus $(1-q^{-\ell})^{\lfloor n/\ell\rfloor}\to0$. Tout texte fixé apparaît donc avec une probabilité tendant vers $1$ lorsque la frappe aléatoire s'allonge.

## 34

1. 

```math
|A_d|=n/d,\qquad\mathbb P(A_d)=1/d.
```


2. Pour toute partie $I$ des facteurs premiers distincts,


```math
\bigcap_{i\in I}A_{p_i}=A_{\prod_{i\in I}p_i},\qquad\mathbb P\!\left(\bigcap_{i\in I}A_{p_i}\right)=\prod_{i\in I}\frac1{p_i}.
```


3. 

```math
\mathbb P(\gcd(X,n)=1)=\prod_{p\mid n}\left(1-\frac1p\right),\qquad\varphi(n)=n\prod_{p\mid n}\left(1-\frac1p\right).
```


4. 

```math
\varphi(p)=p-1,\qquad\varphi(p^a)=p^a-p^{a-1}.
```


Dans le second cas, on retire exactement les multiples de $p$.

## 35

Conditionnellement à $(a,b,c)$ avec $a\ne0$, l'équation $ad=bc$ impose au plus une valeur de $d$. Donc


```math
1-p(n)\leq\mathbb P(a=0)+\mathbb P(ad=bc,\ a\ne0)\leq\frac2{2n+1}\longrightarrow0.
```



## 36

Pour chaque élément, les quatre appartenances à $(A,B)$ sont équiprobables, indépendamment des autres éléments.


```math
\text{(i)}\quad(3/4)^n,\qquad\text{(ii)}\quad(3/4)^n,\qquad\text{(iii)}\quad n\frac14\left(\frac34\right)^{n-1}.
```



## 37

Chaque élément appartient à l'intersection avec probabilité $2^{-r}$; ces événements sont indépendants d'un élément à l'autre. Ainsi


```math
|X_1\cap\cdots\cap X_r|\sim\mathcal B(n,2^{-r}).
```



## 38

1. Les orbites de $\langle\sigma\rangle$ sont les cycles de $\sigma$; la transitivité équivaut à ce que $\sigma$ soit un $n$-cycle.
2. 

```math
p_n=\frac{(n-1)!}{n!}=\frac1n.
```


3. Un groupe non transitif possède une orbite $S$ de cardinal entre $1$ et $\lfloor n/2\rfloor$. Les deux permutations préservent alors $S$. Pour $|S|=k$ fixé,


```math
\mathbb P(X_n(S)=S)=\frac{k!(n-k)!}{n!}=\binom nk^{-1}.
```


Par indépendance et réunion,


```math
1-q_n\leq\sum_{k=1}^{\lfloor n/2\rfloor}\binom nk^{-1}\leq\frac1n+\frac{\lfloor n/2\rfloor-1}{\binom n2}\longrightarrow0.
```


La seconde borne vaut pour $n\geq4$.

## Autocorrection E



```math
s_A=(1-p)^4+4p(1-p)^3,\qquad s_B=(1-p)^2,
```




```math
s_A-s_B=p(1-p)^2(2-3p).
```


Choisir $A$ pour $0<p<2/3$, $B$ pour $2/3<p<1$; égalité pour $p\in\{0,2/3,1\}$.

## Autocorrection F

Pour $-5\leq k\leq5$, il y a $6-|k|$ couples de différence $k$ :


```math
\mathbb P(X=k)=\frac{6-|k|}{36}.
```




```math
\mathbb P(|X|=0)=\frac16,\qquad\mathbb P(|X|=k)=\frac{6-k}{18}\quad(1\leq k\leq5).
```




```math
\mathbb P(X^2=0)=\frac16,\qquad\mathbb P(X^2=k^2)=\frac{6-k}{18}\quad(1\leq k\leq5).
```



## 39

Écrire le score d'Alice $U+B$, celui de Bob $V$, avec $U,V\sim\mathcal B(10,1/2)$ indépendantes et $B\sim\mathcal B(1/2)$ indépendant. Alors


```math
\mathbb P(U+B>V)=\tfrac12\mathbb P(U>V)+\tfrac12\mathbb P(U\geq V)=\frac12,
```


car $U,V$ ont même loi et sont indépendantes. Le jeu est équitable.

## 40

1. Si une face impaire a probabilité $c$, une face paire a probabilité $2c$; $9c=1$. Donc


```math
\mathbb P(X=k)=\begin{cases}1/9&k\text{ impair},\\2/9&k\text{ pair}.\end{cases}
```


2. 

```math
\mathbb P(X\text{ pair})=\frac23,\qquad\mathbb P(X\geq3)=\frac69=\frac23.
```



## 41

Pour $r\geq1$, conditionner par le numéro $K$ de l'urne, uniforme sur $\{0,\ldots,r\}$. Avec la convention $0^0=1$,


```math
\mathbb P(R_{n+1}\mid R_1\cap\cdots\cap R_n)=\frac{\sum_{k=0}^r(k/r)^{n+1}}{\sum_{k=0}^r(k/r)^n}.
```


Diviser les deux sommes par $r$. Par sommes de Riemann, pour $n$ fixé,


```math
\lim_{r\to\infty}\mathbb P(R_{n+1}\mid R_1\cap\cdots\cap R_n)=\frac{\int_0^1x^{n+1}\,dx}{\int_0^1x^n\,dx}=\frac{n+1}{n+2}.
```


Pour $r=0$, les urnes sont vides : le tirage n'est pas défini.

## 42

Si la poche gauche est découverte vide et qu'il reste $k$ allumettes à droite, les $2n-k$ tirages réussis contenaient $n$ choix gauches et $n-k$ choix droits; le choix suivant est gauche. Tous ces mots sont admissibles. En échangeant les poches,


```math
\mathbb P(X=k)=2\binom{2n-k}n2^{-(2n-k+1)}=\binom{2n-k}n2^{-(2n-k)}\quad(0\leq k\leq n).
```



## 43

Pour $n\geq2$, tant que ni la place $1$ ni la place $n$ n'a été choisie par un passager déplacé, ces deux places restent libres et jouent des rôles symétriques. Le premier choix de l'une d'elles est donc chacune avec probabilité $1/2$.

Si la place $1$ est choisie d'abord, la chaîne des déplacements s'arrête et le dernier trouve sa place. Si la place $n$ est choisie d'abord, il la perd. Probabilité : $1/2$. Pour $n=1$, elle vaut $1$.

## Autocorrection G



```math
\mathbb P(\text{as de trèfle})=\frac1{4\cdot32}+\frac3{4\cdot52}=\frac{37}{1664}.
```




```math
\mathbb P(\text{jeu de 32}\mid\text{as de trèfle})=\frac{1/(4\cdot32)}{37/1664}=\frac{13}{37}.
```



## 44



```math
p_0=1,\qquad p_{n+1}=pp_n+(1-p)(1-p_n),
```




```math
p_{n+1}-\tfrac12=(2p-1)(p_n-\tfrac12),\qquad p_n=\frac{1+(2p-1)^n}{2}.
```


Pour $0<p<1$, $p_n\to1/2$. Pour $p=1$, $p_n=1$. Pour $p=0$, $p_n$ alterne entre $1$ et $0$ et ne converge pas.

## 45

Noter $E$ l'événement « les $N-1$ premiers coffres sont vides ». Alors


```math
\mathbb P(E)=1-p+\frac pN,\qquad\mathbb P(\text{dernier coffre}\mid E)=\frac{p/N}{1-p+p/N}=\frac p{N-(N-1)p}.
```



## 46

1. Prendre les $12$ couples ordonnés de cartes distinctes, équiprobables. Noter $D$ : « au moins une dame », $C$ : « la dame de cœur », $Q$ : « les deux dames ».


```math
\mathbb P(Q\mid D)=\frac{2/12}{10/12}=\frac15,\qquad\mathbb P(Q\mid C)=\frac{2/12}{6/12}=\frac13.
```


2. Modèle : sexes indépendants et équiprobables; l'enfant accompagnant est choisi uniformément parmi les deux, indépendamment des sexes. Sur $\{F,G\}^2\times\{1,2\}$ uniforme, parmi les quatre issues où l'enfant choisi est un garçon, deux ont une fille comme autre enfant. Probabilité : $1/2$.

Si l'information est seulement « au moins un garçon », les trois couples $GG,GF,FG$ restent équiprobables et la probabilité devient $2/3$. La règle de rencontre détermine le conditionnement.

## 47

Poser $M=\lfloor\sqrt n\rfloor$. Pour chaque $m<M$, les entiers dont la racine a partie entière $m$ et premier chiffre décimal $1$ appartiennent à


```math
[(m+1/10)^2,(m+2/10)^2[.
```


Le nombre d'entiers de cet intervalle vaut sa longueur à $O(1)$ près :


```math
\frac m5+\frac3{100}+O(1)=\frac m5+O(1).
```


Le dernier intervalle, éventuellement tronqué par $n$, contient $O(M+1)$ entiers. Par conséquent,


```math
np_n=\sum_{m=0}^{M-1}\left(\frac m5+O(1)\right)+O(M+1)=\frac{M^2}{10}+O(M+1)=\frac n{10}+O(\sqrt n),
```




```math
p_n\longrightarrow\frac1{10}.
```



## 48

Récurrence sur le nombre de variables, pour tout polynôme non nul. En une variable, il y a au plus $d$ racines. Écrire ensuite


```math
Q(X_1,\ldots,X_n)=\sum_{j=0}^rQ_j(X_1,\ldots,X_{n-1})X_n^j,\qquad Q_r\ne0,
```


avec $\deg Q_r\leq d-r$. Par récurrence,


```math
\mathbb P(Q_r(U_1,\ldots,U_{n-1})=0)\leq\frac{d-r}{|S|}.
```


Hors de cet événement, conditionner par les $n-1$ premières variables donne un polynôme de degré $r$ en la dernière, donc une probabilité de zéro au plus $r/|S|$. Ainsi


```math
\mathbb P(Q(U_1,\ldots,U_n)=0)\leq\frac{d-r}{|S|}+\frac r{|S|}=\frac d{|S|}.
```



## 49

1. Pour $p=3k+2$, les sommes de deux éléments de $B_0$ sont représentées dans $[2k+2,4k+2]$. Modulo $p$, elles appartiennent à


```math
\{2k+2,\ldots,3k+1\}\cup\{0,\ldots,k\},
```


disjoint de $B_0$. Multiplier par $x\ne0$ et passer à une partie conserve l'absence de sommes.
2. Choisir un tel premier $p>2\max_{a\in A}|a|$. Les classes des éléments de $A$ sont distinctes et non nulles. Pour $x$ uniforme non nul, poser


```math
B_x=\{a\in A:\bar a\in xB_0\}.
```


Chaque $B_x$ est sans somme dans $\mathbb Z$. Pour $a$ fixé, $x^{-1}\bar a$ est uniforme parmi les classes non nulles :


```math
\mathbb E|B_x|=|A|\frac{k+1}{3k+1}>\frac{|A|}{3}.
```


Au moins une réalisation dépasse donc $|A|/3$.
3. Si $p_1,\ldots,p_r$ étaient tous les premiers congrus à $2$ modulo $3$, le nombre $N=3p_1\cdots p_r-1$ serait $2$ modulo $3$, sans être divisible par aucun $p_i$. Au moins un de ses facteurs premiers serait pourtant $2$ modulo $3$, contradiction.

## 50

1. a) Pour une équipe fixée, la probabilité de tout gagner vaut $2^{-(n-1)}$. Deux équipes ne peuvent pas tout gagner simultanément, donc la probabilité qu'il en existe une vaut $n2^{-(n-1)}$.

b) Chaque classement total définit un tournoi transitif distinct, et réciproquement. Parmi $2^{\binom n2}$ tournois,


```math
\mathbb P(\text{classement transitif})=\frac{n!}{2^{\binom n2}}.
```


c) Pour $k$ équipes fixées et une équipe extérieure fixée, la probabilité vaut $2^{-k}$. Pour les $n-k$ équipes extérieures, ces événements utilisent des matchs distincts et sont indépendants. Probabilité qu'au moins une les batte toutes :


```math
1-(1-2^{-k})^{n-k}.
```


2. Par réunion sur les parties de taille $k$,


```math
1-P(n,k)\leq\binom nk(1-2^{-k})^{n-k}\leq n^k e^{-(n-k)2^{-k}}\longrightarrow0
```


pour $k$ fixé.
3. Pour deux équipes distinctes $i,j$, l'absence de chemin $i\to j$ de longueur $1$ ou $2$ a probabilité


```math
\frac12\left(\frac34\right)^{n-2}.
```


Il faut perdre le match direct et, pour chaque troisième équipe, éviter l'une des quatre orientations possibles. Pour une paire non ordonnée, les deux directions possibles de ce type sont disjointes et chacune a probabilité $\frac12(\frac34)^{n-2}$ ; par réunion sur les paires,


```math
1-P(n)\leq\binom n2\left(\frac34\right)^{n-2}\longrightarrow0.
```


4. Choisir une équipe $i$ ayant un nombre maximal de victoires. Si $j$ n'est atteignable depuis $i$ en un ou deux matchs, $j$ bat $i$ et toutes les équipes battues par $i$. Elle a donc strictement plus de victoires que $i$, contradiction.

## 51

Noter $e(X)$ le nombre d'arêtes dont les deux extrémités sont dans $X$. Retirer au plus une extrémité par arête suffit à rendre l'ensemble indépendant. Le retrait minimal vérifie donc


```math
|U|\geq|X|-e(X),\qquad\mathbb E|U|\geq np-\frac{nd}2p^2.
```


Cette parabole est maximale en $p=1/d\in[0,1]$. Comme $\alpha(\Gamma)\geq|U|$ pour toute réalisation,


```math
\alpha(\Gamma)\geq\mathbb E|U|\geq\frac n{2d}.
```



## 52

1. Pour un sommet $v$, être dans $Y$ signifie que ni lui ni aucun de ses $d(v)$ voisins n'est choisi :


```math
\mathbb E|U|=np+\sum_{v\in\Gamma}(1-p)^{d(v)+1}.
```


2. Puisque $d(v)\geq\delta$ et $1-p\leq e^{-p}$,


```math
\mathbb E|U|\leq n\left(p+e^{-p(\delta+1)}\right).
```


3. La dérivée de $p+e^{-(\delta+1)p}$ s'annule en $p=\ln(\delta+1)/(\delta+1)\in[0,1]$, où la fonction est minimale. Il existe une réalisation de taille au plus l'espérance, donc


```math
\gamma(\Gamma)\leq n\frac{1+\ln(\delta+1)}{\delta+1}.
```


Pour $\delta=0$, ce choix donne $p=0$ et la borne $\gamma(\Gamma)\leq n$.
