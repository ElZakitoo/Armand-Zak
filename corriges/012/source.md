# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td12-arithmetique.pdf)

## Autocorrection A

Les divisions successives sont



```math
\begin{aligned}
438&=8\cdot51+30,&51&=30+21,&30&=21+9,&21&=2\cdot9+3,\\
151&=77+74,&77&=74+3,&74&=24\cdot3+2,&3&=2+1,\\
1320&=720+600,&720&=600+120,&600&=5\cdot120,\\
63&=3\cdot17+12,&17&=12+5,&12&=2\cdot5+2,&5&=2\cdot2+1,\\
120&=5\cdot23+5,&23&=4\cdot5+3,&5&=3+2,&3&=2+1,\\
8136&=16\cdot492+264,&492&=264+228,&264&=228+36,&228&=6\cdot36+12.
\end{aligned}
```



Les divisions euclidiennes, suivies de la remontée de Bézout, donnent

| $(a,b)$ | $a\wedge b$ | Relation de Bézout |
|---|---:|---|
| $(438,51)$ | $3$ | $3=43\cdot51-5\cdot438$ |
| $(151,77)$ | $1$ | $1=51\cdot77-26\cdot151$ |
| $(1320,720)$ | $120$ | $120=2\cdot720-1320$ |
| $(63,17)$ | $1$ | $1=26\cdot17-7\cdot63$ |
| $(120,23)$ | $1$ | $1=47\cdot23-9\cdot120$ |
| $(8136,492)$ | $12$ | $12=215\cdot492-13\cdot8136$ |

## Autocorrection B

(i) $n+1\mid n+3$ équivaut à $n+1\mid2$, donc $n=0$ ou $1$. (ii) Le reste de $n^2+3n+5$ modulo $n+2$ est $3$. Il faut $n+2\mid3$, donc $n=1$, qui convient.

## Autocorrection C

$n^4-n^2=n^2(n-1)(n+1)$. Parmi trois entiers consécutifs, l’un est divisible par $3$, l’un est pair; si $n$ est pair, $n^2$ est divisible par $4$ ; si $n$ est impair, $n-1,n+1$ sont deux pairs, dont l’un est multiple de $4$. Le produit est divisible par $12$.

## Exercice 1

Écrivons $N=\sum_{i=0}^ra_i10^i$. Les congruences $10\equiv0\pmod{2,5,10}$ donnent les critères par le dernier chiffre; $10^i\equiv1\pmod{3,9}$ donne le critère de somme des chiffres; $10^i\equiv0\pmod4$ pour $i\ge2$ et $10^i\equiv0\pmod8$ pour $i\ge3$ montrent que seuls les deux ou trois derniers chiffres comptent; modulo 6 on combine 2 et 3; enfin $10^i\equiv(-1)^i\pmod{11}$ donne la somme alternée. Les divisions successives sont $14652=2\cdot7326=2^2\cdot3663=2^2\cdot3\cdot1221=2^2\cdot3^2\cdot407=2^2\cdot3^2\cdot11\cdot37$; $37$ est premier.

## Exercice 2

Le binôme donne $(n+1)^n-1=(1+n)^n-1=\sum_{k=1}^{n}\binom{n}{k}n^k$. Chaque terme est divisible par $n^2$: pour $k=1$, il vaut $n^2$, et pour $k\ge2$, il contient le facteur $n^k$.

## Exercice 3

(i) L’équation équivaut à $(n-2)(p-3)=6$. Les diviseurs signés de $6$ donnent $(n,p)=(3,9),(4,6),(5,5),(8,4),(1,-3),(0,0),(-1,1),(-4,2)$. (ii) En multipliant par $5np$, on obtient $(n-5)(p-5)=25$. Les couples de diviseurs signés donnent $(n,p)=(6,30),(10,10),(30,6),(4,-20),(-20,4)$; la paire donnant $(0,0)$ est exclue. (iii) On a $(n-2)^2-(p+1)^2=8$, donc $(n-p-3)(n+p-1)=8$. Les deux facteurs ont même parité; les paires possibles sont $(2,4),(4,2),(-2,-4),(-4,-2)$. Elles donnent $(n,p)=(5,0),(5,-2),(-1,-2),(-1,0)$.

## Exercice 4

Si $N$ est impair, $N=2+(N-2)$, avec $\gcd(2,N-2)=1$.

Si $N=2m$ avec $m$ pair, alors $m\ge4$ et



```math
N=(m-1)+(m+1),\qquad\gcd(m-1,m+1)\mid2.
```



Les deux termes sont impairs et $>1$, donc leur PGCD est $1$.

Si $N=2m$ avec $m$ impair, alors $m\ge5$ et



```math
N=(m-2)+(m+2),\qquad\gcd(m-2,m+2)\mid4.
```



Les deux termes sont encore impairs et $>1$, donc leur PGCD est $1$.

## Exercice 5

Modulo $n+1$, $n^2+1\equiv2$. Il faut donc $n+1\mid2$; comme $n>0$, cela impose $n=1$, qui convient.

## Exercice 6

1. Tout diviseur commun de $n(n+1)$ et $2n+1$ divise $2n(n+1)-n(2n+1)=n$ puis $2n+1$, donc divise $1$. 2. Un diviseur commun de $3n^2+2n$ et $n+1$ divise $3n^2+2n-3n(n+1)=-n$ et donc $n+1$, donc $1$.

## Exercice 7



```math
2(9k+4)-9(2k+1)=-1\implies\boxed{\gcd(2k+1,9k+4)=1}.
```





```math
\gcd(2k-1,9k+4)=\gcd(2k-1,k+8)=\gcd(k+8,17).
```





```math
\boxed{\gcd(2k-1,9k+4)=\begin{cases}17,&k\equiv9\pmod{17},\\1,&\text{sinon}.\end{cases}}
```



