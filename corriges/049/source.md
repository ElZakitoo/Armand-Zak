# corrigé zakito

[Énoncé](https://christophebertault.fr/documents/coursetexercices/Exercices%20-%20Complements%20probabilistes.pdf)

## 1



```math
\mathbb E((X-x)^2)=\mathbb V(X)+(x-\mathbb E(X))^2.
```


Le minimum est atteint uniquement en $x=\mathbb E(X)$.

## 2

1. Comme $(b-X)(X-a)\geq0$,


```math
0\leq\mathbb E((b-X)(X-a))=(a+b)\mathbb E(X)-ab-\mathbb E(X^2).
```


Ainsi


```math
\mathbb V(X)\leq (a+b)\mathbb E(X)-ab-\mathbb E(X)^2=(b-\mathbb E(X))(\mathbb E(X)-a).
```


2. Le produit ci-dessus vaut au plus $(b-a)^2/4$ (maximum au milieu). Pour $B\sim\mathcal B(1,1/2)$, $Y=a+(b-a)B$ a pour variance $(b-a)^2/4$. La borne est donc optimale.

## 3

Pour $Z=\mathbf1_A+2\mathbf1_B$,
La valeur $2$ exige $B\setminus A$, de probabilité $1/3-1/4=1/12$, et $Z=3$
sur $A\cap B$. Ainsi


```math
\mathbb P(Z=0)=\frac5{12},\quad\mathbb P(Z=1)=\frac14,\quad
\mathbb P(Z=2)=\frac1{12},\quad\mathbb P(Z=3)=\frac14.
```




```math
\mathbb E(Z)=\frac76,\quad\mathbb E(Z^2)=\frac{17}6,\quad
\mathbb V(Z)=\frac{53}{36},\quad\boxed{\sigma(Z)=\frac{\sqrt{53}}6}.
```



## 4

Si $m=1$, $\mathbb E(U)=(n+1)/2$ et $\mathbb E(U^2)=(n+1)(2n+1)/6$, d'où


```math
\mathbb V(U)=\frac{n^2-1}{12}.
```


En général $U=m+U_0-1$, où $U_0$ est uniforme sur $\{1,\ldots,n-m+1\}$; ainsi


```math
\mathbb V(U)=\frac{(n-m+1)^2-1}{12}.
```



## 5

1. $\operatorname{cov}(\mathbf1_A,\mathbf1_B)=\mathbb P(A\cap B)-\mathbb P(A)\mathbb P(B)$. Cauchy-Schwarz donne


```math
|\operatorname{cov}(\mathbf1_A,\mathbf1_B)|\leq\sqrt{\mathbb V(\mathbf1_A)\mathbb V(\mathbf1_B)}
\leq\sqrt{\frac14\cdot\frac14}=\frac14.
```


2. Cauchy-Schwarz donne


```math
\mathbb E(X)=\mathbb E(X\mathbf1_{X\geq1})\leq\sqrt{\mathbb E(X^2)\mathbb P(X\geq1)},
```


d'où $\mathbb P(X\geq1)\geq\mathbb E(X)^2/\mathbb E(X^2)$.

## 6

Par Cauchy-Schwarz, $|\operatorname{cov}(X,Y)|\leq\sigma(X)\sigma(Y)$, donc $|\rho|\leq1$. L'égalité équivaut à la dépendance linéaire presque sûre des variables centrées : $Y-\mathbb E(Y)=a(X-\mathbb E(X))$ p.s., avec $a\ne0$. C'est exactement $Y=aX+b$ p.s. pour $a,b\in\mathbb R$.

## 7

Posons $A=\{X\geq\eta\mathbb E(X)\}$ et $Y=X\mathbf1_A$. Alors


```math
\mathbb E(Y)\geq(1-\eta)\mathbb E(X),\qquad \mathbb E(Y^2)\leq\mathbb E(X^2).
```


Par Cauchy-Schwarz, $\mathbb E(Y)^2\leq\mathbb E(Y^2)\mathbb P(A)$; donc


```math
\mathbb P(X\geq\eta\mathbb E(X))\geq(1-\eta)^2\frac{\mathbb E(X)^2}{\mathbb E(X^2)}.
```



## 8

Écrivons $D=\sum_{\sigma\in\mathfrak S_n}\varepsilon(\sigma)\prod_iR_{i,\sigma(i)}$. Chaque monôme a une espérance nulle, donc $\mathbb E(D)=0$. Au carré, deux monômes distincts contiennent au moins une entrée apparaissant une seule fois; leur produit est d'espérance nulle. Les $n!$ termes diagonaux valent $1$, d'où $\mathbb V(D)=\mathbb E(D^2)=n!$. Ainsi


```math
\mathbb P\!\left(|D|\geq\sqrt{(n+1)!}\right)\leq\frac{n!}{(n+1)!}
=\frac1{n+1}\longrightarrow0.
```



## 9

1. $\sigma(i)$ est uniforme sur $\{1,\ldots,n\}$; son espérance vaut $(n+1)/2$ et sa variance $(n^2-1)/12$.
2. Écrivons $F=\sum_i\mathbf1_{E_i}$. Alors $\mathbb E(F)=1$. Pour $i\ne j$,


```math
\operatorname{cov}(\mathbf1_{E_i},\mathbf1_{E_j})=\frac1{n(n-1)}-\frac1{n^2}=\frac1{n^2(n-1)}.
```


Donc $\mathbb V(F)=n(1/n)(1-1/n)+n(n-1)/(n^2(n-1))=1$. Tchebychev donne


```math
\mathbb P(F\geq4)\leq\mathbb P(|F-1|\geq3)\leq\frac{\mathbb V(F)}{3^2}=\frac19.
```


3. Pour que le cycle de $1$ soit de longueur $k$, on choisit ses $k-1$ autres éléments, on les ordonne en cycle, puis on permute le reste : il y a $\binom{n-1}{k-1}(k-1)!(n-k)!=(n-1)!$ permutations, soit une probabilité $1/n$. Ainsi $L$ est uniforme sur $\{1,\ldots,n\}$.
4. a) Le nouvel élément est soit un cycle singleton, soit inséré après l'un des $n$ éléments dans son cycle; d'où $c_{n+1,k}=c_{n,k-1}+nc_{n,k}$.
b) Pour une permutation uniforme de $n+1$ éléments, le nouveau point est singleton avec probabilité $1/(n+1)$; sinon il est inséré dans un cycle existant. L'ajout d'un point à une permutation uniforme de $n$ réalise une bijection uniforme. Ainsi $\mathbb E(N_{n+1})=\mathbb E(N_n)+1/(n+1)$, donc $\mathbb E(N_n)=H_n\sim\ln n$.

