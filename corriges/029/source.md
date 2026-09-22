# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td29-familles-sommables.pdf)

## Autocorrection A

1. En regroupant selon $N=n+m$,


```math
\sum_{n,m\geq0}\frac{2^n3^m}{(n+m)!}=\sum_{N\geq0}\frac1{N!}\sum_{n=0}^N2^n3^{N-n}=\sum_{N\geq0}\frac{3^{N+1}-2^{N+1}}{N!}=3e^3-2e^2.
```


2. Pour $m=n+1$, $|n^2-m^2|^{-1}=1/(2n+1)$; la somme diverge.
3. Sur la diagonale $n+m=N$, la somme vaut $(N-1)/N^3=O(N^{-2})$; la famille est sommable.
4. L'intervalle $[1,2]\cap\mathbb Q$ contient une infinité de termes supérieurs à $1/4$; pas de sommabilité.

## Autocorrection B

Si $\alpha\leq0$, les termes ne tendent pas vers zéro. Si $\alpha>0$,


```math
\sum_{p\geq2}n^{-\alpha p}=\frac{n^{-2\alpha}}{1-n^{-\alpha}}\asymp n^{-2\alpha}.
```


La série en $n$ converge exactement si $2\alpha>1$. Condition : $\alpha>1/2$.

## Autocorrection C

Posons $a_{ij}=\operatorname{sgn}(i-j)2^{-|i-j|}$, avec $\operatorname{sgn}(0)=0$.
1. À $j$ fixé,


```math
\sum_{i\geq0}a_{ij}=-\sum_{d=1}^j2^{-d}+\sum_{d=1}^{\infty}2^{-d}=2^{-j}.
```


La somme sur $j$ vaut $2$. En sommant d'abord en $j$,


```math
\sum_{j\geq0}a_{ij}=\sum_{d=1}^i2^{-d}-\sum_{d=1}^{\infty}2^{-d}=-2^{-i},
```


et la somme sur $i$ vaut $-2$.
2. Ces deux sommes itérées diffèrent, donc la famille n'est pas sommable.
3. Pour tout $d\geq1$, une infinité de couples ont $|i-j|=d$ et $|a_{ij}|=2^{-d}>0$; la somme des valeurs absolues diverge.

## 1

Pour $r=\max(p,q)$, la couronne contient $2r-1$ couples et $r^\alpha\leq p^\alpha+q^\alpha\leq2r^\alpha$ si $\alpha>0$. Sa somme est donc comparable à $r^{1-\alpha}$ : la somme sur les couronnes converge ssi $\alpha>2$. Si $\alpha\leq0$, les termes ne tendent pas vers zéro.

## 2

Posons $S_n=\sum_{k=1}^nu_k$. L'hypothèse donne $S_{2n}\leq(1+1/n)S_n$. Ainsi


```math
S_{2^r}\leq S_1\prod_{j=0}^{r-1}(1+2^{-j}),
```


produit borné. Les sommes partielles croissent et sont bornées le long de $2^r$, donc $\sum_nu_n$ converge.

## 3

Il y a $8\cdot9^{r-1}$ entiers de $E$ à $r$ chiffres. Chacun est au moins $10^{r-1}$; par conséquent


```math
\sum_{n\in E}\frac1n\leq1+\sum_{r\geq1}\frac{8\cdot9^{r-1}}{10^{r-1}}<+\infty.
```



## Autocorrection D

Pour $p\geq1$, posons $b_p=p\sum_{n\geq p}a_n/[n(n+1)]$ ; le terme d'indice $0$ est pris égal à $0$. Par positivité,


```math
\sum_{p\geq1}b_p=\sum_{n\geq1}\frac{a_n}{n(n+1)}\sum_{p=1}^np
=\frac12\sum_{n\geq1}a_n<+\infty.
```



## Autocorrection E

1. Pour $|z|<1$, la somme absolue est $\sum_{p,q\geq0}|z|^{2p+3q}=((1-|z|^2)(1-|z|^3))^{-1}$. Ainsi


```math
S(z)=\sum_{p,q\geq0}z^{2p+3q}=\frac1{(1-z^2)(1-z^3)}.
```


Pour $|z|=1$, chaque terme a module $1$ : la famille n'est pas sommable. (La mention $|z|\leq1$ dans l'énoncé ne permet donc la sommabilité que pour $|z|<1$.)
2. En regroupant par puissance,


```math
S(z)=\sum_{n\geq0}d_nz^n,\qquad d_n=\#\{(p,q)\in\mathbb N^2:2p+3q=n\}.
```


Il s'agit du nombre de représentations de $n$ comme somme de $p$ pièces de valeur $2$ et $q$ pièces de valeur $3$.

## 4

Par Tonelli,


```math
\sum_{m=1}^{\infty}\sum_{n=m}^{\infty}\frac1{n^{p+1}}
=\sum_{n=1}^{\infty}\frac n{n^{p+1}}=\zeta(p).
```



