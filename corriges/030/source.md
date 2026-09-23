# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td30-determinants.pdf)

## Autocorrection A

### 1



```math
\begin{array}{c|c|c}&\text{cycles non triviaux}&\varepsilon\\\hline(i)&(1\ 5\ 2\ 4\ 6\ 8)(3\ 9)&(-1)^{5+1}=1\\(ii)&(1\ 7\ 5\ 3)(2\ 9)(4\ 6)&(-1)^{3+1+1}=-1\\(iii)&(2\ 7\ 4\ 8\ 9)(3\ 6\ 5)&(-1)^{4+2}=1\\(iv)&(1\ 2)(3\ 5)(8\ 9)&(-1)^3=-1\end{array}
```



### 2

La signature d'un cycle de longueur $r$ vaut $(-1)^{r-1}$, et la signature d'un produit est le produit des signatures :



```math
(i)\ (-1)^{1+2+1}=1;\quad(ii)\ (-1)^7=-1;\quad(iii)\ (-1)^{1+3+2+2+3+1+2}=1;\quad(iv)\ (-1)^{2+1+4+2}=-1.
```



## Exercice 1

### 1

(i) La permutation inverse l'ordre de chaque paire ; elle possède $\binom n2$ inversions : $\varepsilon=(-1)^{n(n-1)/2}$.

(ii) C'est le cycle $(1\ n\ n-1\ \cdots\ 2)$ : $\varepsilon=(-1)^{n-1}$.

### 2

(i) Le produit des $n$ transpositions disjointes $(1\ 2),(3\ 4),\ldots,(2n-1\ 2n)$ a pour signature $(-1)^n$.

(ii) Dans la liste des impairs puis des pairs, $2i-1$ précède et dépasse exactement les $i-1$ pairs $2,4,\ldots,2i-2$. Le nombre d'inversions vaut $\sum_{i=1}^n(i-1)=n(n-1)/2$ ; signature $(-1)^{n(n-1)/2}$.

## Exercice 2

Pour $n=5$, le produit vaut $(1\ 2)(4\ 5)$. Si $\sigma_{n-1}=(1\ 2)(n-2\ n-1)$, alors



```math
\sigma_n=\sigma_{n-1}(n-2\ n-1\ n)=(1\ 2)(n-1\ n).
```



Ainsi, pour tout $n\ge5$,



```math
\boxed{\sigma=(1\ 2)(n-1\ n),\quad\operatorname{ord}(\sigma)=2,\quad\varepsilon(\sigma)=1}.
```



## Exercice 3

Prolonger $\sigma\in S_n$ par l'identité sur $\{n+1,n+2\}$ et poser



```math
\iota(\sigma)=\sigma(n+1\ n+2)^{(1-\varepsilon(\sigma))/2}.
```



Les deux facteurs commutent, les exposants s'additionnent modulo $2$, et $\varepsilon(\iota(\sigma))=1$. Ainsi $\iota$ est un morphisme vers $A_{n+2}$, injectif par restriction à $\{1,\ldots,n\}$.

## Exercice 4

Pour $n=1$, $\varphi$ est trivial ; prendre $\iota$ trivial. Pour $n\ge2$, toutes les transpositions sont conjuguées, donc, $A$ étant abélien, elles ont la même image $a$. Comme une transposition est d'ordre $2$, $a^2=1$.



```math
\sigma=\tau_1\cdots\tau_r\Longrightarrow\varphi(\sigma)=a^r,\qquad\varepsilon(\sigma)=(-1)^r.
```



L'application $\iota(1)=1$, $\iota(-1)=a$ est un morphisme et $\varphi=\iota\circ\varepsilon$.

## Exercice 5

Pour $n\ge2$, fixer une transposition $t$ et poser $\sigma'=t\sigma t^{-1}$. Toute permutation est paire ou s'écrit $\alpha t$ avec $\alpha$ paire. Ainsi



```math
C_S(\sigma)=C_A(\sigma)\cup C_A(\sigma').
```



Deux orbites d'une même action sont égales ou disjointes : si $\alpha\sigma\alpha^{-1}=\beta\sigma'\beta^{-1}$, alors $\sigma'$ est conjuguée à $\sigma$ dans $A_n$. D'où les deux possibilités demandées. Pour $n=1$, les deux classes sont réduites à l'identité.

## Exercice 6

Posons $a=(1\ 2\ 3)$, $b=(4\ 5\ 6)$ et $t=(1\ 4)(2\ 5)(3\ 6)$. Une permutation commutant à $ab$ envoie chaque orbite de $ab$ sur une orbite de même taille.

Si elle conserve les deux orbites, ses restrictions sont des puissances de $a$ et $b$. Si elle les échange, sa composée avec $t$ les conserve. Donc



```math
\boxed{C_{S_6}(ab)=\{a^ib^jt^\epsilon:0\le i,j\le2,\ \epsilon\in\{0,1\}\},\quad |C_{S_6}(ab)|=18}.
```



## Exercice 7

Soit $c=(1\ 2\ \cdots\ n)$. Si $\sigma c=c\sigma$ et $\sigma(1)=c^k(1)$, alors



```math
\sigma(c^j(1))=c^j\sigma(1)=c^{j+k}(1).
```



Les $c^j(1)$ parcourent tout l'ensemble ; donc $\sigma=c^k$. Le centralisateur est $\boxed{\langle c\rangle}$.

## Exercice 8

Les deux générateurs agissent de manière identique sur $(1,2,3,4)$ et $(5,6,7,8)$. Leur restriction au premier ensemble identifie le groupe engendré à



```math
H=\langle a=(1\ 2\ 3),\ b=(1\ 2)(3\ 4)\rangle\subset A_4.
```



Les conjugués $b,aba^{-1},a^2ba^{-2}$ sont les trois doubles transpositions. Avec l'identité, ils forment un sous-groupe $V$ d'ordre $4$, normalisé par $a$. Donc $V\langle a\rangle$ est un sous-groupe contenant les générateurs, et