## 10

1. Si $X$ et $Y$ sont indépendantes, $\mathbb E_{\{Y=y\}}(X)=\mathbb E(X)$. En découpant suivant les valeurs de $Y$,


```math
\mathbb E(X)=\sum_{y\in Y(\Omega)}\mathbb P(Y=y)\mathbb E_{\{Y=y\}}(X).
```


Les termes avec probabilité nulle sont nuls par convention.
2. Par indépendance de $T$ et des $X_i$, conditionnellement à $T=t$, la somme $S_T$ a la loi de $S_t$, ce qui donne l'égalité demandée en prenant l'espérance de $f$. Puis


```math
\mathbb E(S_T)=\sum_t\mathbb P(T=t)\mathbb E(S_t)=\sum_t\mathbb P(T=t)t\mathbb E(X_1)=\mathbb E(T)\mathbb E(X_1).
```


Si les $X_i$ sont centrées, conditionnellement à $T=t$, $\mathbb V(S_T)=t\mathbb V(X_1)$ et $\mathbb E(S_T\mid T)=0$; donc $\mathbb V(S_T)=\mathbb E(T)\mathbb V(X_1)$.

## 11

Les variables $X_0=1,X_1,\ldots,X_n$ sont deux à deux non corrélées. Donc


```math
\mathbb V\!\left(\lambda_0X_0+\cdots+\lambda_nX_n\right)=\sum_{k=1}^n\lambda_k^2\mathbb V(X_k).
```


Si la combinaison est nulle p.s., sa variance impose $\lambda_k=0$ pour $k\geq1$, puis $\lambda_0=0$. Elles sont libres dans $\mathbb R^\Omega$; cette espace est de dimension $|\Omega|$, donc $|\Omega|\geq n+1$.

## 12

1. Pour $x,y\geq0$, l'inégalité pondérée AM-GM donne $x^{1/p}y^{1/q}\leq x/p+y/q$ (avec $1/p+1/q=1$).
2. Appliquée à $x=X^p,y=Y^q$ et prise en espérance, elle donne $\mathbb E(XY)\leq1$ lorsque les deux moments valent $1$.
3. Normaliser $X$ et $Y$ par $\mathbb E(X^p)^{1/p}$ et $\mathbb E(Y^q)^{1/q}$ donne


```math
\mathbb E(XY)\leq\mathbb E(X^p)^{1/p}\mathbb E(Y^q)^{1/q}.
```