## Exercice 8

Le PGCD divise $3(2n+4)-2(3n+3)=6$. Pour $n\equiv0,1,2,3,4,5\pmod6$, les PGCD valent respectivement $1,6,1,2,3,2$; l’ensemble demandé est donc $\{1,2,3,6\}$.

## Exercice 9

Le PGCD de deux entiers positifs divise leur PPCM : $d\mid m$ est nécessaire.

Réciproquement, si $d\mid m$, le couple $(x,y)=(d,m)$ convient. Ainsi



```math
\boxed{\text{Existence}\iff d\mid m.}
```



Toutes les solutions s'écrivent $x=du$, $y=dv$, avec $uv=m/d$ et $\gcd(u,v)=1$.

## Exercice 10

Avec $d=x\wedge y$, $m=x\vee y$, on a $dm=xy$. L’égalité donne $d+m=x+y$. Écrire $x=da,y=db$, $(a,b)=1$, donne $m=dab$ et $d(a+b)=d(1+ab)$, donc $(a-1)(b-1)=0$. Ainsi $a=1$ ou $b=1$, c.-à-d. $x\mid y$ ou $y\mid x$.

## Exercice 11

Dans $n!$, chaque multiple de $p$ apporte une unité de valuation, chaque multiple de $p^2$ une unité supplémentaire, etc. Le nombre de multiples de $p^k$ dans $1,\ldots,n$ vaut $\lfloor n/p^k\rfloor$; en sommant, $v_p(n!)=\sum_{k\ge1}\lfloor n/p^k\rfloor$ (somme finie).

## Exercice 12

1. (a) Pour $x\ne0$, écrivons de façon unique $x=p^a u/v$ avec $a\in\mathbb Z$, $u\in\mathbb Z$, $v>0$, $\gcd(u,v)=1$ et $p\nmid uv$, puis posons $v_p(x)=a$; posons $v_p(0)=+\infty$. La décomposition des produits en facteurs premiers donne $v_p(xy)=v_p(x)+v_p(y)$. (b) Si $r=\min(v_p(x),v_p(y))$, écrivons $x=p^ru$, $y=p^rv$ avec $v_p(u),v_p(v)\ge0$; alors $x+y=p^r(u+v)$ et $v_p(x+y)\ge r$. 2. Posons $r=\lfloor\log_2n\rfloor$. Le seul terme de $H_n$ de valuation $-r$ est $1/2^r$; tous les autres ont valuation au moins $-(r-1)$. Ainsi $v_2(H_n)=-r$. 3. C’est négatif pour $n>1$, donc $H_n$ n’est pas entier. Pour $m=n+1$, $H_m-H_n=1/m$ n’est pas entier. Si $m\ge n+2$, l’intervalle contient un entier pair; soit $2^s$ la plus grande puissance de 2 divisant l’un de ses termes. Un seul terme a cette valuation: deux multiples distincts de $2^s$ à valuation exactement $s$ encadreraient un multiple de $2^{s+1}$ dans l’intervalle. Le terme de valuation minimale dans $\sum_{k=n+1}^m1/k$ est donc unique et cette valuation est strictement négative; la somme n’est pas entière.

## Exercice 13

Soit $k\ge2$ l’exposant et $a,a+1,a+2$ les trois entiers. Si $a$ est impair, ces nombres sont deux à deux premiers entre eux. Si leur produit est une puissance $k$-ième, chacun est une puissance $k$-ième; en particulier $a=u^k$ et $a+2=v^k$, impossible car deux puissances $k$-ièmes positives distinctes diffèrent d’au moins $2^k-1>2$. Si $a$ est pair, $a+1$ est premier avec $a(a+2)$. Une puissance $k$-ième produit imposerait $a+1=u^k$ et $a(a+2)=v^k$. Or $a(a+2)=(a+1)^2-1=u^{2k}-1$, différence de deux puissances $k$-ièmes égale à $1$, impossible: pour $u\ge2$, l’écart entre $u^{2k}$ et $(u^2-1)^k$ est supérieur à $1$, et $u=1$ contredit $a+1\ge3$.

## Exercice 14



```math
R_n=\frac{10^n-1}{9}.
```



Si $X\equiv1\pmod3$ et $3\nmid q$, alors



```math
\frac{X^q-1}{X-1}=1+X+\cdots+X^{q-1}\equiv q\not\equiv0\pmod3.
```



D'autre part, en écrivant $X=1+3t$,



```math
X^2+X+1=3(1+3t+3t^2)\implies v_3(X^3-1)=v_3(X-1)+1.
```



Pour $n=3^sq$, $3\nmid q$, appliquer la première identité à $X=10$, puis la seconde $s$ fois :



```math
v_3(10^n-1)=v_3(10^q-1)+s=2+s.
```





```math
\boxed{v_3(R_n)=v_3(n).}
```



## Exercice 15

Si $n$ est impair, $3^n\equiv3\pmod4$, donc $v_2(3^n-1)=1$ ; la condition impose $n=1$.

Si $n=2^sq$, avec $s\ge1$ et $q$ impair,



```math
3^n-1=(3^q-1)(3^q+1)\prod_{j=1}^{s-1}(3^{2^jq}+1).
```



Puisque $3^q\equiv3\pmod8$, les deux premiers facteurs ont pour valuations $1$ et $2$. Chacun des suivants vaut $2$ modulo $8$, donc a pour valuation $1$. Ainsi



```math
v_2(3^n-1)=s+2.
```



La divisibilité $2^n\mid3^n-1$ équivaut à $n\le s+2$. Pour $s\ge3$, $n\ge2^s>s+2$, impossible. Pour $s=1$, seul $n=2$ convient ; pour $s=2$, seul $n=4$ convient.



```math
\boxed{n\in\{1,2,4\}.}
```



## Exercice 16

