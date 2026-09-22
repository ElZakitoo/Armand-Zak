# corrigé zakito

[Énoncé](https://christophebertault.fr/documents/coursetexercices/Exercices%20-%20Probabilites%20sur%20un%20univers%20fini.pdf)

## 1

1. $P(T^+)=0{,}01\times0{,}9+0{,}04\times0{,}9+0{,}95\times0{,}1=0{,}140$.
2. $P(M_1\mid T^+)=0{,}009/0{,}140=9/140\simeq6{,}43\%$.

## 2



```math
P(\text{blond}\cap\text{bleu})=\frac23\cdot\frac18=\frac1{12},\qquad P(\text{bleu})=\frac{1/12}{0{,}8}=\frac5{48}.
```


Donc $P(\text{non blond}\cap\text{bleu})=5/48-1/12=1/48$.

## 3

Soit $D$ l'événement « dé pipé » et $E$ l'observation de $n$ uns en $2n$ lancers. Les vraisemblances sont


```math
P(E\mid D)=\binom{2n}{n}(5/6)^n(1/6)^n=P(E\mid\bar D).
```


Bayes donne $P(D\mid E)=P(D)=1/4$ : cette observation ne renseigne pas sur le choix du dé.

## 4

1. Pour $Y=\lfloor\sqrt X\rfloor$, les intervalles $[1,3]$, $[4,8]$, $[9,15]$ et $[16,20]$ donnent respectivement $Y=1,2,3,4$. Ainsi


```math
P(Y=1)=\frac3{20},\quad P(Y=2)=\frac5{20},\quad P(Y=3)=\frac7{20},\quad P(Y=4)=\frac5{20}.
```


2. Chaque classe modulo $6$ contient $n$ valeurs possibles de $X$. Le cosinus vaut $1$ pour la classe $0$, $-1$ pour la classe $3$, $1/2$ pour les classes $1,5$ et $-1/2$ pour les classes $2,4$. Donc


```math
P(\cos(\pi X/3)=1)=P(\cos(\pi X/3)=-1)=\frac16,
```




```math
P(\cos(\pi X/3)=1/2)=P(\cos(\pi X/3)=-1/2)=\frac13.
```



## 5

Le quotient des probabilités successives est


```math
\frac{P(X=k+1)}{P(X=k)}=\frac{n-k}{k+1}\frac p{1-p}.
```


Il est supérieur ou égal à $1$ exactement lorsque $k+1\leq(n+1)p$. Le mode est $\lfloor(n+1)p\rfloor$; si $(n+1)p=m$ est entier, les deux modes sont $m-1,m$.

## 6

Le produit est impair exactement quand tous les $X_i$ sont impairs. Il y a $p$ impairs parmi $2p$ entiers, donc


```math
P(X_1\cdots X_n\text{ pair})=1-2^{-n}.
```



## 7

1. L'indépendance et la symétrie donnent $(X,Y)\overset d=(X,-Y)$. Les événements $\{X=Y\}$ et $\{X=-Y\}$ ont même probabilité; leur intersection vaut $\{X=Y=0\}$. Or $\{X^2=Y^2\}$ est leur réunion, donc


```math
P(X^2=Y^2)=2P(X=Y)-P(X=0)P(Y=0).
```


2. $X+Y$ et $-(X+Y)$ ont même loi. Ainsi $P(X+Y>0)=P(X+Y<0)$, d'où $P(X+Y\geq0)=P(X+Y\leq0)$.

## 8

1. Pour toute permutation $\sigma$, les variables permutées restent indépendantes de même loi; les probabilités des pavés $\prod_i\{X_i\in A_i\}$ sont inchangées, donc le vecteur a la même loi.
2. En permutant cycliquement les indices, $(X_1,\ldots,X_{n-1})\overset d=(X_2,\ldots,X_n)$; l'application mesurable qui associe le cardinal des valeurs distinctes conserve l'égalité en loi.

## 9

1. $P(M\geq k)=((n-k+1)/n)^n$. Donc, pour $1\leq k\leq n$,


```math
P(M=k)=\left(\frac{n-k+1}{n}\right)^n-\left(\frac{n-k}{n}\right)^n.
```


2. Par complémentaire et $1-u\leq e^{-u}$,


```math
P(\exists i:X_i=1)=1-(1-1/n)^n\geq1-e^{-1}.
```



## 10

Par passage à la limite à gauche dans l'hypothèse, puis soustraction,


```math
P(X=x,Y\leq y)=P(X\leq x,Y\leq y)-P(X<x,Y\leq y)=P(X=x)P(Y\leq y).
```


La même différence en $y$ donne $P(X=x,Y=y)=P(X=x)P(Y=y)$. En sommant sur les valeurs d'un ensemble, les événements de $X$ et $Y$ sont indépendants.

## 11

1. Si $X,Y$ sont uniformes sur $\{0,\ldots,n\}$, $P(X=Y)=1/(n+1)$. Si elles sont $\mathcal B(n,1/2)$,


```math
P(X=Y)=4^{-n}\sum_{k=0}^n\binom nk^2=4^{-n}\binom{2n}{n}.
```


2. Ces probabilités sont respectivement équivalentes à $1/n$ et $1/\sqrt{\pi n}$. La loi binomiale est concentrée autour de son mode, contrairement à la loi uniforme.
3. Posons $f(t)=\sum_k((1-t)/(n+1)+tp_k)^2$. Alors $f'(0)=0$ et $f''(t)=2\sum_k(p_k-1/(n+1))^2\geq0$. Le minimum sur $[0,1]$ est $f(0)=1/(n+1)$, tandis que $f(1)=P(X=Y)$. Égalité ssi $p_k=1/(n+1)$ pour tout $k$, c.-à-d. $X$ uniforme sur ses $n+1$ valeurs.

## 12

Pour $2\leq s\leq n+1$, $P(X+Y=s)=(s-1)/n^2$; pour $n+2\leq s\leq2n$, $P(X+Y=s)=(2n+1-s)/n^2$. De plus


```math
P(X+Y=Z)=\frac1n\sum_{s=2}^n\frac{s-1}{n^2}=\frac{n-1}{2n^2}.
```



## 13

Posons $q=2p-1$. Alors $\mathbb E(Y_k)=q^k$ et


```math
u_k=\frac{1+q^k}{2},\qquad v_k=\frac{1-q^k}{2};
```


comme $|q|<1$, ces deux suites tendent vers $1/2$. Si $p=1/2$, les $Y_k$ sont indépendantes (la transformation $(X_1,\ldots,X_n)\mapsto(Y_1,\ldots,Y_n)$ est bijective sur $\{-1,1\}^n$). Réciproquement, $Y_1,Y_2$ indépendantes équivaut à $p=P(Y_2=1)=p^2+(1-p)^2$, donc à $p=1/2$ ou $p=1$; ici $p\in(0,1)$, donc $p=1/2$.

## 14

Pour $n\geq2$, poser


```math
A(z)=\mathbb E(z^{X-1}),\qquad B(z)=\mathbb E(z^{Y-1}).
```


Si la somme était uniforme, l'indépendance donnerait


```math
A(z)B(z)=\frac{1+z+\cdots+z^{2n-2}}{2n-1}.
```


Prendre $\zeta=e^{2i\pi/(2n-1)}$ et $\alpha=(n-1)\pi/(2n-1)<\pi/2$. Le membre droit s'annule en $\zeta$. Pourtant, pour $0\leq j\leq n-1$,


```math
\operatorname{Re}(e^{-i\alpha}\zeta^j)=\cos\!\left(\frac{(2j-n+1)\pi}{2n-1}\right)>0.
```


Les coefficients de $A$ et $B$ étant positifs ou nuls et de somme $1$, les parties réelles de $e^{-i\alpha}A(\zeta)$ et $e^{-i\alpha}B(\zeta)$ sont strictement positives. Aucun des deux facteurs n'est nul : contradiction.

Pour $n=1$, $X+Y=2$ est uniforme sur le singleton $\{2\}$; il faut exclure ce cas de l'énoncé.

## 15

1. $A$ est indépendant de lui-même ssi $P(A)=P(A)^2$, soit $P(A)\in\{0,1\}$.
2. Les $2^n$ intersections obtenues en choisissant pour chaque $i$ soit $A_i$, soit son complémentaire, sont deux à deux disjointes, de probabilité strictement positive par indépendance. Chacune contient donc au moins un point de $\Omega$; $|\Omega|\geq2^n$.

## 16

Prendre les supports de probabilités strictement positives et poser $a=\min\operatorname{supp}X$, $b=\max\operatorname{supp}X$, $c=\min\operatorname{supp}Y$. L'indépendance donne


```math
\min\operatorname{supp}(X+Y)=a+c=\min\operatorname{supp}(2X)=2a,
```


donc $c=a$. Alors


```math
P(X=a)P(Y=a)=P(X+Y=2a)=P(2X=2a)=P(X=a)>0,
```


d'où $P(Y=a)=1$. Les maxima des supports donnent à leur tour $b+a=2b$, donc $a=b$. Ainsi $P(X=a)=1$.

## 17

1. En notant $F_k$ « face » et $P_k=F_k^c$ :
   a) $A=(F_1\cap F_3\cap\cdots\cap F_{2n-1}\cap P_2\cap\cdots\cap P_{2n})\cup(P_1\cap P_3\cap\cdots\cap P_{2n-1}\cap F_2\cap\cdots\cap F_{2n})$.
   b) $B=\bigcup_{j=1}^{2n}(F_1\cap\cdots\cap F_{j-1}\cap P_j\cap F_{j+1}\cap\cdots\cap F_{2n})$.
   c) $C=\bigcup_{k=0}^{2n}(F_1\cap\cdots\cap F_k\cap P_{k+1}\cap\cdots\cap P_{2n})$.