```math
H=V\langle a\rangle,\qquad V\cap\langle a\rangle=\{1\},\qquad\boxed{|H|=4\cdot3=12}.
```



## Exercice 9

Si $\sigma$ est centrale, alors, pour tous $i\ne j$,



```math
(\sigma(i)\ \sigma(j))=\sigma(i\ j)\sigma^{-1}=(i\ j).
```



Pour $j,k$ distincts de $i$ et distincts entre eux, $\sigma(i)\in\{i,j\}\cap\{i,k\}=\{i\}$. Ainsi $\sigma(i)=i$ pour tout $i$ : le centre est trivial.

## Exercice 10

### 1

Si $\gamma\delta=\delta\gamma$, le support de $\gamma$ est stable par $\delta$ : $\gamma(x)\ne x$ implique $\gamma(\delta x)=\delta\gamma(x)\ne\delta x$. Si les supports se rencontrent, l'orbite de ce point sous le cycle $\delta$ donne $\operatorname{supp}\delta\subset\operatorname{supp}\gamma$. L'argument symétrique donne l'égalité.

### 2

Fixer $x$ ; pour une permutation $\sigma$ commutant avec le $n$-cycle $\gamma$, écrire $\sigma(x)=\gamma^k(x)$. Alors $\sigma(\gamma^jx)=\gamma^{j+k}x$ pour tout $j$, donc $\sigma=\gamma^k$.

## Exercice 11

### 1

Pour des cycles disjoints de longueurs $\ell_1,\ldots,\ell_r$,



```math
\sigma^m=1\iff\ell_i\mid m\ (\forall i),\qquad\boxed{\operatorname{ord}\sigma=\operatorname{ppcm}(\ell_1,\ldots,\ell_r)}.
```



### 2

L'ordre $14$ impose un cycle de longueur $7$ et un cycle de longueur $2$, les dix lettres ne permettant pas de cycle de longueur $14$. Il reste une lettre fixe. Donc $\varepsilon(\sigma)=(-1)^{6+1}=-1$.

### 3

Si la plus grande longueur vaut $10,9,8,7,6$, les ordres maximaux correspondants sont $10,9,8,21,12$. Si elle vaut $5$, les partitions possibles des cinq lettres restantes donnent un ordre au plus $\operatorname{ppcm}(5,3,2)=30$. Si elle est au plus $4$, l'ordre divise $\operatorname{ppcm}(1,2,3,4)=12$.

Le produit de cycles disjoints de longueurs $5,3,2$ a ordre $30$ : $\boxed{\max\operatorname{ord}(\sigma)=30}$.

## Exercice 12

### 1

Pour $i<j$, avec $\tau_k=(k\ k+1)$,



```math
(i\ j)=\tau_i\tau_{i+1}\cdots\tau_{j-2}\tau_{j-1}\tau_{j-2}\cdots\tau_i.
```



Toute transposition, puis toute permutation, appartient au groupe engendré.

### 2

Construire le graphe dont les sommets sont $1,\ldots,n$ et les arêtes les transpositions données. Chaque générateur conserve les composantes connexes. Un graphe connexe à $n$ sommets possède au moins $n-1$ arêtes ; avec moins d'arêtes, le groupe engendré n'est pas transitif, donc n'est pas $S_n$.

## Exercice 13

### 1



```math
\gamma^k(1\ 2)\gamma^{-k}=(k+1\ k+2)\quad(0\le k\le n-2).
```



Ces transpositions engendrent $S_n$.

### 2

Pour $\tau=(a\ b)$, poser $d=\gcd(n,b-a)$. Les conjugués de $\tau$ par les puissances de $\gamma$ sont les arêtes $\{x,x+b-a\}$ dans $\mathbb Z/n\mathbb Z$ ; leurs composantes sont les classes modulo $d$.

Si $d=1$, le graphe est connexe. Les transpositions d'un graphe connexe engendrent toutes les transpositions : le long d'un chemin, conjuguer successivement les transpositions des arêtes. Donc le groupe est $S_n$.

Si $d>1$, $\gamma$ permute les classes modulo $d$ et $\tau$ les conserve. Le groupe engendré préserve cette partition non triviale, contrairement à $S_n$.



```math
\boxed{\langle\gamma,\tau\rangle=S_n\iff\gcd(n,b-a)=1}.
```



## Exercice 14

Tout élément de $A_n$ est produit d'un nombre pair de transpositions. Regrouper celles-ci par paires. Deux transpositions égales s'annulent ; deux transpositions ayant une lettre commune donnent un $3$-cycle. Pour quatre lettres distinctes,



```math
(a\ b)(c\ d)=(a\ c\ b)(a\ c\ d).
```



Chaque paire est donc produit de $3$-cycles. Réciproquement, chaque $3$-cycle est pair ; ils engendrent exactement $A_n$.

## Exercice 15

Oui. Par récurrence, énumérer les permutations de $\{1,\ldots,n-1\}$ en commençant par l'identité, deux permutations consécutives différant par une transposition de positions adjacentes.

Pour chaque permutation de cette liste, insérer $n$ successivement dans les $n$ positions, de droite à gauche dans les blocs impairs et de gauche à droite dans les blocs pairs. À l'intérieur d'un bloc, deux mots diffèrent par un échange adjacent de $n$. Entre deux blocs, $n$ reste au même bout et les autres lettres subissent l'échange adjacent de l'énumération précédente.

On obtient ainsi les $n!$ permutations une seule fois, en commençant par l'identité. Si elles sont $\sigma_0,\ldots,\sigma_{n!-1}$, poser



```math
\tau_i=\sigma_i\sigma_{i-1}^{-1}.
```



Chaque $\tau_i$ est une transposition et $\sigma_i=\tau_i\cdots\tau_1$.

## Exercice 16