$n=1,3$ conviennent. Soit $n>1$ solution. Il est impair, sinon $n^2$ serait pair alors que $2^n+1$ est impair. Soit $p$ le plus petit diviseur premier de $n$ et $d$ l’ordre de $2$ modulo $p$. Comme $2^n\equiv-1\pmod p$, $d=2s$, avec $s\mid n$, $s\mid p-1$ et $n/s$ impair. Tout facteur premier de $s$ diviserait $n$ et serait inférieur à $p$, donc $s=1$. Alors $p\mid 2+1$, d’où $p=3$. Écrivons $3^e\Vert n$. La démonstration de l’exercice 14, appliquée à $X=-2\equiv1\pmod3$, donne $v_3(2^n+1)=v_3((-2)^n-1)=1+v_3(n)=1+e$, puisque $n$ est impair. Puisque $n^2\mid2^n+1$, $2e\le1+e$, donc $e=1$. Si $q>3$ était le plus petit autre facteur premier de $n$, l’ordre de $2$ modulo $q$ serait $2s$, où $s\mid n$ et $s\mid q-1$. Tout facteur premier de $s$ serait inférieur à $q$ et diviserait $n$; il ne peut être que $3$, avec exposant au plus $1$. Ainsi $s=1$ ou $3$. Le premier cas impose $q\mid3$; le second, l’ordre étant $6$, impose $q\mid2^3+1=9$. Dans les deux cas $q\le3$, contradiction. Donc $n=3$.

## Exercice 17

Soit $B$ le bloc de $666$ chiffres $6$. Ses trois derniers chiffres donnent



```math
B\equiv666\equiv2\pmod8\implies v_2(B)=1,\qquad B\equiv1\pmod5\implies v_5(B)=0.
```



Pour $N=B10^r$, $r\ge0$,



```math
v_2(N)=r+1,\qquad v_5(N)=r.
```



Ces deux entiers consécutifs ne peuvent être tous deux pairs. Donc $N$ n'est jamais un carré.

## Exercice 18

Supposons $x<y$. Les logarithmes donnent $\log x/x=\log y/y$. Si $x\ge3$, la fonction $t\mapsto\log t/t$ décroît strictement pour $t\ge3$, impossible. Si $x=1$, l’équation impose $y=1$, contradiction. Il reste $x=2$, et l’équation devient $2^y=y^2$. Pour $y=3$, $2^3\ne3^2$ ; on vérifie $y=4$. Pour $y\ge4$, le quotient $2^y/y^2$ est strictement croissant car $2y^2/(y+1)^2>1$, donc cette solution est unique. Les solutions sont $x=y$ et $(2,4),(4,2)$.

## Exercice 19

Les assertions sont fausses avec l’initialisation imprimée $F_0=F_1=1$. Pour 1, $n=m=1$ donne $F_2=2$ alors que $F_1F_2+F_0F_1=3$. Pour 2, $n=m=2$ donne $F_2\wedge F_4=2\wedge5=1$, mais $F_2\wedge F_2=2$. Pour 3, $n=m=2$ et le reste $r=0$ donnent $F_2\wedge F_2=2$ mais $F_2\wedge F_0=1$. Pour 4, $n=2,m=4$ donnent $F_2\wedge F_4=1$ alors que $F_{2\wedge4}=F_2=2$. Les formules données sont celles de la suite standard commençant par $0,1$ et comportent un décalage d’indice par rapport à la suite définie ici.


Poser $G_0=0$ et $G_n=F_{n-1}$ pour $n\ge1$. Alors $G_0=0$, $G_1=1$, $G_{n+2}=G_{n+1}+G_n$.

### 1 — Formule corrigée

Pour $m=1$, $G_{n+1}=G_1G_{n+1}+G_0G_n$. Pour $m=2$, $G_{n+2}=G_{n+1}+G_n$. En additionnant les identités aux rangs $m$ et $m+1$, la récurrence donne celle au rang $m+2$. Ainsi



```math
G_{n+m}=G_mG_{n+1}+G_{m-1}G_n.
```



### 2 — PGCD



```math
\gcd(G_{n+1},G_n)=\gcd(G_n,G_{n-1})=\cdots=\gcd(1,0)=1.
```



Par la formule précédente et le lemme de Gauss,



```math
\gcd(G_n,G_{n+m})=\gcd(G_n,G_mG_{n+1})=\gcd(G_n,G_m).
```



### 3 — Division euclidienne

Si $m=qn+r$, itérer l'identité 2 donne



```math
\gcd(G_n,G_m)=\gcd(G_n,G_r).
```



### 4 — Formule finale

L'algorithme d'Euclide sur les indices conduit à $d=\gcd(n,m)$, puis



```math
\gcd(G_n,G_m)=\gcd(G_d,G_0)=G_d.
```



Pour la suite effectivement imprimée, on en déduit



```math
\boxed{\gcd(F_n,F_m)=F_{\gcd(n+1,m+1)-1}.}
```



## Exercice 20

1. $1\le\tau(n)\le n$ et $n\le p(n)\le n^{\tau(n)}$. 2. Les diviseurs se regroupent en paires $d,n/d$; un diviseur seul correspond exactement à $d=\sqrt n$. 3. Si $n=\prod p^{\alpha_p}$, alors $\tau(n)=\prod(\alpha_p+1)$. 4. Dans le produit des diviseurs, chaque premier apparaît avec exposant $\alpha_p\tau(n)/2$, donc $p(n)=n^{\tau(n)/2}$.

## Exercice 21