2. Les événements des unions sont disjoints :


```math
P(A)=2[p(1-p)]^n,\quad P(B)=2n(1-p)p^{2n-1},\quad P(C)=\sum_{k=0}^{2n}p^k(1-p)^{2n-k}.
```



## 18

Point par point, si $m=\sum_i\mathbf1_{A_i}$, alors $\mathbf1_{\cup A_i}\geq m-\binom m2$ (égalité pour $m=0,1,2$; le membre droit est ensuite au plus $1$). Prendre l'espérance donne la formule.

## 19

1. $1-(5/6)^4$.
2. $4(1/6)(5/6)^3$.
3. Le complément est que les quatre résultats soient distincts, de probabilité $6\cdot5\cdot4\cdot3/6^4=5/18$. Réponse : $13/18$.

## 20

Les arrangements équiprobables des lettres de BAOBAB sont $6!/(3!2!)=60$; un seul redonne BAOBAB. Probabilité $1/60$.

## 21

1. $\binom66\binom62/\binom{12}8=1/33$.
2. Avec remise, la probabilité d'au moins un succès en $n$ essais vaut $1-(32/33)^n$. Elle dépasse $1/2$ dès


```math
n>\frac{\ln(1/2)}{\ln(32/33)}\simeq22{,}53,
```