Pour $n\ge2$, soit $H$ contenant strictement $G$, et choisir $h\in H$ tel que $h(1)=j\ne1$. Comme $G$ agit transitivement sur $\{2,\ldots,n\}$, l'orbite de $1$ sous $H$ est tout l'ensemble. Son stabilisateur dans $H$ est exactement $G$. Donc



```math
|H|=n|G|=n(n-1)!=n!,
```



et $H=S_n$. Pour $n=1$, $G=S_1$ : il n'est pas un sous-groupe propre maximal ; il n'existe néanmoins aucun groupe strictement intermédiaire.

## Exercice 17

L'application $G\to\{1,\ldots,n\}$, $\sigma\mapsto\sigma(1)$ est surjective. Si $\sigma(1)=1$, pour tout $j$ choisir $\tau\in G$ tel que $\tau(1)=j$. Alors



```math
\sigma(j)=\sigma\tau(1)=\tau\sigma(1)=j.
```



Le stabilisateur de $1$ est trivial ; l'application est bijective et $\boxed{|G|=n}$.

## Exercice 18

### 1

$GL_2(\mathbb F_2)$ permute les trois vecteurs non nuls. L'action est fidèle car une application linéaire fixant ces vecteurs fixe une base. Or



```math
|GL_2(\mathbb F_2)|=(2^2-1)(2^2-2)=6=|S_3|.
```



Le morphisme injectif ainsi obtenu est un isomorphisme.

### 2

Les droites de $\mathbb F_3^2$ sont



```math
\langle(1,0)\rangle,\ \langle(0,1)\rangle,\ \langle(1,1)\rangle,\ \langle(1,-1)\rangle.
```



L'action sur ces quatre droites définit $\rho:GL_2(\mathbb F_3)\to S_4$. Une matrice du noyau stabilise les deux axes, donc vaut $\operatorname{diag}(a,b)$ ; la stabilité de $\langle(1,1)\rangle$ impose $a=b$. Le noyau est donc $\{I,-I\}$.



```math
|\operatorname{im}\rho|=\frac{(9-1)(9-3)}2=24=|S_4|.
```



Ainsi $\rho$ est surjective.

## Exercice 19

Soustraire la première ligne à toutes les autres. Tous les coefficients des $n-1$ dernières lignes appartiennent à $\{-2,0,2\}$. En extrayant $2$ de chacune,



```math
\det A=2^{n-1}\det B,\qquad B\in M_n(\mathbb Z).
```



Donc $\det A\in2^{n-1}\mathbb Z$.

## Exercice 20

La somme définissant $\varphi$ est multilinéaire. Si deux arguments sont égaux, tous les termes sont nuls sauf éventuellement ceux où $u$ agit sur l'un de ces deux arguments ; ces deux termes s'annulent par échange des deux places. Donc $\varphi$ est alternée, et $\varphi=c\det$.

Pour une base $(e_i)$ de déterminant $1$, si $u(e_j)=\sum_i a_{ij}e_i$,



```math
c=\varphi(e_1,\ldots,e_n)=\sum_{j=1}^na_{jj}=\operatorname{tr}u.
```





```math
\boxed{\varphi=(\operatorname{tr}u)\det}.
```



## Exercice 21

La somme et les multiples scalaires de formes $p$-linéaires alternées sont encore $p$-linéaires alternées. Fixer une base $(e_1,\ldots,e_n)$.

Une telle forme est déterminée par ses valeurs sur les $p$-uplets de vecteurs de base. Les valeurs comportant une répétition sont nulles ; les autres sont déterminées, à la signature près, par



```math
\omega(e_{i_1},\ldots,e_{i_p}),\qquad i_1<\cdots<i_p.
```



Pour chaque partie $I=\{i_1<\cdots<i_p\}$, la forme



```math
\omega_I(v_1,\ldots,v_p)=\det\bigl(e_{i_a}^*(v_b)\bigr)_{1\le a,b\le p}
```



prend la valeur $1$ sur le $p$-uplet croissant indexé par $I$, et $0$ sur les autres. Les $\omega_I$ forment donc une base.



```math
\boxed{\dim\Lambda^pE^*=\binom np\ (0\le p\le n),\qquad\dim\Lambda^pE^*=0\ (p>n)}.
```



Pour $p=0$, la forme est un scalaire et la dimension vaut $1$.

## Autocorrection B

### (i)



```math
L_3=(a+b+c)L_1-L_2\Longrightarrow\boxed{\det=0}.
```



### (ii)

Effectuer $L_3\leftarrow L_3-aL_2$, puis $L_2\leftarrow L_2-aL_1$ :



```math
\boxed{\det=(1-a^2)^2}.
```



### (iii)

Les vecteurs $(1,1,1,1)$, $(1,-1,-1,1)$, $(1,1,-1,-1)$, $(1,-1,1,-1)$ sont propres, avec valeurs respectives $a+b+2c$, $a+b-2c$, $a-b$, $a-b$. Ils sont indépendants, donc



```math
\boxed{\det=(a-b)^2\bigl((a+b)^2-4c^2\bigr)}.
```



### (iv)

Chaque ligne est combinaison de $(a^2,b^2,c^2,d^2)$, $(a,b,c,d)$ et $(1,1,1,1)$. Le rang est au plus $3$ ; $\boxed{\det=0}$.

### (v)

La permutation de renversement a $n(n-1)/2$ inversions :



```math
\boxed{\det\left(\sum_i a_iE_{i,n+1-i}\right)=(-1)^{n(n-1)/2}\prod_{i=1}^na_i}.
```



### (vi)

La matrice a pour coefficient $a_{\min(i,j)}$, où $a_i=1$ pour $i$ impair et $a_i=0$ pour $i$ pair. Si $L$ est triangulaire inférieure remplie de $1$, elle s'écrit



```math
L\operatorname{diag}(a_1,a_2-a_1,\ldots,a_n-a_{n-1})L^T.
```