1. Les diviseurs donnent $1+2+3+6=12$ et $1+2+4+7+14+28=56$. 2. Pour une puissance première, $\sigma(p^a)=1+p+\cdots+p^a=(p^{a+1}-1)/(p-1)$. Si $n=\prod p^a$, les diviseurs se choisissent indépendamment pour chaque premier, donc $\sigma(n)=\prod_{p^a\parallel n}(1+p+\cdots+p^a)$. 3. Si $(m,n)=1$, tout diviseur de $mn$ s’écrit de façon unique $de$, $d\mid m,e\mid n$; en sommant, $\sigma(mn)=\sigma(m)\sigma(n)$. 4. Si $2^p-1$ est premier, il est premier avec $2^{p-1}$; la formule donne $\sigma(2^{p-1}(2^p-1))=(2^p-1)2^p=2n$. 5. Écrivons $n=2^ab$, $b$ impair. (a) La multiplicativité donne $\sigma(n)=(2^{a+1}-1)\sigma(b)$. (b) Posons $q=2^{a+1}-1$. De $2^{a+1}b=q\sigma(b)$ et $(q,2^{a+1})=1$, on déduit $q\mid b$; écrivons $b=qc$. L’égalité donne $\sigma(b)=2^{a+1}c$. (c) Alors la somme des diviseurs propres de $b$ vaut $\sigma(b)-b=c$. Comme $c\mid b$ et $c<b$, si $c>1$, les diviseurs propres distincts $1,c$ ont déjà une somme supérieure à $c$. Donc $c=1$; alors $\sigma(b)=b+1$, ce qui impose que $b$ soit premier. (d) La forme est $n=2^a(2^{a+1}-1)=2^{k-1}(2^k-1)$ avec $k=a+1$.

## Autocorrection D

Soit $q$ un diviseur premier de $n!+1$. Aucun premier $\le n$ ne divise ce nombre, donc $q>n$ et $q\le n!+1$. En faisant varier $n$, tout ensemble fini de nombres premiers serait contenu dans $[1,n]$ pour n assez grand, contradiction.

## Exercice 22

$p$ impair donne $p^2\equiv1\pmod8$; $3\nmid p$ donne $p^2\equiv1\pmod3$. Comme $8$ et $3$ sont premiers entre eux, $24\mid p^2-1$.

## Exercice 23

Soient $p<q$ deux nombres premiers consécutifs. Si $p=2$, leur somme $5$ n’est pas un produit de deux nombres premiers. Sinon ils sont impairs, donc $p+q=2r$ si cette somme était un produit de deux nombres premiers, avec $r$ premier. Or $p<r<q$, contradiction avec la consécutivité.

## Exercice 24

Les $n$ entiers $(n+1)!+2,\ldots,(n+1)!+(n+1)$ sont divisibles respectivement par $2,\ldots,n+1$; ils sont composés et consécutifs.

## Exercice 25

Une longueur paire finit par $10$, donc le nombre est divisible par $10$. Une longueur impaire s’écrit $N_m=1+10^2+\cdots+10^{2m-2}=(100^m-1)/99$, où $m$ est le nombre de chiffres $1$. Si $m$ est impair et $m>1$, alors $N_m=((10^m-1)/9)((10^m+1)/11)$; les deux facteurs sont entiers et strictement supérieurs à $1$. Si $m$ est pair et $m>2$, alors $N_m=N_{m/2}(100^{m/2}+1)$, deux facteurs strictement supérieurs à $1$. Les seuls candidats premiers sont donc $m=1$ (le nombre $1$, non premier) et $m=2$, qui donne $101$, premier.

## Exercice 26

1. Si les nombres premiers $3\pmod4$ étaient $p_1,\ldots,p_r$, $N=4p_1\cdots p_r-1$ est $3\pmod4$ et n’est divisible par aucun $p_i$. Ses facteurs premiers ne peuvent tous être $1\pmod4$, leur produit serait $1\pmod4$; un facteur $3\pmod4$ nouveau apparaît. 2. Supposer finis les premiers $5\pmod6$; choisir $N=6p_1\cdots p_r-1$, qui vaut $5\pmod6$. Aucun $p_i$ ne divise $N$. Ses facteurs premiers sont tous $1$ ou $5\pmod6$, et leur produit vaut $5\pmod6$, donc au moins un facteur $5\pmod6$ nouveau.

## Exercice 27

Pour $n=2$, $1!\equiv-1\pmod2$. Si $n=p$ est premier impair, les inverses modulo $p$ se groupent par paires $a,a^{-1}$, sauf $1$ et $-1$, d’où $(p-1)!\equiv-1\pmod p$. Réciproquement, si $n$ est composé et non carré, il possède un diviseur $d$ avec $1<d<n$ et $d\ne n/d$; les deux facteurs figurent dans $(n-1)!$, donc $n\mid(n-1)!$. Si $n=d^2$ avec $d>2$, les facteurs $d$ et $2d<n$ figurent dans $(n-1)!$ et leur produit est divisible par $n$. Le cas $n=4$ se vérifie: $3!\equiv2\not\equiv-1\pmod4$. Ainsi aucun composé ne satisfait la congruence.

## Exercice 28

1. Si $x^2\equiv-1\pmod p$, alors la classe de $x$ est d’ordre 4 dans $(\mathbb Z/p\mathbb Z)^\times$: son carré n’est pas 1, mais son quatrième pouvoir l’est. L’ordre divise $p-1$, donc $4\mid p-1$. 2. Supposons la liste des nombres premiers congrus à 1 modulo 4 finie, de produit $P$ (produit vide égal à 1). Un premier $q$ divisant $(2P)^2+1$ ne divise pas $2P$ et pour lui $(2P)^2\equiv-1\pmod q$; par 1, $q\equiv1\pmod4$. Il n’est aucun des premiers de la liste, contradiction. 3. Le théorème de Wilson donne $(p-1)!\equiv-1\pmod p$. En groupant les facteurs $k$ et $p-k$, $1\le k\le(p-1)/2$, on obtient $(p-1)!\equiv(-1)^{(p-1)/2}(((p-1)/2)!)^2\pmod p$. Avec Wilson, on en déduit $(((p-1)/2)!)^2\equiv(-1)^{(p+1)/2}\pmod p$, qui vaut $-1$ si $p\equiv1\pmod4$.