soit $n\geq23$.

## 22

Une semaine : $1-\binom{97}{5}/\binom{100}{5}$. Cinq semaines indépendantes : $1-(97/100)^5$. Numériquement, les probabilités valent environ $0{,}1440$ et $0{,}1413$; acheter les cinq billets la même semaine est légèrement préférable.

## 23

1. $\displaystyle \frac n{n+b}\frac b{n+b-1}$.
2. Les couleurs doivent alterner. Si $|n-b|>1$, la probabilité est nulle. Si $n=b$, il y a deux suites de couleurs possibles; si $|n-b|=1$, une seule. Chaque suite de couleurs a probabilité $n!b!/(n+b)!$. Ainsi la probabilité vaut respectivement $2n!b!/(n+b)!$ ou $n!b!/(n+b)!$.

## 24

1. Pour $n\geq3$, probabilité que les deux premiers entiers appartiennent au second tirage : $\binom{n-2}{1}/\binom n3=6/(n(n-1))$.
2. Probabilité que les trois entiers du second tirage évitent les deux premiers : $\binom{n-2}{3}/\binom n3$ (nulle si $n<5$).

## 25

Les six multiensembles de somme $9$ ont au total $25$ permutations ordonnées : $6+6+3+3+6+1$. Ceux de somme $10$ en ont $27$ : $6+6+3+6+3+3$. Les deux sommes ont six représentations non ordonnées, mais les permutations sont plus nombreuses pour $10$.