Donc $\boxed{D_n=(-1)^{\lfloor n/2\rfloor}}$.

## Exercice 22

### (i)

Le développement sur la dernière ligne donne



```math
D_n=(1+x^2)D_{n-1}-x^2D_{n-2},\qquad D_0=1,\quad D_1=1+x^2.
```



La récurrence est satisfaite par $\sum_{k=0}^nx^{2k}$, donc



```math
\boxed{D_n=\sum_{k=0}^nx^{2k}=\begin{cases}\dfrac{1-x^{2n+2}}{1-x^2},&x^2\ne1,\\n+1,&x^2=1.\end{cases}}
```



### (ii)

Soustraire la dernière ligne à chacune des $n-1$ premières : la ligne $i<n$ n'a plus que le coefficient $i-n$ en colonne $i$. Le développement suivant la dernière colonne donne



```math
\boxed{D_n=n\prod_{i=1}^{n-1}(i-n)=(-1)^{n-1}n!}.
```



### (iii)

Pour $n\ge2$ et $z\ne0$, remplacer $L_1$ par $L_1-(x/z)\sum_{i=2}^nL_i$ :



```math
D_n=\left(a-\frac{(n-1)xy}{z}\right)z^{n-1}.
```



Par identité polynomiale, pour tout $z$,



```math
\boxed{D_n=az^{n-1}-(n-1)xyz^{n-2}}.
```



Pour $n=1$, $D_1=a$.

### (iv)



```math
M_{ij}=S_{\min(i,j)}=\sum_{k\le\min(i,j)}k,\qquad M=L\operatorname{diag}(1,2,\ldots,n)L^T.
```





```math
\boxed{\det M=n!}.
```



## Exercice 23

### (i)

Pour une matrice $(b_{\max(i,j)})$, soustraire la ligne $i+1$ à la ligne $i$, dans l'ordre $i=1,\ldots,n-1$. Les premières lignes ont pour dernier coefficient non nul, en colonne $i$, $b_i-b_{i+1}$. Ainsi



```math
\det(b_{\max(i,j)})=b_n\prod_{i=1}^{n-1}(b_i-b_{i+1}).
```



Avec $b_i=a^i$,



```math
\boxed{\det(a^{\max(i,j)})=a^{n(n+1)/2}(1-a)^{n-1}}.
```



### (ii)

Le polynôme $\binom Xk$ a degré $k$ et coefficient dominant $1/k!$. Donc



```math
\det\left(\binom i{j-1}\right)=\frac{\prod_{1\le i<j\le n}(j-i)}{\prod_{k=0}^{n-1}k!}=\boxed1.
```



### (iii)

L'identité de Vandermonde donne



```math
\binom{i+j-2}{i-1}=\sum_{k\ge0}\binom{i-1}k\binom{j-1}k.
```



La matrice est donc $LL^T$, où $L_{ik}=\binom{i-1}{k-1}$ est triangulaire inférieure de diagonale $1$. Son déterminant vaut $\boxed1$.

### (iv)

Les colonnes sont les évaluations aux points $1,\ldots,n$ des polynômes $X\mapsto P(X+j-1)$, tous dans $\mathbb R_{n-2}[X]$, de dimension $n-1$. Les $n$ colonnes sont liées ; $\boxed{\det=0}$.

## Exercice 24

### 1

Pour $n\ge1$, $Jx=(\sum_i x_i)\mathbf1$, donc



```math
\mathbb R^n=\mathbb R\mathbf1\oplus\left\{x:\sum_i x_i=0\right\},\qquad J\sim\operatorname{diag}(n,0,\ldots,0).
```



### 2



```math
M=(a-b)I+bJ\sim\operatorname{diag}(a+(n-1)b,a-b,\ldots,a-b).
```





```math
\boxed{\det M=(a-b)^{n-1}(a+(n-1)b)}.
```



Le déterminant vide, pour $n=0$, vaut $1$.

## Exercice 25

### 1



```math
Ce_j=e_{j+1}\ (j<n),\qquad Ce_n=e_1.
```



$C$ représente le cycle $(1\ 2\ \cdots\ n)$ ; donc $C^n=I$.

### 2

Pour $\omega^n=1$,



```math
CX=\omega X\iff X=x_1(1,\omega^{-1},\ldots,\omega^{-(n-1)})^T.
```



L'espace propre est une droite. Les $n$ valeurs propres distinctes $1,\zeta,\ldots,\zeta^{n-1}$ donnent une base propre, donc $C\sim\operatorname{diag}(1,\zeta,\ldots,\zeta^{n-1})$.

### 3

La matrice affichée est $M=\sum_{k=0}^{n-1}a_kC^{-k}$. Dans cette base propre,



```math
\det M=\prod_{j=0}^{n-1}\left(\sum_{k=0}^{n-1}a_k\zeta^{-jk}\right)=\boxed{\prod_{j=0}^{n-1}\left(a_0+\zeta^ja_1+\cdots+\zeta^{j(n-1)}a_{n-1}\right)}.
```



La dernière égalité utilise la permutation $j\mapsto-j$ modulo $n$.

## Exercice 26

### 1



```math
\begin{pmatrix}I&0\\-CA^{-1}&I\end{pmatrix}\begin{pmatrix}A&B\\C&D\end{pmatrix}=\begin{pmatrix}A&B\\0&D-CA^{-1}B\end{pmatrix}.
```



Le premier facteur a déterminant $1$, donc



```math
\boxed{\det M=\det A\det(D-CA^{-1}B)}.
```



### 2

Correction : sous $AC=CA$, le second membre est $\det(AD-CB)$.



```math
\det M=\det\bigl(A(D-CA^{-1}B)\bigr)=\boxed{\det(AD-CB)}.
```



La formule imprimée $\det(AD-BC)$ est fausse. Par exemple,