## Exercice 29

Si $n$ est pair, $n^4+4^n$ est divisible par $16$ et strictement supérieur à $16$, donc composé. Si $n>1$ est impair, posons $y=2^{(n-1)/2}$. L’identité de Sophie Germain donne $n^4+4^n=n^4+4y^4=(n^2-2ny+2y^2)(n^2+2ny+2y^2)$. Le premier facteur vaut $(n-y)^2+y^2\ge y^2\ge4$ ; le second est encore plus grand. Les deux facteurs sont donc strictement supérieurs à $1$.

## Exercice 30

1. $a^n-1=(a-1)(1+a+\cdots+a^{n-1})$. 2. Si $a>2$, le facteur $a-1$ est non trivial; si $n$ composé, $a^n-1=(a^{n/d}-1)(\cdots)$ est composé. 3. $a=bq+r$ donne $2^a-1=(2^b)^q2^r-1\equiv2^r-1\pmod{2^b-1}$. Comme $0\le r<b$, on a $0\le2^r-1<2^b-1$ : il s’agit bien du reste euclidien. 4. L’algorithme d’Euclide appliqué à $2^a-1,2^b-1$ reproduit celui sur les exposants, donc le PGCD vaut $2^{(a,b)}-1$.

## Exercice 31

1. Si $m$ a un diviseur impair $d>1$, $2^m+1$ est divisible par $2^{m/d}+1$; donc $m$ est une puissance de $2$. 2. $F_0=3,F_1=5,F_2=17,F_3=257,F_4=65537$. 3. $F_{n+1}-2=2^{2^{n+1}}-1=(2^{2^{n}}-1)(2^{2^{n}}+1)=(F_n-2)F_n$. 4. $F_n=2+\prod_{k=0}^{n-1}F_k=2+3\prod_{k=1}^{n-1}F_k$, avec produit vide égal à 1. 5. Pour $m>n$, la relation précédente donne $F_m\equiv2\pmod{F_n}$; comme $F_n$ est impair, le PGCD divise $2$ et vaut $1$. 6. Les $F_n$ sont deux à deux premiers entre eux et supérieurs à $1$, donc donnent une infinité de facteurs premiers.

## Autocorrection E

Par le théorème chinois, les idempotents correspondant à $2,3,5,7$ modulo $210$ sont $105,70,126,120$. Ainsi $n=105a+70b+126c+120d$ convient.

## Autocorrection F

Modulo 13, $2^{12}=3^{12}=1$, donc $2^{70}+3^{70}\equiv2^{10}+3^{10}\equiv10+3=13\equiv0\pmod{13}$.

## Exercice 32

Écrire $a=b+kn$; le binôme donne $a^n-b^n=\sum_{j=1}^n\binom nj b^{n-j}(kn)^j$. Le terme $j=1$ est $n^2kb^{n-1}$; tous les autres contiennent $n^2$ aussi.

## Exercice 33



```math
82\,589\,933\equiv1\pmod4,\qquad2^{82\,589\,933}\equiv2\pmod{10}.
```





```math
\boxed{2^{82\,589\,933}-1\equiv1\pmod{10}.}
```



Le dernier chiffre est $\boxed1$.

## Exercice 34

(i) $(x,y)=(3+5t,-4-7t)$, $t\in\mathbb Z$. (ii) Aucune solution, car $3\nmid1$. (iii) $x-2y=3$, donc $(x,y)=(3+2t,t)$. (iv) $(x,y)=(2+3t,-2-5t)$, $t\in\mathbb Z$.

## Exercice 35

Une solution particulière est $(2,0,0)$. Pour le système homogène, la congruence modulo $3$ impose $y\equiv z\pmod3$; posons $y=t+3u$, $z=t$. Alors $x=-3t-4u$. Toutes les solutions sont $(x,y,z)=(2-3t-4u,t+3u,t)$, $t,u\in\mathbb Z$.

## Exercice 36

(i) $5^{-1}\equiv3\pmod7$, donc $x\equiv3\pmod7$. (ii) $3^{-1}\equiv13\pmod{19}$, donc $x\equiv52\equiv14\pmod{19}$. (iii) $23$ est inversible modulo $97$, donc $x\equiv0\pmod{97}$. (iv) $8^{-1}\equiv92\pmod{105}$, donc $x\equiv7\cdot92\equiv14\pmod{105}$. (v) En divisant par $4$, $x\equiv2\pmod3$. (vi) Il n’y a pas de solution, car $\gcd(4,12)=4$ ne divise pas $6$.

## Exercice 37

La première congruence donne $y\equiv6-4x\pmod{12}$. En la remplaçant dans la seconde, on obtient $15x\equiv21\pmod{12}$, soit $x\equiv3\pmod4$. Les solutions sont donc $(x,y)=(3+4t,6-4(3+4t)+12s)$, avec $s,t\in\mathbb Z$.

## Exercice 38