## 26

1. En plaçant les objets indépendamment et uniformément, la probabilité vaut


```math
\frac{n(n-1)\cdots(n-k+1)}{n^k}\quad(0\leq k\leq n),
```


et $0$ pour $k>n$.
2. Avec des dates indépendantes et uniformes sur $365$ jours,


```math
P(\text{date commune})=1-\prod_{j=0}^{m-1}\frac{365-j}{365}.
```


Les premiers effectifs dépassant $0.5$, $0.9$, $0.99$ sont respectivement $23$, $41$, $57$.
3. a) Sur $]-1/2,1/2[$, poser $g(x)=\ln(1+x)-x+x^2$. Alors


```math
g'(x)=\frac{x(1+2x)}{1+x},\qquad g(x)\geq g(0)=0.
```


La fonction $x-\ln(1+x)$ a également son minimum en $0$. Ainsi $x-x^2\leq\ln(1+x)\leq x$ sur cet intervalle.
b) Pour $k=\lfloor t\sqrt n\rfloor$, les nombres $-j/n$ sont dans cet intervalle pour $n$ assez grand. En sommant les bornes,


```math
-\frac{k(k-1)}{2n}-\frac1{n^2}\sum_{j=0}^{k-1}j^2\leq\ln p_n\leq-\frac{k(k-1)}{2n}.
```


Le terme principal tend vers $-t^2/2$ et l'erreur est $O(k^3/n^2)=O(n^{-1/2})$. Donc $p_n\to e^{-t^2/2}$.

## 27

Pour $1\leq k<n$, $P(N\geq k)=1/k!$ : parmi les $k!$ ordres possibles de $\sigma(1),\ldots,\sigma(k)$, un seul est croissant. Donc


```math
P(N=k)=\frac1{k!}-\frac1{(k+1)!}\quad(k<n),\qquad P(N=n)=\frac1{n!}.
```



## 28

1. $P(X\in k\mathbb Z)=\lfloor n/k\rfloor/n$, donc $1/k$ si $k\mid n$. Pour des $k_i$ premiers entre eux divisant $n$, le théorème chinois donne $P(\cap_i\{k_i\mid X\})=1/(\prod_i k_i)=\prod_iP(k_i\mid X)$.
2. Inclusion-exclusion sur les premiers divisant $n$ : $\varphi(n)/n=\prod_{p\mid n}(1-1/p)$.
3. Le nombre d'entiers $x\leq n$ tels que $\gcd(x,n)=n/d$ est $\varphi(d)$; donc $P(\gcd(X,n)=n/d)=\varphi(d)/n$. En sommant : $\sum_{d\mid n}\varphi(d)=n$.

## 29

1. $P(T=k)=p(1-p)^{k-1}$ pour $1\leq k\leq n$ et $P(T=+\infty)=(1-p)^n$.
2. a) Pour toute fenêtre de longueur $r$, la probabilité de la séquence est $q=p^s(1-p)^{r-s}$.
b) Les $\lfloor n/r\rfloor$ blocs disjoints sont indépendants; ainsi $P(E)\leq(1-q)^{\lfloor n/r\rfloor}\to0$. Presque sûrement, la séquence finit par apparaître dans les essais prolongés indéfiniment.