```math
A=\begin{pmatrix}1&0\\0&2\end{pmatrix},\ C=\begin{pmatrix}3&0\\0&4\end{pmatrix},\ B=\begin{pmatrix}0&1\\1&0\end{pmatrix},\ D=\begin{pmatrix}1&2\\3&4\end{pmatrix}
```



vérifient $AC=CA$, mais $\det M=10$ et $\det(AD-BC)=14$.

## Exercice 27

Posons $L_{ik}=1$ si $k\mid i$, et $0$ sinon. Alors



```math
(LL^T)_{ij}=\sum_{k=1}^n\mathbf1_{k\mid i}\mathbf1_{k\mid j}
```



est le nombre de diviseurs communs à $i,j$. Donc $A=LL^T$. La matrice $L$ est triangulaire inférieure de diagonale $1$ ; $\boxed{\det A=1}$.

## Exercice 28



```math
\boxed{\det\left(\frac1{a_i+b_j}\right)=\frac{\displaystyle\prod_{i<j}(a_j-a_i)(b_j-b_i)}{\displaystyle\prod_{i,j}(a_i+b_j)}}.
```



Pour la preuve, travailler d'abord avec des indéterminées et multiplier le déterminant par $\prod_{i,j}(a_i+b_j)$. Le numérateur obtenu est un polynôme alterné en les $a_i$, puis en les $b_j$ ; il est donc divisible par les deux produits de Vandermonde. Son degré total vaut $n^2-n$, exactement celui de leur produit. Il est donc égal à ce produit multiplié par une constante $c_n$.

Multiplier par $a_n+b_n$ puis substituer $a_n=-b_n$ dans la formule rationnelle. Dans le déterminant, le développement suivant la dernière ligne laisse seulement le mineur de taille $n-1$. Dans le produit proposé, les facteurs supplémentaires se simplifient :



```math
\frac{\prod_{i<n}(-b_n-a_i)\prod_{j<n}(b_n-b_j)}{\prod_{j<n}(-b_n+b_j)\prod_{i<n}(a_i+b_n)}=1.
```



Ainsi $c_n=c_{n-1}$ et $c_1=1$. L'identité polynomiale universelle obtenue se spécialise dans tout corps, les dénominateurs étant non nuls.

## Exercice 29

Notons $V=\prod_{i<j}(x_j-x_i)$ et $e_r$ le polynôme symétrique élémentaire de degré $r$ en les $x_i$, avec $e_0=1$.

Ajouter à la matrice de Vandermonde d'exposants $0,\ldots,n$ la dernière ligne $(1,t,\ldots,t^n)$. Son déterminant vaut



```math
V\prod_{i=1}^n(t-x_i)=V\sum_{k=0}^n(-1)^{n-k}e_{n-k}t^k.
```



Le développement suivant cette dernière ligne donne pour coefficient de $t^k$ : $(-1)^{n+k}D_k$, où $D_k$ est le déterminant demandé. Donc



```math
\boxed{D_k=e_{n-k}(x_1,\ldots,x_n)\prod_{i<j}(x_j-x_i)}.
```



## Exercice 30

En caractéristique différente de $2$,



```math
E=E_1(s)\oplus E_{-1}(s),\qquad s\sim\operatorname{diag}(I_r,-I_{n-r}),\qquad\boxed{\det s=(-1)^{n-r}},\quad r=\dim E_1(s).
```



En caractéristique $2$, $s^2=I$ donne $(\det s)^2=1$, donc $\det s=1$, et la même expression scalaire vaut $1$.

## Exercice 31



```math
\varphi(X^k)=(1-X)^k=(-1)^kX^k+\text{termes de degré inférieur}.
```



La matrice est triangulaire de diagonale $1,-1,\ldots,(-1)^n$. Ainsi



```math
\boxed{\operatorname{tr}\varphi=\frac{1+(-1)^n}{2},\qquad\det\varphi=(-1)^{n(n+1)/2}}.
```



## Exercice 32

La famille $(e^x,xe^x,\ldots,x^ne^x)$ est une base de $E$ : une relation se réduit, après division par $e^x$, à une relation polynomiale. Or



```math
D(x^ke^x)=x^ke^x+kx^{k-1}e^x.
```



La matrice de $D$ est triangulaire de diagonale $1$ ; $\boxed{\det D=1}$.

## Exercice 33

### 1

Une racine multiple $z$ vérifierait $nz^{n-1}=1$ et $z^n-z+1=0$, donc $z/n-z+1=0$ et $z=n/(n-1)>1$. Alors $nz^{n-1}>1$, contradiction. Par le théorème fondamental de l'algèbre, $P$ est simplement scindé sur $\mathbb C$.

### 2

Les racines sont non nulles. La multilinéarité, ou la formule du déterminant d'une perturbation de rang $1$, donne



```math
\det(\operatorname{diag}(z_i)+\mathbf1\mathbf1^T)=\prod_i z_i\left(1+\sum_i\frac1{z_i}\right).
```





```math
\prod_i z_i=(-1)^nP(0)=(-1)^n,\qquad\sum_i\frac1{z_i}=-\frac{P'(0)}{P(0)}=1.
```





```math
\boxed{\det=2(-1)^n}.
```



## Exercice 34

### 1

Pour $\deg P_j=j$ et coefficient dominant $c_j$, la matrice des coefficients des $P_j$ dans $(1,X,\ldots,X^{n-1})$ est triangulaire de diagonale $(c_j)$. Ainsi



```math
\boxed{\det(P_{j-1}(x_i))=\left(\prod_{j=0}^{n-1}c_j\right)\prod_{i<j}(x_j-x_i)}.
```



Si « échelonnée » signifie seulement degrés strictement croissants sans $\deg P_j=j$, cette formule ne s'applique pas : par exemple $(1,X^2)$ donne $(x_2-x_1)(x_1+x_2)$.

### 2



```math
\cos(k\theta)=T_k(\cos\theta),\qquad T_0=1,\ T_1=X,\ T_{k+1}=2XT_k-T_{k-1}.
```