1. Pour $p$ impair, $4(x^2+x+3)=(2x+1)^2+11$. Comme $2$ est inversible modulo $p$, les deux équations sont équivalentes. 2. (a) Modulo 2, $x^2+x+3\equiv1$, donc aucune solution. Modulo 3, l’équation est $x(x+1)\equiv0$, donc $x\equiv0,2$. (b) Le discriminant impose $y^2\equiv-11$: modulo 5, $y\equiv\pm2$, donnant $x\equiv1,3$; modulo 7, $3$ n’est pas un carré, donc aucune solution; modulo 11, $y\equiv0$ et $x\equiv5$. (c) Par le théorème chinois, modulo 10 il n’y a aucune solution; modulo 15 les solutions sont $3,6,8,11$; modulo 55 elles sont $16,38$; modulo 105 aucune. (d) Modulo 121, une solution imposerait $2x+1=11t$, dont le carré est divisible par 121, alors qu’il devrait être congru à $-11$, impossible. Modulo 25 les racines sont $8,16$; modulo 125 elles sont $33,91$. (e) Les deux racines modulo 5 sont $1,3$, et $f'(x)=2x+1$ vaut respectivement $3,2$, non nuls modulo 5. Si $r$ est une racine modulo $5^j$, ses relèvements sont $r+t5^j$, $0\le t<5$; $f(r+t5^j)\equiv f(r)+t5^jf'(r)\pmod{5^{j+1}}$. Il existe un unique $t$ donnant zéro modulo $5^{j+1}$. Chaque racine se relève donc de façon unique à chaque étape; il y a exactement deux racines modulo $5^k$.

## Exercice 39

Modulo 5, il faut $n\equiv\pm1$; modulo 13, il faut $n\equiv\pm4$. Le théorème chinois donne les quatre classes modulo 65: $n\equiv4,9,56,61\pmod{65}$ (substitution directe). Chacune contient une infinité d’entiers positifs.

## Exercice 40

Modulo $5$, $2^n\equiv3$ équivaut à $n\equiv3\pmod4$; modulo $13$, l’ordre de $2$ est $12$ et $3=2^4$, donc $n\equiv4\pmod{12}$. Chacune des congruences a une infinité de solutions, mais elles sont incompatibles modulo $4$; aucun terme n’est multiple de $65$.

## Exercice 41

La valeur $11$ est atteinte pour $(n,m)=(1,2)$. Montrons qu’aucune valeur absolue $<11$ ne convient. Posons $D=36^n-5^m$. Modulo 5, $D\equiv1$, donc $|D|\equiv1$ ou $4\pmod5$. Modulo 4, $D\equiv-1\equiv3$; si $D>0$, les seuls entiers $1\le D<11$ congrus à 3 modulo 4 sont 3 et 7, qui ne sont pas congrus à 1 modulo 5. Si $D<0$, alors $|D|\equiv1\pmod4$ et $4\pmod5$, donc le seul candidat inférieur à 11 est 9. Mais modulo 3, $|D|\equiv5^m\equiv\pm1$, contradiction avec $9\equiv0$. Ainsi la borne inférieure est 11.

## Exercice 42

La période de $3^n$ modulo 7 est 6. Pour $r=n\pmod6$, la condition devient $n\equiv(3^r)^{-1}\pmod7$. Le tableau des solutions, dans l’ordre $r=0,1,2,3,4,5$, est $n\equiv36,19,16,27,32,17\pmod{42}$. Les solutions sont donc $n\equiv16,17,19,27,32,36\pmod{42}$.

## Exercice 43

Pour $p=2$, $n=2$ convient. Supposons $p$ impair. Écrivons $n=r+k(p-1)$, où $0\le r<p-1$. Alors $2^n\equiv2^r\pmod p$ et $n\equiv r-k\pmod p$. Choisissons $k$ parmi $0,\ldots,p-1$ tel que $k\equiv r-2^r\pmod p$. On a alors $2^n\equiv n\pmod p$.

## Exercice 44

1. Pour $1\le k<p$, $\binom pk=\dfrac{p(p-1)\cdots(p-k+1)}{k!}$ a un numérateur divisible par $p$ et un dénominateur premier à $p$; donc $p\mid\binom pk$. 2. Par le binôme, $(a+1)^p\equiv a^p+1\pmod p$. Une récurrence de $a=0$ à tous les entiers positifs donne $a^p\equiv a$; pour $a<0$ et $p$ impair, $a^p-a=-((-a)^p-(-a))$ est divisible par $p$. Pour $p=2$, la congruence se vérifie directement selon la parité de $a$.

## Exercice 45

L’exposant est $2^{6k+2}$. Comme $2^6=64\equiv10\pmod{18}$ et $10^k\equiv1$ ou $10\pmod{18}$, on a $2^{6k+2}\equiv4\pmod{18}$. L’ordre de $2$ modulo $19$ est $18$, donc $2^{2^{6k+2}}+3\equiv2^4+3=19\equiv0\pmod{19}$.

## Exercice 46

Ni 2 ni 5 ne divise un repunit, car un repunit ne finit ni par un chiffre pair ni par 0 ou 5. Le premier 3 divise $111$. Pour tout premier $p\ne2,3,5$, $10$ est inversible modulo $p$; deux de ses puissances coïncident dans le groupe fini $(\mathbb Z/p\mathbb Z)^\times$, donc $10^r\equiv1\pmod p$ pour un $r>0$. Comme $p\ne3$, on en déduit $p\mid(10^r-1)/9$, un repunit. Les premiers cherchés sont exactement ceux différents de 2 et 5.

## Exercice 47

1. Les cubes modulo $9$ sont $0,1,-1$; l’équation est résoluble exactement pour $n\equiv0,1,-1\pmod9$. 2. Une somme de trois éléments de $\{0,1,-1\}$ modulo $9$ ne vaut que $0,\pm1,\pm2,3,-3$; or $11111\equiv5\pmod9$. 3. Modulo $9$, l’équation donnerait $x^3\equiv5$, impossible puisque les cubes valent $0,\pm1$.

## Exercice 48

Si $x$ est impair, $3^x\equiv3\pmod8$, donc $y^2\equiv3\pmod8$, impossible. Ainsi $x$ est pair; l’équation modulo 8 donne alors $y^2\equiv1$, donc $y$ est impair. Écrivons $x=2r$. Alors $(3^r-y)(3^r+y)=8$. Les deux facteurs sont positifs et pairs, donc ils valent 2 et 4. Il vient $3^r=3$, $y=1$, soit $(x,y)=(2,1)$, qui convient.