## 30

1. Probabilité initiale : $1/3$.
2. Le maître révèle toujours un verre vide parmi les deux autres. Si l'on change, on gagne exactement lorsque le choix initial était faux, probabilité $2/3$; il faut donc changer.

## 31

Avec $p_n=P(\text{tartines au jour }n)$,


```math
p_{n+1}=\frac34p_n+\frac15(1-p_n)=\frac{11}{20}p_n+\frac15.
```


Le point fixe vaut $4/9$ et $p_n-4/9=(11/20)^n(p_0-4/9)\to0$.

## 32

1. Il y a $k+2$ boules après le $k$-ième tirage.
2. Initialement $N_0=1$ est uniforme sur $\{1\}$. Si $N_k$ est uniforme sur $\{1,\ldots,k+1\}$, alors pour $1\leq j\leq k+2$,


```math
P(N_{k+1}=j)=\frac1{k+1}\frac{k+2-j}{k+2}+\frac1{k+1}\frac{j-1}{k+2}=\frac1{k+2}.
```


La propriété suit par récurrence.

## 33

La matrice est $M=\frac14\begin{pmatrix}2&0&2\\1&3&0\\1&3&0\end{pmatrix}$. La formule des probabilités totales donne $\pi_{k+1}=\pi_kM$. Le calcul donne


```math
4M^3-5M^2=-M,\qquad M(4M^2-5M+I)=0.
```


Les valeurs propres sont $0,1,1/4$. Pour $n\geq1$,


```math
M^n=A+4^{-n}4(M-A),\qquad A=\begin{pmatrix}1/3&1/2&1/6\\1/3&1/2&1/6\\1/3&1/2&1/6\end{pmatrix}.
```


Donc $M^n\to A$ et $P(X_n=j)\to(1/3,1/2,1/6)_j$.

## 34

1. a) $c_1=4/9$, $c_2=(1/3)(4/9)=4/27$. $P_{G_1\cap G_2}(C_{k+2})=0$; conditionnellement à $G_1$, il faut perdre en deuxième partie puis attendre le premier doublé dans la suite, donc $P_{G_1}(C_{k+2})=c_k/3$. b) En séparant $G_1$ et $\overline G_1$, on obtient $c_{k+2}=\frac13c_{k+1}+\frac29c_k$. Les racines sont $2/3,-1/3$ et


```math
c_k=\frac8{27}\left(\frac23\right)^{k-1}+\frac4{27}\left(-\frac13\right)^{k-1}.
```


2. a) Les deux vecteurs de Bernoulli ont même loi par invariance de la loi produit sous décalage des indices. b) Conditionner par $X_1=0$ enlève le premier indice : $P_{X_1=0}(T=k+1)=P(T=k)$.

## 35

1. Choisir une partie de taille $s$ d'un ensemble de taille $n$, puis y distinguer $k$ éléments, revient à choisir les $k$ éléments distingués puis les $s-k$ autres :


```math
\binom ns\binom sk=\binom nk\binom{n-k}{s-k}.
```


2. $S\sim\mathcal B(n,1/6)$. Conditionnellement à $S=s$, $F\sim\mathcal B(s,1/2)$. Pour $0\leq k\leq n$,


```math
P(F=k)=\sum_{s=k}^n\binom ns\left(\frac16\right)^s\left(\frac56\right)^{n-s}\binom sk2^{-s}
```




```math
=\binom nk\left(\frac1{12}\right)^k\sum_{r=0}^{n-k}\binom{n-k}r\left(\frac1{12}\right)^r\left(\frac56\right)^{n-k-r}
```




```math
=\binom nk\left(\frac1{12}\right)^k\left(\frac{11}{12}\right)^{n-k}.
```


Donc $F\sim\mathcal B(n,1/12)$.

## 36