## 5

Pour $n\geq k$, $n(n-1)\cdots(n-k+1)/n!=1/(n-k)!$, donc la somme vaut $e$ (y compris $k=0$). Or


```math
n^4=n(n-1)(n-2)(n-3)+6n(n-1)(n-2)+7n(n-1)+n.
```


Après division par $n!$ et sommation, $\sum_{n\geq0}n^4/n!=(1+6+7+1)e=15e$.

## 6

Les développements ci-dessous sont absolument convergents pour $|x|<1$, ce qui autorise le regroupement.
1. En développant le membre de gauche, le coefficient de $x^N$ est le nombre $d(N)$ de diviseurs positifs de $N$. Dans le premier terme de droite, $(x^n-x^{n^2})/(1-x^n)=\sum_{k=1}^{n-1}x^{nk}$ compte les diviseurs strictement supérieurs à $\sqrt N$; ils sont en bijection avec ceux strictement inférieurs à $\sqrt N$. Si $N$ est carré, le terme $x^{n^2}$ fournit le diviseur central. Les coefficients coïncident :


```math
\sum_{n\geq1}\frac{x^n}{1-x^n}=2\sum_{n\geq1}\frac{x^n-x^{n^2}}{1-x^n}+\sum_{n\geq1}x^{n^2}.
```


2. Les deux côtés comptent les diviseurs impairs de chaque exposant :


```math
\sum_{n\geq1}\frac{x^{2n-1}}{1-x^{2n-1}}=\sum_{i\geq1}\frac{x^i}{1-x^{2i}}.
```


3. Le coefficient de $x^N$ à gauche est $\sum_{i\mid N}i$; à droite il vaut $\sum_{d\mid N}N/d$, même quantité :


```math
\sum_{i,k\geq1}i x^{ik}=\sum_{n\geq1}\frac{nx^n}{1-x^n}.
```


Dans les trois égalités, les coefficients sont respectivement $d(N)$, le nombre de diviseurs impairs de $N$, et $\sigma(N)=\sum_{d\mid N}d$.

## 7

Notons $A=\sum_{n\geq1}H_n/n^2$ et $B=\sum_{n\geq1}H_n/(n+1)^2$. Les sommes convergent, par comparaison à $\sum (1+\ln n)/n^2$. D'abord, en sommant en $m$,


```math
\sum_{n,m\geq1}\frac1{nm(n+m)}=\sum_{n\geq1}\frac1n\sum_{m\geq1}\frac1{m(n+m)}=\sum_{n\geq1}\frac{H_n}{n^2}=A,
```


car $1/[m(n+m)]=(1/m-1/(m+n))/n$. En groupant plutôt par $r=n+m$,


```math
A=\sum_{r\geq2}\frac{2H_{r-1}}{r^2}=2B.
```


Enfin $A-B=\sum_{n\geq1}(H_n-H_{n-1})/n^2=\zeta(3)$. Donc $B=\zeta(3)$ et $A=2\zeta(3)$; la double somme vaut aussi $2\zeta(3)$.

## 8

Tout couple s'écrit $(p,q)=d(a,b)$ avec $\gcd(a,b)=1$. Donc


```math
\zeta(2)^2=\sum_{d\geq1}d^{-4}\sum_{\substack{a,b\geq1\\(a,b)=1}}a^{-2}b^{-2}.
```


La somme cherchée vaut $\zeta(2)^2/\zeta(4)=5/2$.

## 9

Par $1/(2^n-1)=\sum_{k\geq1}2^{-nk}$, puis $\sum_{d\mid m}\varphi(d)=m$,


```math
\sum_{n\geq1}\frac{\varphi(n)}{2^n-1}=\sum_{m\geq1}\frac{\sum_{n\mid m}\varphi(n)}{2^m}=\sum_{m\geq1}\frac m{2^m}=2.
```



## 10

Chaque $n\in P$ s'écrit de façon unique $n=a^k$, où $a$ n'est pas une puissance parfaite et $k\geq2$. Pour un tel $a$,


```math
\sum_{k\geq1}\frac1{a^k(a^k-1)}=\sum_{k\geq1}\left(\frac1{a^k-1}-\frac1{a^k}\right)=\sum_{k\geq2}\frac1{a^k-1},
```


car $\sum_{k\geq1}a^{-k}=1/(a-1)$. Les écritures uniques $n=a^k$ pour tous les $a$ non-puissances parfaites et $k\geq1$ parcourent exactement les entiers $n\geq2$. Ainsi


```math
\sum_{n\in P}\frac1{n-1}=\sum_{a\text{ non-puissance parfaite}}\sum_{k\geq2}\frac1{a^k-1}=\sum_{n\geq2}\frac1{n(n-1)}=1.
```



## 11