4. Pour des variables réelles, appliquer le résultat à $|X|,|Y|$ et utiliser $|XY|=|X||Y|$. Si $\mathbb E(|X|^p)=0$ ou $\mathbb E(|Y|^q)=0$, la variable correspondante est nulle p.s. et l'inégalité est immédiate; sinon, on peut normaliser comme à la question 3.

## 13

1. Sur $A=\{X-\mathbb E(X)\geq a\}$, $X-\mathbb E(X)+t\geq a+t$. Markov appliqué au carré donne


```math
\mathbb P(A)\leq\frac{\mathbb E((X-\mathbb E(X)+t)^2)}{(a+t)^2}=\frac{V(X)+t^2}{(a+t)^2}.
```


2. Si $V(X)>0$, le minimum est atteint en $t=V(X)/a$ et vaut $V(X)/(V(X)+a^2)$. Si $V(X)=0$, la probabilité est nulle et le résultat est immédiat.
3. Appliquer la borne unilatérale aux deux queues :


```math
\mathbb P(|X-\mathbb E(X)|\geq a)\leq\frac{2V(X)}{V(X)+a^2}\leq\frac{2V(X)}{a^2}.
```


L'inégalité de Bienaymé-Tchebychev donne $V(X)/a^2$. La borne $2V(X)/(V(X)+a^2)$ est meilleure si $V(X)\geq a^2$, moins bonne si $V(X)\leq a^2$ (égalité si $V(X)=a^2$).

## 14

1. Markov donne $\mathbb P(X\geq\alpha)\leq e^{-t\alpha}\mathbb E(e^{tX})$.
2. a) $g(u)=(1+u+u^2)e^{-u}$ a pour dérivée $g'(u)=u(1-u)e^{-u}$; elle est négative sur $[-1,0]$ et positive sur $[0,1]$. Le minimum est $g(0)=1$.
b) Le développement de $e^{tX}$ et $|X|\leq1$, $\mathbb E(X)=0$ donnent, pour $0\leq t\leq1$,


```math
\mathbb E(e^{tX})\leq1+t^2\mathbb E(X^2)\leq1+\sigma^2t^2\leq e^{\sigma^2t^2}.
```


La même borne vaut pour $-X$.
3. Pour $0\leq t\leq1$, $\mathbb P(X\geq\lambda\sigma)\leq e^{-t\lambda\sigma+\sigma^2t^2}$. Choisir $t=\lambda/(2\sigma)$, admissible si $\lambda\leq2\sigma$, puis doubler pour les deux queues :


```math
\mathbb P(|X|\geq\lambda\sigma)\leq2e^{-\lambda^2/4}.
```



## 15

Pour $t>0$, l'inégalité de Markov appliquée à $e^{tX}$ et la fonction génératrice binomiale donnent


```math
\mathbb P(X\geq n(p+\varepsilon))\leq e^{-n(p+\varepsilon)t}(1-p+pe^t)^n.
```


Le logarithme du facteur par $n$ vaut $h(t)=-(p+\varepsilon)t+\ln(1-p+pe^t)$, avec $h(0)=0$ et $h'(0)=-\varepsilon<0$. Il existe donc $t>0$ tel que $\eta=e^{h(t)}<1$, et la probabilité est au plus $\eta^n$.

## 16

1. $\cosh x=\sum_{k\geq0}x^{2k}/(2k)!\leq\sum_{k\geq0}x^{2k}/(2^kk!)=e^{x^2/2}$, car $(2k)!\geq2^kk!$.
2. a) La convexité de $x\mapsto e^{\lambda x}$ donne, pour $x\in[-1,1]$, sa majoration par la corde joignant $-1$ et $1$ : $e^{\lambda x}\leq\frac{1-x}{2}e^{-\lambda}+\frac{1+x}{2}e^\lambda=\cosh\lambda+x\sinh\lambda$. b) En prenant l'espérance, $\mathbb E(e^{\lambda X})\leq\cosh\lambda\leq e^{\lambda^2/2}$.
3. a) Indépendance et l'étape précédente donnent


```math
\mathbb E(e^{\lambda M})=\prod_{i=1}^n\mathbb E(e^{\lambda X_i/n})\leq e^{\lambda^2/(2n)}.
```


Comme $e^{\lambda|M|}\leq e^{\lambda M}+e^{-\lambda M}$, son espérance est au plus $2e^{\lambda^2/(2n)}$. b) Markov donne


```math
\mathbb P\left(|M|\geq\frac{t}{\sqrt n}\right)\leq2\exp\left(\frac{\lambda^2}{2n}-\frac{\lambda t}{\sqrt n}\right).
```