Ainsi $\deg T_k=k$ et son coefficient dominant vaut $2^{k-1}$ pour $k\ge1$. Donc



```math
\boxed{\det=2^{(n-1)(n-2)/2}\prod_{i<j}(\cos\theta_j-\cos\theta_i)}\quad(n\ge1).
```



## Exercice 35

### 1



```math
M=(x_i^j)_{0\le i,j\le n}\in M_{n+1}(\mathbb Z),\qquad(P(x_i))_i=M(a_j)_j.
```





```math
\det M=\prod_{i<j}(x_j-x_i)\in\mathbb Z\setminus\{0\}.
```



### 2

Correction d'indices : les valeurs considérées sont $P(x_0),\ldots,P(x_n)$.



```math
d=|\det M|\ge1,\qquad dM^{-1}=\pm\operatorname{adj}(M)\in M_{n+1}(\mathbb Z).
```



Si toutes les valeurs sont entières, le vecteur des coefficients de $dP$ est entier ; donc $dP\in\mathbb Z[X]$.

### 3

Non. Pour $P=\sqrt2\prod_{i=0}^n(X-x_i)$, toutes les valeurs prescrites sont nulles, mais, pour tout entier $d\ge1$, le coefficient dominant de $dP$ est $d\sqrt2\notin\mathbb Z$.

## Exercice 36

### 1

Écrire les colonnes de $A+tB$ sous la forme $A_j+tB_j$ et développer par multilinéarité. Le coefficient de $t^k$ est une somme de déterminants utilisant $k$ colonnes de $B$. Si $k>\operatorname{rg}B$, ces colonnes sont liées. Donc



```math
\deg\det(A+tB)\le\operatorname{rg}B.
```



### 2



```math
\chi_A(t)=\det(tI-A)=t^n+\text{termes de degré inférieur}.
```



Il s'agit d'un polynôme unitaire de degré $n$, et



```math
\chi_A(\lambda)=0\iff\ker(\lambda I-A)\ne0.
```



Ses racines réelles sont les valeurs propres réelles de $A$ ; sur $\mathbb C$, ses racines sont les valeurs propres complexes.

### 3

Le polynôme $t\mapsto\det(A+tI)$ n'a qu'un nombre fini de racines. Choisir $t_k\in(0,1/k)$ évitant ces racines. Alors



```math
A_k=A+t_kI\in GL_n(\mathbb R),\qquad A_k\longrightarrow A.
```



## Exercice 37

Comme $\operatorname{rg}B=1$, $\det(A+tB)=a+bt$, où $a=\det A$. Donc



```math
\det((A+B)(A-B))=(a+b)(a-b)=a^2-b^2\le\boxed{(\det A)^2}.
```



## Exercice 38

### 1



```math
\det A=\det A^T=\det(-A)=(-1)^{2n+1}\det A=-\det A\Longrightarrow\det A=0.
```



### 2

Pour $J=\mathbf1\mathbf1^T$, la fonction $p(t)=\det(A+tJ)$ est affine. Or



```math
p(t)=\det(-A+tJ)=\det(A-tJ)=p(-t).
```



Elle est donc constante : $\boxed{\det(A+tJ)=\det A}$.

### 3

Réduire les coefficients modulo $2$ : $\overline A=I+J$ dans $M_{2n}(\mathbb F_2)$. Comme $J^2=(2n)J=0$,



```math
(I+J)^2=I.
```



Donc $\det\overline A=1$ ; l'entier $\det A$ est impair et en particulier non nul.

### 4

Soit $m=(m_1,\ldots,m_{2n+1})^T$ le vecteur des masses. Pour chaque caillou $i$ retiré, coder les deux tas par $+1$ et $-1$, et mettre $0$ à la place $i$. Les lignes ainsi obtenues forment une matrice $A$ telle que



```math
Am=0,\qquad A\mathbf1=0.
```



Tout mineur principal de taille $2n$ est inversible par la question 3. Ainsi $\operatorname{rg}A\ge2n$. Comme $\mathbf1\in\ker A$, le rang vaut exactement $2n$ et $\ker A=\mathbb R\mathbf1$. Donc $m_1=\cdots=m_{2n+1}$.

## Exercice 39



```math
J^2=-I_n\Longrightarrow(\det J)^2=(-1)^n>0\Longrightarrow n\text{ pair}.
```



Pour $n=2r$, prendre $J=\operatorname{diag}(R,\ldots,R)$ avec $R=\begin{pmatrix}0&-1\\1&0\end{pmatrix}$. Alors $J^2=-I_n$.

## Exercice 40

### 1

Notons $D_n$ le déterminant demandé. Il est affine en $r_n$, de coefficient dominant $D_{n-1}$. À $r_n=b$, soustraire la dernière colonne aux $n-1$ autres : le dernier coefficient vaut $b$, et le bloc restant est triangulaire inférieur de diagonale $(r_i-a)_{i<n}$. Donc



```math
D_n=(r_n-b)D_{n-1}+b\prod_{i=1}^{n-1}(r_i-a),\qquad D_1=r_1.
```



Par récurrence, si $a\ne b$,



```math
\boxed{D_n=\frac{a\prod_{i=1}^n(r_i-b)-b\prod_{i=1}^n(r_i-a)}{a-b}}.
```



Pour $a=b=c$, la continuité polynomiale, ou le développement de $\operatorname{diag}(r_i-c)+cJ$, donne



```math
\boxed{D_n=\prod_i(r_i-c)+c\sum_{i=1}^n\prod_{j\ne i}(r_j-c)}.
```



### 2

Pour $c=1$ et $r_i>1$, tous les termes de la dernière expression sont strictement positifs. Le déterminant est donc strictement positif.

### 3

Soient $m$ les droites déterminées par les $n$ points, et $N\in M_{n,m}(\mathbb R)$ leur matrice d'incidence. Deux points distincts appartiennent à exactement une droite, donc