## Exercice 49

Soit $d$ le chiffre absent. La somme des neuf chiffres présents vaut $45-d$. Or



```math
2^{29}\equiv2^5\equiv5\pmod9\implies45-d\equiv5\pmod9\implies d\equiv4\pmod9.
```



Comme $0\le d\le9$, $\boxed{d=4}$.

## Exercice 50

### 1 — Termes congrus à $2$ modulo $3$

Un carré est congru à $0$ ou $1$ modulo $3$. Si $a_j\equiv2\pmod3$, aucun terme ultérieur n'est un carré et



```math
a_{j+k}=a_j+3k.
```



Aucune valeur ne se répète une infinité de fois.

### 2 — Multiples de $3$

Les opérations conservent la divisibilité par $3$. Pour un terme $a\ge6$ multiple de $3$, le carré $(a-3)^2$ est congru à $a$ modulo $3$ et



```math
(a-3)^2\ge a.
```



En ajoutant successivement $3$, on rencontre donc un premier carré $r^2$ avec $a\le r^2\le(a-3)^2$. Après l'extraction de la racine,



```math
3\mid r,\qquad0<r\le a-3<a.
```



Les valeurs obtenues après les opérations racine décroissent donc jusqu'à $3$, puis



```math
3\longmapsto6\longmapsto9\longmapsto3.
```



### 3 — Termes congrus à $1$ modulo $3$

$a=1$ est fixe. Pour $a>1$, donc $a\ge4$, le carré $(a-2)^2$ est congru à $a$ modulo $3$ et $(a-2)^2\ge a$. Le prochain carré rencontré a donc une racine $r$ satisfaisant



```math
2\le r\le a-2<a,\qquad r\equiv1\text{ ou }2\pmod3.
```



Tant que ces racines sont congrues à $1$, elles décroissent strictement et restent $\ge2$ ; cela ne peut continuer indéfiniment. Une racine finit donc congrue à $2$ modulo $3$, puis le cas 1 s'applique.



```math
\boxed{a_0=1\quad\text{ou}\quad3\mid a_0.}
```



Si l'on autorise $a_0=0$ dans la dernière question, la règle imprimée donne $0\mapsto3$ : il convient aussi et appartient déjà à la seconde famille.

## Exercice 51

Si $n$ est impair, les termes $k^n$ et $(n-k)^n$ s’annulent modulo $n$; le terme $n^n$ est nul. Donc $n\mid\sum_{k=1}^n k^n$. Si $n$ est pair et $2^a\Vert n$, alors $n\ge2^a$. Pour tout $k$ impair, $k^{2^{a-1}}\equiv1\pmod{2^a}$, donc $k^n\equiv1\pmod{2^a}$; pour $k$ pair, $k^n\equiv0\pmod{2^a}$. Il y a $n/2=2^{a-1}(n/2^a)$ termes impairs, et $n/2^a$ est impair: ainsi la somme vaut $2^{a-1}\pmod{2^a}$, donc n’est pas divisible par $n$.

## Exercice 52

Poser $T_1=a$, $T_{j+1}=a^{T_j}$. Comme $a\ge2$ et $2^t>t$ pour $t\ge1$, la suite $T$ est strictement croissante et tend vers $+\infty$.

Montrer par récurrence forte sur $m\ge1$ que $T$ est stationnaire modulo $m$. Le cas $m=1$ est immédiat. Pour $m>1$, écrire



```math
m=uv,\qquad u=\prod_{\substack{p^e\parallel m\\p\mid a}}p^e,\qquad\gcd(v,a)=\gcd(u,v)=1.
```



Si $p^e\mid u$, alors



```math
v_p(T_j)=T_{j-1}v_p(a)\longrightarrow+\infty.
```



Ainsi $T_j\equiv0\pmod u$ à partir d'un rang.

Si $v>1$, le théorème d'Euler donne $a^{\varphi(v)}\equiv1\pmod v$. Comme $\varphi(v)<v\le m$, la récurrence assure que $T_j$ est stationnaire modulo $\varphi(v)$. Par conséquent $T_{j+1}=a^{T_j}$ est stationnaire modulo $v$. Si $v=1$, cette conclusion est immédiate.

Le théorème chinois conclut que $T_j$ est stationnaire modulo $m$, donc modulo $b$.

## Exercice 53

Pour $1\le k<p/2$, le développement de l’inverse donne $(p-k)^\dagger\equiv-k^\dagger-p(k^\dagger)^2\pmod{p^2}$. En sommant ces paires, la somme cherchée vaut $-p\sum_{k=1}^{(p-1)/2}(k^\dagger)^2\pmod{p^2}$. Modulo $p$, les inverses permutent les éléments non nuls; de plus $(p-k)^{-2}\equiv k^{-2}$, donc deux fois cette somme partielle vaut $\sum_{k=1}^{p-1}k^{-2}\equiv0\pmod p$. La dernière somme vaut $\sum k^2=p(p-1)(2p-1)/6\equiv0\pmod p$ pour $p\ge5$. La somme initiale est donc nulle modulo $p^2$.

## Exercice 54

Écrivons $x=a/b$ en fraction irréductible. Multiplier l’équation par $b^n$ donne $a^n+b(a_{n-1}a^{n-1}+a_{n-2}a^{n-2}b+\cdots+a_0b^{n-1})=0$. Donc $b\mid a^n$; $(a,b)=1$ impose $b=1$.

## Exercice 55

Les racines de l’unité communes vérifient $z^n=z^m=1$, donc $z^{(n,m)}=1$ par Bézout. Réciproquement toute racine d’ordre divisant $(n,m)$ est commune; $U_n\cap U_m=U_{(n,m)}$.

## Exercice 56