Prendre $\lambda=t\sqrt n$ donne $2e^{-t^2/2}$.
4. Appliquer le résultat à $(X_i-m)/a$ :


```math
\mathbb P\left(|M-m|\geq\frac{t}{\sqrt n}\right)\leq2e^{-t^2/(2a^2)}.
```


5. Pour $X\sim\mathcal B(n,p)$, écrire $X=\sum_{i=1}^nX_i$, où les $X_i$ sont Bernoulli$(p)$. L'étape précédente, avec $a=1$ et $t=\varepsilon\sqrt n$, donne


```math
\mathbb P(|X-np|\geq n\varepsilon)\leq2e^{-n\varepsilon^2/2}.
```



## 17

1. $\mathbb V(S_k)=\sum_{i=1}^k\sigma_i^2\leq\sigma^2$; Tchebychev donne $\mathbb P(|S_k|\geq x)\leq\sigma^2/x^2$.
2. Les $A_k$ sont disjoints et leur réunion est $\{\max_{1\leq i\leq n}|S_i|\geq x\}$. Comme $A_k$ dépend seulement de $X_1,\ldots,X_k$, $S_n-S_k$ est indépendant de $A_k$ et de moyenne nulle. Ainsi


```math
\mathbb E(S_n^2\mathbf1_{A_k})=\mathbb E(S_k^2\mathbf1_{A_k})+\mathbb E((S_n-S_k)^2)\mathbb P(A_k)\geq x^2\mathbb P(A_k).
```


En sommant, $\sum_k\mathbb E(S_n^2\mathbf1_{A_k})\leq\mathbb E(S_n^2)=\sigma^2$.
3. Le même développement montre $\mathbb E(S_n^2\mathbf1_{A_k})\geq\mathbb E(S_k^2\mathbf1_{A_k})$.
4. Donc


```math
x^2\mathbb P\left(\max_{1\leq i\leq n}|S_i|\geq x\right)\leq\sum_k\mathbb E(S_k^2\mathbf1_{A_k})\leq\sigma^2.
```



## 18

Si $X/Y>\mathbb E(X)/\mathbb E(Y)$ presque sûrement, alors, puisque $Y>0$,


```math
X>Y\frac{\mathbb E(X)}{\mathbb E(Y)}\quad\text{p.s.}
```


L'espérance donnerait $\mathbb E(X)>\mathbb E(X)$, contradiction. Le complément de cette inégalité stricte a donc une probabilité positive.

## 19

1. Supposons qu'il n'y ait qu'un nombre fini $p_1,\ldots,p_r$ de nombres premiers congrus à $2$ modulo $3$. L'entier $N=3p_1\cdots p_r-1$ vaut $2$ modulo $3$ et n'est divisible par aucun $p_i$. Ses facteurs premiers sont tous $1$ ou $2$ modulo $3$; comme leur produit vaut $2$ modulo $3$, au moins l'un est $2$ modulo $3$, donnant un nouveau premier, contradiction.
2. a) Écrivons $p=3k+2$. Les résidus de $I+I$ modulo $p$, où $I=\{k+1,\ldots,2k+1\}$, sont dans $\{0,1,\ldots,k\}\cup\{2k+2,\ldots,3k+1\}$, disjoint de $I$. Donc $I$ est sans somme modulo $p$. Pour tout $\Lambda\in(\mathbb Z/p\mathbb Z)^*$, si $a,b\in B$ et $a+b\in B$, alors $\Lambda^{-1}a,\Lambda^{-1}b,\Lambda^{-1}(a+b)\in I$, impossible.
b) Pour chaque $a\in A$, $\Lambda^{-1}a$ est uniforme sur les $p-1$ résidus non nuls. Ainsi $\mathbb P(a\in B)=|I|/(p-1)=(k+1)/(3k+1)>1/3$, et $\mathbb E|B|>|A|/3$. Il existe donc une réalisation telle que $|B|>|A|/3$.

## 20

1. Pour tout sommet $s$, l'événement $s\in V$ implique que $s$ et ses au moins $d$ voisins ne sont pas choisis dans $U$; donc $\mathbb P(s\in V)\leq(1-p)^{d+1}$. Par linéarité,


```math
\frac{\mathbb E(|U|+|V|)}{|S|}\leq p+(1-p)^{d+1}\leq p+e^{-(d+1)p}.
```