```math
(NN^T)_{ij}=1\ (i\ne j),\qquad(NN^T)_{ii}=r_i,
```



où $r_i$ compte les droites passant par le point $i$. Puisque les points ne sont pas tous alignés, $r_i\ge2$ pour tout $i$. La question 2 donne $NN^T$ inversible ; ainsi



```math
n=\operatorname{rg}(NN^T)\le\operatorname{rg}N\le m.
```



## Exercice 41

L'énoncé imprimé est contradictoire pour $i=j$ : sa deuxième hypothèse impose $a_{ii}=0$. Correction : imposer cette deuxième hypothèse seulement pour $i\ne j$.

Pour une permutation $\sigma\ne\operatorname{id}$, choisir un cycle $(i_1,\ldots,i_r)$ de longueur $r\ge2$. Si tous les facteurs $a_{i_k,i_{k+1}}$ de ce cycle étaient non nuls, la transitivité donnerait $a_{i_2,i_1}\ne0$, en contradiction avec $a_{i_1,i_2}\ne0$. Ainsi le terme de Leibniz associé à $\sigma$ est nul.



```math
\boxed{\det A=\prod_{i=1}^na_{ii}\ne0}.
```



## Exercice 42

Le déterminant vaut



```math
D=(x_2-x_1)(f(x_3)-f(x_1))-(x_3-x_1)(f(x_2)-f(x_1)).
```



Puisque $x_3-x_1>0$,



```math
D\ge0\iff f(x_2)\le\frac{x_3-x_2}{x_3-x_1}f(x_1)+\frac{x_2-x_1}{x_3-x_1}f(x_3).
```



Cette condition pour tous $x_1<x_2<x_3$ est exactement la convexité de $f$ sur $I$.

## Exercice 43

Si $\sum_i a_if_i=0$ et la matrice $(f_i(x_j))$ est inversible, l'évaluation aux $x_j$ donne $a_i=0$ pour tout $i$.

Réciproquement, poser $v(x)=(f_1(x),\ldots,f_n(x))\in\mathbb R^n$. Si leur espace engendré était propre, une forme linéaire non nulle l'annulerait, donnant une relation non triviale entre les $f_i$. Donc les $v(x)$ engendrent $\mathbb R^n$ ; en extraire une base $v(x_1),\ldots,v(x_n)$ donne le déterminant non nul.

## Exercice 44

Si $M,N\in M_n(\mathbb Z)$ et $MN=I$, alors $\det M\det N=1$ dans $\mathbb Z$, donc $\det M=\pm1$.

Réciproquement, si $\det M=\pm1$,



```math
M^{-1}=\frac{\operatorname{adj}(M)}{\det M}=\pm\operatorname{adj}(M)\in M_n(\mathbb Z).
```



Donc $\boxed{GL_n(\mathbb Z)=\{M\in M_n(\mathbb Z):\det M=\pm1\}}$.

## Exercice 45



```math
p(t)=\det(A+tB)\in\mathbb Z[t],\qquad\deg p\le2.
```



Les cinq valeurs $p(0),\ldots,p(4)$ appartiennent à $\{-1,1\}$. L'une de ces deux valeurs apparaît au moins trois fois ; le polynôme $p-1$ ou $p+1$, de degré au plus $2$, possède donc trois racines distinctes et est nul. Ainsi $p\equiv\pm1$, en particulier $\det(A+5B)=\pm1$.

## Exercice 46

### 1

Pour $n=1$, prendre $f(x,y)=x+y$.

Pour $n\ge2$, poser $A=I_n$ et $B_t=\operatorname{diag}(t,0,\ldots,0)$. Alors $\det A=1$, $\det B_t=0$, mais $\det(A+B_t)=1+t$ varie avec $t$. Aucune telle fonction n'existe.

### 2

Pour $n=1$, toutes les matrices conviennent. Pour $n\ge2$, la propriété est invariante par équivalence : écrire $A=PJ_rQ$, avec $P,Q$ inversibles et $J_r=\operatorname{diag}(I_r,0)$, puis poser $B=PCQ$.

Si $1\le r<n$, choisir $C=\operatorname{diag}(0_r,I_{n-r})$. Alors $\det(J_r+C)=1$, tandis que $\det J_r+\det C=0$.

Si $r=n$, choisir $C=\operatorname{diag}(1,0,\ldots,0)$. Alors $\det(I+C)=2\ne1=\det I+\det C$.

Il reste $r=0$, qui convient : $\boxed{A=0\quad(n\ge2)}$.

## Exercice 47

La comatrice et l'adjointe sont transposées, donc ont même rang. Posons $r=\operatorname{rg}A$.

Si $r=n$, $\operatorname{adj}(A)=(\det A)A^{-1}$ est inversible : rang $n$.

Si $r\le n-2$, tous les mineurs d'ordre $n-1$ sont nuls : rang $0$.

Si $r=n-1$, au moins un mineur d'ordre $n-1$ est non nul, donc l'adjointe n'est pas nulle. Comme $A\operatorname{adj}(A)=0$, son image est contenue dans $\ker A$, de dimension $1$ ; son rang vaut $1$.



```math
\boxed{\operatorname{rg}\operatorname{com}(A)=\begin{cases}n,&r=n,\\1,&r=n-1,\\0,&r\le n-2.\end{cases}}
```



Pour $n=1$, la comatrice vaut $(1)$, y compris lorsque $A=0$.

## Exercice 48

Sur $\mathbb C^{2n}$, les sous-espaces $\{(x,ix):x\in\mathbb C^n\}$ et $\{(x,-ix):x\in\mathbb C^n\}$ sont supplémentaires. La matrice $M=\begin{pmatrix}A&B\\-B&A\end{pmatrix}$ les stabilise, avec restrictions $A+iB$ et $A-iB$.