Les deux premiers six apparaissent ensemble au rang $k$ exactement si les $2(k-1)$ résultats précédents sont différents de six et les deux résultats du rang $k$ valent six. Les événements sont disjoints, donc


```math
P(\text{premiers six simultanés})=\sum_{k=1}^n\frac1{36}\left(\frac{25}{36}\right)^{k-1}=\frac1{11}\left(1-\left(\frac{25}{36}\right)^n\right).
```



## 37

1. La première intersection est du côté de $A$; les suivantes alternent entre les côtés de $B$ et de $A$. Une sortie par $B$ se produit donc après un nombre pair d'intersections.
2. Au premier carrefour, les deux choix mènent au circuit. Au deuxième, la sortie par $B$ a probabilité $1/2$. Pour atteindre la prochaine occasion de sortir par $B$, il faut ensuite éviter la sortie par $B$, puis celle par $A$, avec probabilité $(1/2)^2=1/4$. Ainsi


```math
P(\text{sortie par $B$ à l'intersection $2j$})=\frac12\left(\frac14\right)^{j-1},
```




```math
P(\text{sortie indemne})=\frac12\sum_{j=0}^{n-1}4^{-j}=\frac23(1-4^{-n})\longrightarrow\frac23.
```



## 38

1. a) Il faut que les $n$ parties de chaque joueur soient perdues : probabilité $((1-a)(1-b))^n$. b) Posons $r=(1-a)(1-b)$. Les probabilités que $A$ et $B$ gagnent valent respectivement $a\sum_{j=0}^{n-1}r^j$ et $(1-a)b\sum_{j=0}^{n-1}r^j$. Équilibre ssi $a=b(1-a)$, soit $a=b/(1+b)$.
2. Les sommes $9,10,11,12$ correspondent à $4+3+2+1=10$ couples, donc $a=10/36=5/18$. Pour $B$, $b=1-(4/6)^2=5/9$. Alors


```math
b(1-a)=\frac59\frac{13}{18}=\frac{65}{162}>\frac{45}{162}=a.
```


$B$ a la plus grande probabilité de gagner le jeu.

## 39

1. Pour chaque face $i$, la probabilité qu'elle n'apparaisse pas vaut $(5/6)^n$.
2. Inclusion-exclusion :


```math
1-3(5/6)^n+3(4/6)^n-(3/6)^n.
```



## 40

1. L'intuition suggère une limite $e^{-1}$.
2. Par inclusion-exclusion sur les événements « le cadeau $i$ est attribué à $i$ »,


```math
|D_n|=\sum_{k=0}^n(-1)^k\binom nk(n-k)!=n!\sum_{k=0}^n\frac{(-1)^k}{k!}.
```


3. La probabilité est $|D_n|/n!=\sum_{k=0}^n(-1)^k/k!\to e^{-1}$.

## 41

Pour une face donnée, la probabilité qu'elle reste visible à chaque lancer est $(3/4)^n$. Deux faces données restent visibles simultanément avec probabilité $(1/2)^n$. L'inclusion-exclusion donne


```math
4(3/4)^n-6(1/2)^n+4(1/4)^n,
```


donc un équivalent $4(3/4)^n$.

## 42

Il y a cinq positions possibles pour OUI; chacune donne $26^4$ mots. Deux occurrences ne peuvent se chevaucher, et les trois couples de positions disjointes sont $(1,4),(1,5),(2,5)$; chaque intersection contient $26$ mots. Ainsi


```math
P(\text{OUI apparaît})=\frac{5\cdot26^4-3\cdot26}{26^7}.
```



## 43

Pour $X,Y$ Bernoulli$(1/2)$, $(S,D)$ prend $(0,0),(1,1),(1,-1),(2,0)$ avec probabilité $1/4$ chacun; $S,D$ ne sont pas indépendantes puisque $P(S=0,D=0)=1/4\ne P(S=0)P(D=0)=1/8$. Enfin $SD=X^2-Y^2=X-Y$, donc $E(SD)=0=E(S)E(D)$.