Choisir $p=\ln(d+1)/(d+1)$ (cas $d=0$ trivial) donne la borne $(\ln(d+1)+1)/(d+1)$.
2. Tout sommet hors $U\cup V$ n'est pas dans $V$, donc a un voisin dans $U$. Ainsi $U\cup V$ domine $S$. Il existe une réalisation de taille au plus son espérance, d'où la borne demandée.

## 21

Par indépendance,


```math
\mathbb E(|U|-|B|)=|S|p-|A|p^2.
```


Avec $p=|S|/(2|A|)$, cette quantité vaut $|S|^2/(4|A|)$. Il existe donc une réalisation telle que $|U|-|B|\geq |S|^2/(4|A|)$. En supprimant de $U$ au plus une extrémité par arête induite (au plus $|B|$ sommets), il reste une anticlique de taille au moins $|U|-|B|$.

## 22

1. Si $K=(S_n+n)/2$ est le nombre de pas $+1$, alors $K\sim\mathcal B(n,p)$, $S_n=2K-n$, $\mathbb E(S_n)=n(2p-1)$ et $\mathbb V(S_n)=4np(1-p)$. Par parité, $\mathbb P(S_{2n+1}=0)=0$.
2. a) Sur $\{S_n<0\}$, $e^{-tS_n}>1$, donc $\mathbb P(S_n<0)\leq\mathbb E(e^{-tS_n})=(pe^{-t}+(1-p)e^t)^n$. Si $p>1/2$, la dérivée en $0$ du facteur vaut $1-2p<0$; pour un $t>0$ assez petit, ce facteur est un $\eta<1$.
b) Si $p<1/2$, le facteur $pe^{-t}+(1-p)e^t$ est supérieur à $1$ pour tout $t>0$; la borne exponentielle décroissante n'est plus obtenue. En fait $\mathbb P(S_n<0)\to1$.

## 23

1. Pour $n$ sauts de Rademacher, $K=(S_n+n)/2\sim\mathcal B(n,1/2)$ et $S_n=2K-n$, donc $\mathbb E(S_n)=0$, $\mathbb V(S_n)=n$. $\mathbb P(S_{2n+1}=0)=0$ et


```math
q_n=\mathbb P(S_{2n}=0)=\binom{2n}{n}4^{-n}\sim\frac1{\sqrt{\pi n}},\qquad q_{n+1}=q_n\frac{2n+1}{2n+2}.
```


2. a) Vérification par les cas $k>0,k=0,k<0$ : $|k+1|+|k-1|=2|k|+2\mathbf1_{k=0}$. Conditionner par $S_n$ et utiliser l'équiprobabilité des deux pas donne $\mathbb E|S_{n+1}|=\mathbb E|S_n|+\mathbb P(S_n=0)$.
b) En sommant, seuls les temps pairs contribuent : $\mathbb E|S_{2n}|=\sum_{j=0}^{n-1}q_j=2nq_n$ (la dernière égalité se vérifie aussi par récurrence avec la relation entre $q_{n+1}$ et $q_n$). Donc $\mathbb E|S_{2n}|\sim2\sqrt{n/\pi}$, et $\mathbb E|S_n|\sim\sqrt{2n/\pi}$.
3. Un chemin en $n-m$ pas de $a$ à $b$ doit comporter $r=(n-m+b-a)/2$ pas montants. Il y en a


```math
C_{(m,a)}^{(n,b)}=\binom{n-m}{r},
```


si $r$ est entier entre $0$ et $n-m$, et zéro sinon.
4. a) Réfléchir le chemin jusqu'à son premier contact avec l'axe donne une bijection entre chemins de $(1,1)$ à $(n,k)$ touchant l'axe et chemins de $(1,-1)$ à $(n,k)$.
b) Le principe de réflexion donne pour les chemins positifs de $(0,0)$ à $(n,k)$ :


```math
\binom{n-1}{(n+k-2)/2}-\binom{n-1}{(n+k)/2}=\frac{k}{n}\binom{n}{(n+k)/2}=\frac{k}{n}C_{(0,0)}^{(n,k)}.
```


c) Les chemins allant de $0$ à $k>0$ ont même probabilité $2^{-n}$; le rapport des comptages donne


```math
\mathbb P(S_1\ne0,\ldots,S_n\ne0,S_n=k)=\frac{k}{n}\mathbb P(S_n=k).
```


5. Pour $k<0$, la symétrie donne le même résultat avec $|k|$; pour $k=0$, les deux côtés sont nuls. En sommant,


```math
\mathbb P(S_1\ne0,\ldots,S_n\ne0)=\frac{\mathbb E|S_n|}{n}\sim\sqrt{\frac{2}{n\pi}}.
```