Un morphisme est déterminé par l’image de $1$, un élément $y\in\mathbb Z/m\mathbb Z$ tel que $ny=0$. Poser $d=\gcd(n,m)$, $n=dn_0$, $m=dm_0$, avec $\gcd(n_0,m_0)=1$. Alors $m\mid ny\iff m_0\mid y$. Les possibilités sont $y=0,m_0,\ldots,(d-1)m_0$ modulo $m$ : il y a donc $\boxed{d=\gcd(n,m)}$ morphismes.

## Exercice 57

Supposons $\varphi\ne0$ et soit $d>0$ le générateur de son image $d\mathbb Z$. Pour chaque $j$, soit $G_j$ le sous-groupe des suites dont les $j$ premières coordonnées sont nulles. Toute suite diffère de sa queue par une suite à support fini; ainsi $\varphi(G_j)=d\mathbb Z$. Choisissons $x_j\in G_j$ avec $\varphi(x_j)=d$. La somme $y=\sum_{j\ge1}j!x_j$ est définie coordonnée par coordonnée, car pour une coordonnée fixée seuls un nombre fini de $x_j$ sont non nuls. Pour tout $N$, sa queue $\sum_{j>N}j!x_j$ est coordonnée par coordonnée divisible par $(N+1)!$, donc $\varphi(y)\equiv d\sum_{j=1}^N j!\pmod{(N+1)!}$. Pour $N\ge2$, $\sum_{j=1}^N j!\le2N!$, donc $d\sum_{j=1}^N j!/(N+1)!\le2d/(N+1)\to0$. Pour $N$ assez grand, les deux membres ont des représentants de valeur absolue strictement inférieure à $(N+1)!/2$; cette congruence force alors $\varphi(y)=d\sum_{j=1}^N j!$. Le membre de droite tend vers l’infini avec $N$, alors que le membre de gauche est fixe: contradiction. Donc $\varphi=0$.

## Exercice 58

L’addition est point par point. La convolution est commutative et associative en réindexant les sommes finies sur les diviseurs (l’associativité correspond aux factorisations $n=abc$); la distributivité est terme à terme. L’unité est $\delta_1$, valant 1 en 1 et 0 ailleurs. Une fonction $f$ est inversible si et seulement si $f(1)\ne0$: si $f*g=\delta_1$, alors $f(1)g(1)=1$; réciproquement, lorsque $f(1)\ne0$, on pose $g(1)=1/f(1)$, puis, pour $n>1$, $g(n)=-\frac1{f(1)}\sum_{d\mid n,\ d>1}f(d)g(n/d)$. Les arguments $n/d<n$ assurent que cette récurrence définit bien $g$, et la formule donne $f*g=\delta_1$. Pour $n=\prod p_i^{e_i}$, $\sum_{d\mid n}\mu(d)=\prod_i(1-1)$ vaut 0 si $n>1$ et vaut 1 si $n=1$; donc $\mu*1=\delta_1$. Enfin $\varphi*1=\mathrm{id}$, car $\sum_{d\mid n}\varphi(d)=n$ (partitionner $1,\ldots,n$ selon le PGCD avec $n$). Convoluer par $\mu$ donne $\varphi=\mathrm{id}*\mu$, soit $\varphi(n)=\sum_{d\mid n}d\mu(n/d)$.

## Exercice 59

1. Si $a/b,c/d\in A$, leurs dénominateurs $b,d$ sont premiers à $p$; les dénominateurs $bd$ de leur somme et de leur produit le sont aussi. Ainsi $A$ est un sous-anneau de $\mathbb Q$, donc intègre. 2. La fraction $a/b$ est inversible dans $A$ exactement lorsque $p\nmid a$: alors son inverse $b/a$ appartient à $A$; si $p\mid a$, son inverse aurait un dénominateur divisible par $p$. 3. Le morphisme unitaire $\varphi:A\to\mathbb F_p$ doit envoyer $a/b$ sur $\bar a\bar b^{-1}$, ce qui définit bien un morphisme surjectif et prouve son unicité. Son noyau est l’ensemble des $a/b$ avec $p\mid a$, exactement les non-inversibles; ainsi $A^\times=A\setminus\ker\varphi$.

## Exercice 60

1. (a) Pour $\ell=0$, la congruence est une égalité. Si elle est vraie au rang $\ell-1$, on élève à la puissance $p$: les termes binomiaux d’ordre au moins 2 sont divisibles par $p^{\ell+2}$, et l’on obtient $(1+p)^{p^\ell}\equiv1+p^{\ell+1}\pmod{p^{\ell+2}}$ (pour $\ell=1$, le terme d’ordre 2 contient aussi $p$ dans $\binom p2$). (b) On a $(1+p)^{p^{k-1}}\equiv1\pmod{p^k}$ et, pour $k\ge2$, $(1+p)^{p^{k-2}}\equiv1+p^{k-1}\not\equiv1\pmod{p^k}$; l’ordre est donc $p^{k-1}$. Pour $k=1$, l’ordre vaut 1. (c) Le groupe des unités modulo $p^k$ a ordre $p^{k-1}(p-1)$. Si $g$ relève un générateur modulo $p$, son ordre modulo $p^k$ est $(p-1)p^s$ pour un $s\le k-1$; alors $g^{p^s}$ a ordre $p-1$. Son produit avec $1+p$, d’ordre premier à $p-1$, a ordre $p^{k-1}(p-1)$; le groupe est cyclique. 2. Pour $k\ge3$, tout carré impair est congru à 1 modulo 8; il n’y a que $2^{k-3}$ classes modulo $2^k$ congrues à 1 modulo 8. Or, dans un groupe cyclique d’ordre $2^{k-1}$, les carrés formeraient un sous-groupe de taille $2^{k-2}$. Le groupe des unités modulo $2^k$ n’est donc pas cyclique.