## 44

Le nombre total de boules est $n(2n+1)$; $P(N=k)=k/[n(2n+1)]$ pour $1\leq k\leq2n$. Donc


```math
E(N)=\frac{\sum_{k=1}^{2n}k^2}{n(2n+1)}=\frac{4n+1}3.
```


De plus


```math
P(N>n)=\frac{3n+1}{2(2n+1)}\to\frac34,\qquad P(N\text{ pair})=\frac{n+1}{2n+1}\to\frac12.
```



## 45

L'espérance du gain par tirage est $bg/(n+b)-n/(n+b)$. Pour qu'elle soit nulle, choisir $g=n/b$.

## 46

Pour $1\leq k\leq n$,


```math
P(Y=k)=\sum_{x=k}^n\frac1n\frac1x=\frac{H_n-H_{k-1}}n.
```


Puis $E(Y)=E(E(Y\mid X))=E((X+1)/2)=(n+3)/4$.

## 47

Sous l'hypothèse de crues annuelles indépendantes, une crue survient chaque année avec probabilité $1/100$. La probabilité d'aucune crue en $100$ ans vaut


```math
\left(1-\frac1{100}\right)^{100}\simeq e^{-1}.
```



## 48

1. Pour $k\leq m\leq n$, $P(M\leq m)=\binom mk/\binom nk$, donc $P(M=m)=\binom{m-1}{k-1}/\binom nk$.
2. a) Par la formule de Pascal et télescopage, $\sum_{i=k}^n\binom ik=\binom{n+1}{k+1}$.
b) Ainsi


```math
E(M)=\frac1{\binom nk}\sum_{m=k}^n m\binom{m-1}{k-1}=\frac{k}{\binom nk}\binom{n+1}{k+1}=\frac{k(n+1)}{k+1}.
```



## 49

Par symétrie, $P(X_{i+1}>X_i)=(p-1)/(2p)$ et $P(X_{i+1}=X_i)=1/p$, donc $P(X_{i+1}\geq X_i)=(p+1)/(2p)$. Par linéarité, $E(N)=(n-1)(p+1)/(2p)$.

## 50

1. $X=\sum_{k=0}^{n-1}\mathbf1_{\{X>k\}}$ point par point; prendre l'espérance donne l'identité.
2. $P(M_n>k)=1-(k/p)^n$ pour $0\leq k<p$, donc


```math
E(M_n)=\sum_{k=0}^{p-1}\left(1-(k/p)^n\right)=p-p^{-n}\sum_{k=0}^{p-1}k^n\longrightarrow p.
```



## 51

1. $P(I\geq k)=((n-k+1)/n)^2$, donc $P(I=k)=(2n-2k+1)/n^2$ et


```math
E(I)=\sum_{j=1}^n j^2/n^2=\frac{(n+1)(2n+1)}{6n}.
```


2. Pour $n\geq2$, $P(I=n,S=n)=1/n^2\ne P(I=n)P(S=n)$; elles ne sont pas indépendantes.
3. $I+S=U+V$, donc $E(S)=2E(U)-E(I)=n+1-E(I)=\frac{(n+1)(4n-1)}{6n}$.
4. Pour $i<j$, $P(I=i,S=j)=2/n^2$; pour $i=j$, $P(I=i,S=i)=1/n^2$; nul si $i>j$.

## 52

1. Les positions des deux noires sont équiprobables parmi les $\binom n2$ paires. Donc $P(R_1=i)=(n-i)/\binom n2$ pour $1\leq i<n$, et $E(R_1)=(n+1)/3$.
2. Conditionnellement à $R_1=i$, $R_2$ est uniforme sur $\{i+1,\ldots,n\}$. Ainsi $P(R_2=j)= (j-1)/\binom n2$ pour $2\leq j\leq n$, et $E(R_2)=2(n+1)/3=2E(R_1)$.

## 53