Écrivons $b(n)=\sum_{k\geq0}\mathbf1_{\text{bit }k\text{ de }n=1}$. Pour un $k$ fixé, les blocs où ce bit vaut $1$ sont $[(2j+1)2^k,(2j+2)2^k-1]$. Comme $1/(n(n+1))=1/n-1/(n+1)$, la contribution d'un bloc vaut $2^{-k}/((2j+1)(2j+2))$. Or


```math
\sum_{j\geq0}\frac1{(2j+1)(2j+2)}=\ln2.
```


En sommant sur $k$, la réponse est $\sum_{k\geq0}2^{-k}\ln2=2\ln2$.

## 12

1. Comme $\Im z>0$, $az+b=0$ avec $a,b\in\mathbb R$ entraîne $a=b=0$. Sur le compact $\max(|a|,|b|)=1$, la fonction $|az+b|$ a un minimum $c_z>0$ et un maximum $C_z<\infty$. Par homogénéité, pour $k\geq0$, $|az+b|^{-k}\leq c_z^{-k}/\max(|a|,|b|)^k$; pour $k<0$, $|az+b|^{-k}\leq C_z^{-k}\max(|a|,|b|)^{-k}$. On peut donc prendre l'entier $A_z=\lceil\max(c_z^{-k},C_z^{-k})\rceil$.
2. Sur la couronne $\max(|m|,|n|)=r$, il y a $8r$ couples. Pour $k\geq3$, la borne $C_{z,k}r^{-k}$ donne $\sum_r8C_{z,k}r^{1-k}<\infty$.
3. La famille est absolument sommable; $(m,n)\mapsto(-m,-n)$ change le signe si $k$ est impair, donc $G_k(z)=0$.
4. Pour $z=iy$, les termes $(m,0)$ donnent $2\zeta(k)$. Pour $n\ne0$, chaque terme tend vers zéro lorsque $y\to\infty$; pour $y\geq1$ il est dominé par $(m^2+n^2)^{-k/2}$, sommable pour $k>2$. Donc $G_k(iy)\to2\zeta(k)$.

## 13

La semi-convergence implique que les sommes des termes positifs et des opposés des termes négatifs valent $+\infty$, et que $u_n\to0$. Construire l'ordre par blocs : ajouter les positifs inutilisés, dans l'ordre de leurs indices, jusqu'à dépasser $S$, puis les négatifs inutilisés dans le même ordre jusqu'à passer sous $S$, et répéter. À chaque dépassement, l'écart à $S$ est au plus le module du dernier terme ajouté, donc tend vers $0$. À l'intérieur d'un bloc, les sommes partielles sont comprises entre ses deux extrémités ; elles convergent donc aussi vers $S$. Insérer également les termes nuls, un par étape, s'il y en a; chaque indice est alors utilisé une fois et la réorganisation est une bijection.

## 14

Tel qu’il est écrit, l’énoncé est faux. Posons $u_0(n)=(-1)^n/(n+1)$, $u_1(n)=-u_0(n)$ et $u_k(n)=0$ pour $k\geq2$. Toutes les séries $\sum_nu_k(n)$ convergent, mais une majorante éventuelle $v$ doit vérifier $v(n)\geq |u_0(n)|=1/(n+1)$ : en effet, pour chaque $n$, l’un de $u_0(n),u_1(n)$ vaut $1/(n+1)$. Ainsi $\sum_nv(n)$ diverge.

Avec l’hypothèse supplémentaire $u_k(n)\geq0$, le résultat est vrai. Choisissons des entiers croissants $N_j$ tels que


```math
\sum_{n\geq N_j}\sum_{k=0}^j u_k(n)\leq2^{-j}.
```


Posons $v(n)=0$ pour $n<N_0$, et $v(n)=\sum_{k=0}^j u_k(n)$ si $N_j\leq n<N_{j+1}$. Pour chaque $k$, dès $n\geq N_k$, $v(n)\geq u_k(n)$. De plus,


```math
\sum_nv(n)\leq\sum_{j\geq0}\sum_{n=N_j}^{N_{j+1}-1}\sum_{k=0}^j u_k(n)\leq\sum_{j\geq0}2^{-j}<\infty.
```



## 15

1. Par factorisation unique et produits géométriques,


```math
\prod_{j=1}^r(1-p_j^{-s})^{-1}=\sum_{n\in E_r}n^{-s}.
```


2. Les ensembles $E_r$ croissent et leur réunion est $\mathbb N^*$. Pour $s>1$, convergence de $\sum n^{-s}$ et convergence monotone donnent la limite $\zeta(s)$.
3. Si $\sum_p1/p$ converge, $\prod_p(1-1/p)^{-1}$ converge puisque $-\ln(1-1/p)\sim1/p$. Or les produits partiels majorent $\sum_{n\leq N}1/n$ dès qu'ils incluent tous les premiers $p\leq N$, contradiction avec la divergence harmonique.