```math
\det M=\det(A+iB)\det(A-iB)=\boxed{|\det(A+iB)|^2\ge0}.
```



## Exercice 49

Notons $p_1,\ldots,p_p$ les colonnes de $P$. La colonne $j$ de $PQ$ est $\sum_{k=1}^pq_{kj}p_k$. Par multilinéarité,



```math
\det(PQ)=\sum_{k_1,\ldots,k_n}q_{k_1,1}\cdots q_{k_n,n}\det(p_{k_1},\ldots,p_{k_n}).
```



Les termes avec répétition sont nuls. Pour une partie $I=\{i_1<\cdots<i_n\}$, sommer les termes $k_j=i_{\sigma(j)}$ donne



```math
\det(P_I)\sum_{\sigma\in S_n}\varepsilon(\sigma)\prod_{j=1}^nq_{i_{\sigma(j)},j}=\det(P_I)\det(Q_I).
```



Donc $\boxed{\det(PQ)=\sum_{|I|=n}\det(P_I)\det(Q_I)}$.

Si $n>p$, $\operatorname{rg}(PQ)\le p<n$, donc $\det(PQ)=0$ ; la somme sur les parties de cardinal $n$ est vide.

## Exercice 50

Écrire $P=X+iY$ avec $X,Y$ réelles. L'égalité $BP=PA$ donne $BX=XA$ et $BY=YA$. Le polynôme réel $q(t)=\det(X+tY)$ n'est pas identiquement nul, puisque



```math
q(i)=\det(X+iY)=\det P\ne0.
```



Choisir $t\in\mathbb R$ tel que $q(t)\ne0$. Alors $Q=X+tY\in GL_n(\mathbb R)$ et $BQ=QA$, donc $\boxed{B=QAQ^{-1}}$.

## Exercice 51

### 1

Pour $1\le k\le n^2$, poser $c_k=2^{2^k}$. Dans toute matrice utilisant exactement ces coefficients, chaque terme non nul de Leibniz vaut, au signe près, $2^s$, où $s$ est la somme des $2^k$ correspondant aux $n$ positions sélectionnées.

Deux permutations sélectionnent deux ensembles distincts de positions ; l'unicité de l'écriture binaire rend leurs exposants distincts. Le terme de plus grand exposant domine strictement la somme des valeurs absolues de tous les autres :



```math
\sum_{s<S}2^s\le2^S-1<2^S.
```



Le déterminant est donc non nul pour toute disposition des $c_k$.

### 2

Posons $M=\max c_k$, $N=1+n!M^n$, $\epsilon=1/N$, et



```math
\boxed{a_k=1+\epsilon c_k}.
```



Ils sont distincts et appartiennent à $[1,2]$. Pour une disposition quelconque, écrire la matrice obtenue sous la forme $J+\epsilon C$, où $C$ utilise les $c_k$. Pour $n\ge2$, puisque $J$ a rang $1$, la multilinéarité donne



```math
\det(J+tC)=t^{n-1}(u+vt),\qquad u\in\mathbb Z,\quad v=\det C\in\mathbb Z\setminus\{0\}.
```



De plus $|v|\le n!M^n<N$. Si $u=0$, $u+v\epsilon\ne0$. Si $u\ne0$,



```math
|u+v\epsilon|\ge|u|-|v|/N>1-1=0.
```



Ainsi toutes les dispositions des $a_k$ sont inversibles. Pour $n=1$, tout unique coefficient dans $[1,2]$ convient.

## Exercice 52

### (ii) implique (i)

Pour tout $t\in\mathbb R$, $(A+tB)(V)\subset W$. Comme $\dim V>\dim W$, la restriction à $V$ possède un noyau non nul ; $A+tB$ est singulière.

### (i) implique (ii)

Le polynôme $p(t)=\det(A+tB)$, de degré au plus $n$, possède $n+1$ racines distinctes ; donc $p\equiv0$. La matrice $A+tB$ est singulière sur le corps $\mathbb R(t)$ ; après multiplication par un dénominateur commun, il existe un vecteur polynomial non nul $v(t)$ tel que $(A+tB)v(t)=0$.

Choisir un tel vecteur de degré minimal $d$, et écrire



```math
v(t)=v_0+tv_1+\cdots+t^dv_d,\qquad v_d\ne0.
```



L'identification des coefficients donne



```math
Av_0=0,\qquad Av_i=-Bv_{i-1}\ (1\le i\le d),\qquad Bv_d=0.
```



Les vecteurs $v_0,\ldots,v_d$ sont indépendants. En effet, supposons $\sum_{i=0}^dc_iv_i=0$ avec certains $c_i\ne0$. Pour $0\le i<d$, poser



```math
w_{i+1}(t)=v_{i+1}+tv_{i+2}+\cdots+t^{d-i-1}v_d.
```



Les relations précédentes donnent $(A+tB)w_{i+1}=-Bv_i$. Par conséquent,



```math
w(t)=\sum_{i=0}^{d-1}c_iw_{i+1}(t)\quad\text{vérifie}\quad(A+tB)w=-B\sum_{i=0}^{d-1}c_iv_i=c_dBv_d=0.
```



Soit $j$ le plus petit indice tel que $c_j\ne0$. Il vérifie $j<d$, car $v_d\ne0$. Les degrés des $w_{i+1}$ décroissent strictement avec $i$, et le coefficient dominant de $w$ est $c_jv_d\ne0$. Ainsi $w\ne0$ et $\deg w=d-j-1<d$, contradiction. Pour $d=0$, l'indépendance est immédiate.

Poser enfin



```math
V=\operatorname{Vect}(v_0,\ldots,v_d),\qquad W=\operatorname{Vect}(Bv_0,\ldots,Bv_{d-1}),
```



avec $W=\{0\}$ si $d=0$. Alors



```math
A(V)\subset W,\quad B(V)\subset W,\qquad\dim V=d+1>d\ge\dim W.
```