1. $1/x\leq(a+b-x)/(ab)$ équivaut à $(x-a)(b-x)\geq0$.
2. Après espérance, $E(1/X)\leq(a+b-E(X))/(ab)$. Par conséquent


```math
E(X)E(1/X)\leq\frac{E(X)(a+b-E(X))}{ab}\leq\frac{(a+b)^2}{4ab}.
```



## 54

1. a) Une moyenne convexe de valeurs de l'intervalle reste dans l'intervalle. b) Pour une loi finie $P(X=x_i)=p_i$, l'inégalité de concavité finie donne $\sum_i p_if(x_i)\leq f(\sum_i p_ix_i)$ (récurrence sur le nombre de valeurs).
2. Pour $u>0$, $u\geq1+\ln u$. En prenant $u=X/Y$,


```math
E(X/Y)\geq1+E(\ln X)-E(\ln Y)=1,
```


car $X$ et $Y$ ont même loi.

## 55

1. Par indépendance et même loi,


```math
\mathbb E(Z_1\overline{Z_2})=\mathbb E(Z_1)\mathbb E(\overline{Z_2})=\mathbb E(Z_1)\overline{\mathbb E(Z_1)}=|\mathbb E(Z_1)|^2.
```


2. a) Appliquer 1 à $Z_1=e^{iX}$, $Z_2=e^{iY}$ et prendre les parties réelles :


```math
|\mathbb E(e^{iX})|^2=\mathbb E(e^{i(X-Y)})=\mathbb E(\cos(X-Y)).
```


b) Comme $|\cos x|\leq1$,


```math
|\cos x|\geq\cos^2x=\frac{1+\cos(2x)}2.
```


c) On a $|X-Y|\leq t\leq\pi/2$, donc $\cos(X-Y)\geq0$. Avec b), puis a) appliqué à $2X,2Y$,


```math
|\mathbb E(e^{iX})|^2\geq\frac{1+\mathbb E(\cos(2X-2Y))}2=\frac{1+|\mathbb E(e^{2iX})|^2}2\geq\frac12.
```


De plus $\cos(X-Y)\geq\cos t$, donc


```math
|\mathbb E(e^{iX})|\geq\max\left(\frac1{\sqrt2},\sqrt{\cos t}\right).
```


d) Pour $X$ uniforme sur $\{0,\pi/2\}$,


```math
|\mathbb E(e^{iX})|=\left|\frac{1+i}{2}\right|=\frac1{\sqrt2}.
```


3. Prendre $X$ uniforme sur la liste $\theta_1,\ldots,\theta_n$, comptée avec multiplicité. Elle est à valeurs dans $[\min\theta_k,\max\theta_k]$, de longueur au plus $\pi/2$. Alors


```math
\left|\sum_{k=1}^ne^{i\theta_k}\right|=n|\mathbb E(e^{iX})|\geq\frac n{\sqrt2}.
```



## 56

1. Les $A_{k,x}$ sont disjoints et $A_x=\bigcup_{k=1}^nA_{k,x}$.
2. a) Si $|S_k|\geq3x$ et $|S_n|<x$, alors $|S_n-S_k|\geq|S_k|-|S_n|>2x$.
b) $A_{k,3x}$ ne dépend que de $X_1,\ldots,X_k$, tandis que $S_n-S_k$ ne dépend que des termes suivants; indépendance.
c) En séparant selon $|S_n|\geq x$, puis avec a), b), et en sommant les événements disjoints $A_{k,3x}$ :


```math
P(A_{3x})\leq P(|S_n|\geq x)+\max_{1\leq k\leq n}P(|S_n-S_k|\geq2x).
```


d) Si $|S_n-S_k|\geq2x$, alors $|S_n|\geq x$ ou $|S_k|\geq x$. Donc le dernier maximum est au plus $2M$, avec $M=\max_jP(|S_j|\geq x)$. Ainsi


```math
P(\max_k|S_k|\geq3x)=P(A_{3x})\leq3M.
```

