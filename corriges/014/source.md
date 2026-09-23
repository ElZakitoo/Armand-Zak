# corrigé zakito

[Énoncé exact](https://www.bourrigan.fr/data/td14-reels.pdf)

## Autocorrections

### A

Si $a\ne0$, on choisit $\varepsilon=|a|/2$, ce qui contredit $|a|\leq\varepsilon$. Donc $a=0$.

### B

Pour $n\in\mathbb Z$, $a\leq n$ équivaut à $\lceil a\rceil\leq n$, et $n\leq b$ équivaut à $n\leq\lfloor b\rfloor$. Ainsi


```math
[a,b]\cap\mathbb Z=\{\lceil a\rceil,\ldots,\lfloor b\rfloor\},
```


ensemble vide si la borne inférieure dépasse la borne supérieure.

### C

1. L'entier $\lfloor r\rfloor+1$ appartient à $[r,s]$ si $s-r>1$.
2. Pour tout intervalle ouvert $(u,v)$, prenons $m$ tel que $k^m(v-u)>1$. L'intervalle $(k^mu,k^mv)$ contient un entier $n$, donc $n/k^m\in D_k\cap(u,v)$.
3. Avec $k=2$, $D_2\subset\mathbb Q$ et $D_2$ est dense; donc $\mathbb Q$ est dense.

### D

Tout majorant de $B$ majore $A$ et tout minorant de $B$ minore $A$. Par conséquent


```math
\sup A\leq\sup B,\qquad \inf A\geq\inf B.
```



### E

(i) $\inf=0$ sans minimum, $\sup=1$ maximum. (ii) Le set est $\{0\}\cup\{1/n:n\geq1\}$ : mêmes bornes, et minimum $0$. (iii) $\inf=-1$ et $\sup=1$, tous deux atteints. (iv) $\inf=a$, $\sup=b$, aucun n'est atteint. (v) Les termes pairs sont $1+1/n$ et les impairs $-1+1/n$; $\sup=3/2$ maximum (à $n=2$), $\inf=-1$ non atteint. (vi) Les termes pairs sont $1+1/n$ et les impairs $1-1/n$; $\inf=0$ minimum (à $n=1$), $\sup=3/2$ maximum (à $n=2$). (vii) Les termes pairs sont $1-1/n$ et les impairs $-1+1/n$; $\inf=-1$ et $\sup=1$, aucun des deux n’étant atteint.

## Partie entière

### Exercice 1

(i) Écrivons $x=p+u$, $y=q+v$, avec $p,q\in\mathbb Z$ et $u,v\in[0,1)$. Alors $\lfloor x+y\rfloor=p+q+\lfloor u+v\rfloor$, où $\lfloor u+v\rfloor\in\{0,1\}$.

(ii) Écrivons $x=p+u$ comme ci-dessus. $\lfloor nx\rfloor=np+\lfloor nu\rfloor$, et $0\leq\lfloor nu\rfloor<n$. Donc $\lfloor\lfloor nx\rfloor/n\rfloor=p$.

(iii) Si $u=\{x\}$, alors $\lfloor2x\rfloor=2p+\lfloor2u\rfloor$ tandis que $\lfloor x+1/2\rfloor=p+\lfloor u+1/2\rfloor$. Ces deux derniers planchers sont liés par $\lfloor2u\rfloor=\lfloor u+1/2\rfloor$.

### Exercice 2

Écrivons $x=p+u$, $p\in\mathbb Z$, $u\in[0,1)$. La somme vaut $np+\sum_{j=0}^{n-1}\lfloor u+j/n\rfloor$. Si $u=0$, cette dernière somme est $0$. Si $u>0$, ses termes valent $0$ pour $j<n(1-u)$ et $1$ ensuite; leur somme est $\lfloor nu\rfloor$. Dans les deux cas la somme totale est $np+\lfloor nu\rfloor=\lfloor nx\rfloor$.

### Exercice 3

$f(x)=\lfloor3x\rfloor-3x$ vérifie $f(x+1/3)=f(x)$; sa période fondamentale est $1/3$. Sur $[k/3,(k+1)/3[$, $f(x)=k-3x$, droite décroissante de $0$ (atteint à gauche) à la limite $-1$ (non atteinte).

Pour $g(x)=\lfloor x/2\rfloor-\lfloor(x+1)/2\rfloor$, on vérifie $g(x+2)=g(x)$. Sur $[2k,2k+1[$, $g=0$; sur $[2k+1,2k+2[$, $g=-1$. La période fondamentale est $2$.

### Exercice 4

Écrivons $x=p+u$, $y=q+v$, $z=r+w$, avec $p,q,r\in\mathbb Z$ et $u,v,w\in[0,1[$. Le système équivaut à



```math
p+q+u+w=1.1,\qquad p+r+v+w=2.2,\qquad q+r+u+v=3.3.
```



Comme chaque somme de deux parties fractionnaires appartient à $[0,2[$, on obtient



```math
A=p+q\in\{0,1\},\quad B=p+r\in\{1,2\},\quad C=q+r\in\{2,3\}.
```



De plus $A+B+C=2(p+q+r)$ est pair. Pour les quatre triplets possibles $(A,B,C)=(0,1,3),(0,2,2),(1,1,2),(1,2,3)$, les parties fractionnaires sont données par



```math
\begin{aligned}
u&=\frac{(1.1-A)+(3.3-C)-(2.2-B)}2,\\
v&=\frac{(2.2-B)+(3.3-C)-(1.1-A)}2,\\
w&=\frac{(1.1-A)+(2.2-B)-(3.3-C)}2.
\end{aligned}
```



Les trois premiers donnent respectivement $w=1$, $u=1.1$ et $v=1.2$, impossibles puisque $u,v,w<1$. Le dernier donne $(u,v,w)=(0.1,0.2,0)$. Les équations sur les parties entières donnent alors $(p,q,r)=(0,1,2)$. Ainsi l'unique solution est



```math
\boxed{(x,y,z)=(0.1,1.2,2)}.
```



### Exercice 5

1. Posons $\alpha'=(3-\sqrt{17})/2$. Alors $\alpha+\alpha'=3$, $\alpha\alpha'=-2$ et $|\alpha'|<1$. $S_n=\alpha^n+(\alpha')^n$ est entier et vérifie $S_{n+2}=3S_{n+1}+2S_n$. Comme $\alpha'<0$, pour $n$ assez grand


```math
\lfloor\alpha^n\rfloor=S_n-\mathbf1_{2\mid n}.
```


En particulier cette suite vérifie la récurrence entière d'ordre $4$ de polynôme caractéristique $(X^2-3X-2)(X^2-1)$. Attention : l'énoncé demande une récurrence d'ordre $2$; pour cette valeur de $\alpha$, c'est faux en général, car la correction $-\mathbf1_{2\mid n}$ est périodique non constante. En effet la formule comporte effectivement les quatre composantes exponentielles de bases $\alpha,\alpha',1,-1$, toutes de coefficient non nul; son polynôme minimal d'annulation est $(X^2-3X-2)(X^2-1)$, de degré $4$. Pour $n\ge1$, la récurrence donne $S_n\equiv1\pmod2$. Si $n$ est impair, on ne retranche rien, donc $\lfloor\alpha^n\rfloor$ est impair; si $n$ est pair, on retranche $1$, donc $\lfloor\alpha^n\rfloor$ est pair, comme demandé.

2. Posons $\beta'=3-\sqrt5\in(0,1)$. La somme $T_n=\beta^n+{\beta'}^n$ est entière et vérifie $T_{n+2}=6T_{n+1}-4T_n$, avec $T_0=2,T_1=6$. Comme $0<{\beta'}^n<1$, pour $n\ge1$ on a $\lfloor\beta^n\rfloor=T_n-1$. Pour calculer les trois derniers chiffres avant la virgule, il suffit donc de calculer $T_n$ modulo $1000$. On peut exponentier par dichotomie la matrice $M=\begin{pmatrix}6&-4\\1&0\end{pmatrix}$ modulo $1000$, puisque



```math
\binom{T_n}{T_{n-1}}=M^{n-1}\binom{6}{2}.
```



On renvoie le résidu de $T_n-1$ modulo $1000$, écrit sur trois chiffres.

3. Pour $\gamma=1+\sqrt2$, son conjugué $1-\sqrt2$ est de module inférieur à $1$ et $\gamma$ est racine de $X^2-2X-1$. Ainsi $\gamma^n+(1-\sqrt2)^n$ est entier et fournit, pour $n$ grand, l'entier le plus proche de $\gamma^n$. On obtient une récurrence entière d'ordre $2$ et un calcul rapide analogue.

### Exercice 6

Posons $s=\sqrt n+\sqrt{n+1}$ et $t=\sqrt{4n+2}$. On a


```math
t^2-s^2=(\sqrt{n+1}-\sqrt n)^2\in(0,1),
```


donc $s<t$. Il n'existe aucun entier $k$ dans $]s,t]$: sinon $s^2<k^2\leq t^2=4n+2$. Les deux derniers termes sont entiers et leur différence est strictement inférieure à $1$, donc $k^2=4n+2$, impossible puisque $4n+2\equiv2\pmod4$. Aucun entier ne sépare donc $s$ et $t$, et $\lfloor s\rfloor=\lfloor t\rfloor$.

## Densité

### Exercice 7

1. $\ln(1+1/n)\leq1/n$, par $\ln(1+t)\leq t$.
2. Les $\ln n$ tendent vers $+\infty$ et leurs écarts successifs tendent vers $0$. Pour tout $t$ assez grand, prenons le premier $n$ tel que $\ln n\geq t$; alors $0\leq\ln n-t\leq1/(n-1)$. Ainsi les $\ln n$ approchent tout réel arbitrairement grand, modulo $2\pi$ en particulier. La continuité de cosinus et la surjectivité de cosinus sur $[0,\pi]$ montrent que les valeurs $\cos(\ln n)$ sont denses dans $[-1,1]$.

### Exercice 8

Pour $x\geq0$, prenons $m=k^2$ et $n=k^2+\lfloor2kx\rfloor$. Alors


```math
\sqrt n-\sqrt m=\frac{n-m}{\sqrt n+k}\longrightarrow x
```


quand $k\to\infty$. Les valeurs négatives s'obtiennent en échangeant $m,n$; $0$ est obtenu avec $m=n$. L'ensemble est dense dans $\mathbb R$.

### Exercice 9

1. Tout intervalle ouvert contient $a\in A$; comme $B$ est dense, on peut choisir $b\in B$ de sorte que $a+b$ soit dans l'intervalle. Donc $A+B$ est dense.
2. Soit $(u,v)$ un intervalle ouvert. S'il contient un réel non nul $t$, choisissons $a\in A$ proche de $1$ et non nul, puis $b\in B$ proche de $t/a$; alors $ab\in(u,v)$. Si l'intervalle est autour de $0$, choisissons $a\ne0$ dans $A$ et $b$ suffisamment proche de $0$ dans $B$. Donc $AB$ est dense.

### Exercice 10

Si $H$ est dense, fixons $x\notin H$. Pour tout $y$ et $\varepsilon>0$, choisissons $h\in H$ tel que $|h-(y-x)|<\varepsilon$. Alors $x+h\notin H$ (sinon $x\in H$), et $x+h$ approche $y$. Si $H$ n'est pas dense, sa fermeture $K$ est un sous-groupe fermé strict de $\mathbb R$. Tout sous-groupe fermé strict de $\mathbb R$ est soit $\{0\}$, soit $a\mathbb Z$ : en posant $a=\inf(K\cap\mathbb R_{>0})$, le cas $a=0$ rend $K$ dense donc égal à $\mathbb R$; si $a>0$, la fermeture donne $a\in K$ et la division euclidienne montre $K=a\mathbb Z$. Or $\mathbb R\setminus K$ est dense et est inclus dans $\mathbb R\setminus H$.

### Exercice 11

Posons $\lambda=\ln2/\ln3$, irrationnel (sinon $2^q=3^p$ pour certains entiers positifs, impossible par unicité de la décomposition en facteurs premiers). Le sous-groupe $\mathbb Z+\lambda\mathbb Z$ est dense : les parties fractionnaires de $b\lambda$ sont denses modulo $1$, par le principe des tiroirs appliqué à des multiples de $\lambda$. En exponentiant $a\ln2+b\ln3$, on obtient la densité de $\{2^a3^b:a,b\in\mathbb Z\}$ dans $\mathbb R_+^*$.

### Exercice 12

1. L'image d'un ensemble dense par une application continue est dense dans l'image : appliquer cela à $\cos$ et $\sin$. La réciproque est fausse. Un contre-exemple simple est $A=\{e^{it}:t\in[0,\pi/2]\}\cup\{e^{it}:t\in[\pi,3\pi/2]\}$ : projections complètes $[-1,1]$ mais $A$ n'est pas dense dans le cercle.
2. Écrivons $\rho=\theta/(2\pi)$. Si $\rho=p/q\in\mathbb Q$, les puissances sont finies. Si $\rho$ est irrationnel, le sous-groupe $\mathbb Z\rho+\mathbb Z$ est dense modulo $1$: parmi $0,\rho,\ldots,N\rho$ deux parties fractionnaires sont à distance $<1/N$, ce qui fournit un pas non nul arbitrairement petit modulo $1$, dont les multiples approchent tout point. Les $e^{in\theta}$ sont donc denses dans $\mathbb U$.

### Exercice 13

Réglons un $\eta>0$. Si $M=\{0\}$, la conclusion vaut avec $a=0$. Sinon fixons $p\in M$, $p>0$. Pour $p,q>0$ avec $p/q$ irrationnel, les résidus de $np$ modulo $q$ sont denses dans $[0,q]$. Ils contiennent donc un $\eta$-réseau fini de résidus modulo $q$: choisissons des indices $n$ dans un ensemble fini qui réalise ce réseau. Pour tout $t$ assez grand, choisissons parmi eux un $n$ dont le résidu $np$ approche celui de $t$ modulo $q$ à moins de $\eta$, puis posons $m=\lfloor(t-np)/q\rfloor\ge0$. Alors $np+mq$ approche $t$ à moins de $\eta$. Si $p/q$ est rationnel, le monoïde engendré par $p,q$ contient tous les multiples assez grands de $d=\gcd(p,q)$ (après mise à l'échelle), donc il est $\eta$-dense à l'infini dès que $d<\eta$. Si $M$ ne contient aucun $h$ avec $0<h<\eta$, examinons les $q\in M_{>0}$. Un rapport $p/q$ irrationnel entraîne la densité à l'infini. Sinon tous les rapports sont rationnels; en écrivant $q/p=r/s$ sous forme irréductible, $d=p/s\ge\eta$ borne $s\le p/\eta$. Les dénominateurs étant bornés, leur ppcm fournit $a>0$ tel que $M\subset a\mathbb N$. Par contraposition, si $M$ n'est inclus dans aucun réseau $a\mathbb N$, il contient un $h$ avec $0<h<\eta$ pour tout $\eta>0$; les multiples de $h$ approchent tout $t$ à moins de $h$, dès que $t$ est assez grand. Ainsi $M$ est dense à l'infini. La contraposée établit l'alternative.

### Exercice 14

1. Si $P(X)=\sum_{j=0}^d c_jX^j$ s'annule en $x\ne0$, alors $(-1)^dP(-X)$ s'annule en $-x$ et $X^dP(1/X)$ s'annule en $1/x$; les coefficients restent dans $\{-1,0,1\}$.
2. Pour une racine réelle $x$ avec $|x|>1$, le terme dominant impose $|x|^d\leq\sum_{j<d}|x|^j=(|x|^d-1)/(|x|-1)$, donc $|x|<2$. Les racines de module au plus $1$ sont déjà dans l'intervalle voulu; par réciprocité on obtient en fait $A\subset[-2,2]$.
3. Soit $\beta\in(1,2)$. Définissons $r_0=1$, $\epsilon_j=\lfloor\beta r_{j-1}\rfloor\in\{0,1\}$ et $r_j=\beta r_{j-1}-\epsilon_j\in[0,1)$. Alors $1=\sum_{j=1}^N\epsilon_j\beta^{-j}+r_N\beta^{-N}$, donc $1=\sum_{j\ge1}\epsilon_j\beta^{-j}$. Posons $F_N(x)=1-\sum_{j=1}^N\epsilon_jx^{-j}$. Si l'expansion est finie, le polynôme correspondant s'annule déjà en $\beta$. Sinon, pour $N$ assez grand, au moins deux chiffres valent $1$, donc $F_N(1)<0$, tandis que $F_N(\beta)>0$; comme $F_N$ est strictement croissante sur $]1,+\infty[$, elle a une unique racine $\lambda_N\in(1,\beta)$. Pour tout $x<\beta$ assez proche de $\beta$, la série $\sum\epsilon_jx^{-j}$ dépasse $1$, donc $F_N(x)<0$ dès que $N$ est assez grand; ainsi $\lambda_N\to\beta$. En multipliant $F_N(\lambda_N)=0$ par $\lambda_N^N$, on obtient un polynôme de coefficients dans $\{-1,0,1\}$ ayant cette racine. Les transformations $x\mapsto1/x$ et $x\mapsto-x$ donnent la densité sur les autres intervalles; les extrémités suivent par fermeture.

## Bornes supérieure et inférieure

### Exercice 15

Pour $n$ pair, $u_n=1+1/n$ décroît à partir de $3/2$; pour $n$ impair, $u_n=-1+1/n$ décroît vers $-1$. Ainsi $\sup E=3/2$ (maximum en $n=2$) et $\inf E=-1$, non atteint.

### Exercice 16

Pour $n\ge2$, $|\cos n|/n\le1/2<\cos1$ (hypothèse), donc $\sup E=\cos1$, atteint en $n=1$. Pour $n\ge4$, $\cos n/n\ge-1/4$. Les séries alternées du cosinus donnent $-1<\cos3<-0.98$ et $-0.42<\cos2<-0.41$, donc $\cos3/3<-1/4$ et $\cos3/3<\cos2/2<0$; le terme $n=1$ est positif. Donc $\inf E=\cos3/3$, atteint en $n=3$.

### Exercice 17

$E=\{1-1/n-1/m\}$. Le terme est strictement inférieur à $1$ et tend vers $1$ lorsque $m,n\to\infty$, donc $\sup E=1$, non atteint. Il est minimal pour $m=n=1$, où il vaut $-1$; ainsi $\inf E=-1$, minimum.

### Exercice 18

1. $\sqrt{n+1}-\sqrt n=1/(\sqrt{n+1}+\sqrt n)\leq1/(2\sqrt n)$.
2. $E\subset[0,1)$; $0\in E$ et les parties fractionnaires $\{\sqrt n\}$ s'approchent de $1$ (prendre $n=k^2-1$), donc $\inf E=0$, minimum, et $\sup E=1$, non atteint.
3. Pour $t\in[0,1]$, prenons $n_k=\lfloor(k+t)^2\rfloor$. Alors $\sqrt{n_k}-(k)$ tend vers $t$, d'où $\{\sqrt{n_k}\}\to t$ (aux extrémités, utiliser $k^2$ et $k^2-1$). Ainsi $E$ est dense dans $[0,1]$.

### Exercice 19

Pour $x\in[a_k,a_{k+1}]$, la somme $\sum_i|x-a_i|$ est affine de pente $2k-n$; elle décroît jusqu'à une médiane et croît ensuite. Si $n=2p+1$, son minimum est atteint en $x=a_{p+1}$ et vaut $\sum_i|a_{p+1}-a_i|$. Si $n=2p$, il est atteint pour tout $x\in[a_p,a_{p+1}]$ et vaut $\sum_{i=p+1}^{2p}a_i-\sum_{i=1}^{p}a_i$.

### Exercice 20

1. Si tout $a\in A$ était $\leq0$, alors $0$ serait un majorant et $\sup A\leq0$, contradiction.
2. Non : $A=]-\infty,0[$ est majoré, de supremum $0$, sans élément positif.

### Exercice 21

1. Les majorants de $A\cup B$ sont exactement ceux qui majorent les deux ensembles; son supremum est donc $\max(\sup A,\sup B)$.
2. L'intersection est majorée par les deux suprema. Exemple $A=[0,1]$, $B=[2,3]$ n'est pas permis car disjoint; prendre $A=[0,2]$, $B=[1,3]$ donne égalité. Pour une inégalité stricte, $A=\{0,2\}$, $B=\{0,1\}$ donne $\sup(A\cap B)=0<1$.
3. $-\sup A$ est le plus grand minorant de $-A$, donc $\inf(-A)=-\sup A$.
4. La translation transporte les majorants, donc $\sup(A+\lambda)=\sup A+\lambda$.
5. $\sup A+\sup B$ majore $A+B$. Pour tout $\varepsilon>0$, choisissons $a>\sup A-\varepsilon/2$ et $b>\sup B-\varepsilon/2$; alors $a+b>\sup A+\sup B-\varepsilon$.
6. Pour $\lambda>0$, multiplier transporte le supremum : $\sup(\lambda A)=\lambda\sup A$. Si $\lambda<0$ et $A$ est minoré, $\sup(\lambda A)=\lambda\inf A$; si $A$ n'est pas minoré, $\lambda A$ n'est pas majoré. Si $\lambda=0$, $\lambda A=\{0\}$.

### Exercice 22

Comme $m=\inf A$, il existe $a\in A$ tel que $a<m+1$, donc $B\ne\varnothing$. $m$ est minorant de $B$, et tout $\varepsilon>0$ admet $a\in A$ avec $a<m+\min(\varepsilon,1)$; cet $a$ appartient à $B$. Donc $\inf B=m$.

### Exercice 23

1. Fixons $y_0\in B$, $x_0\in A$. Alors $x\le y_0$ et $y\ge x_0$; donc $A$ est majorée, $B$ minorée, et en passant aux bornes $\sup A\le\inf B$. L'égalité est possible : $A=]-\infty,0[$, $B=[0,+\infty[$.
2. Les mêmes conclusions valent; égalité aussi, par $A=]-\infty,0[$, $B=[0,+\infty[$ puisque $x<y$ pour tout couple.
3. On a $x+\varepsilon\le y$, donc $\sup A+\varepsilon\le\inf B$.

### Exercice 24

1. $|f|$ est non vide et majoré car $f$ est bornée; son supremum existe.
2. Une borne supérieure de $|f|$ vaut $0$ exactement si $|f(t)|=0$ pour tout $t$.
3. (a) $|\lambda f(t)|\le|\lambda|\|f\|_\infty$. (b) Si $\lambda\ne0$, appliquer (a) à $\lambda f$ avec $1/\lambda$ donne $\|f\|_\infty\le|1/\lambda|\|\lambda f\|_\infty$; combiner. Cas nul immédiat.
4. $|f+g|\le|f|+|g|\le\|f\|_\infty+\|g\|_\infty$.
5. $0<1/(1+x^2)\le1$, avec égalité en $x=0$, donc norme $1$.
6. $|\arctan x|<\pi/2$ et les valeurs tendent vers $\pi/2$ quand $x\to+\infty$; norme $\pi/2$.

### Exercice 25

1. Si $A$ est borné, $|x-y|$ est majoré par une constante; l'ensemble des distances est non vide, donc son supremum existe.
2. $|x-y|\le\sup A-\inf A$, donc le diamètre est au plus cette différence. Pour $\varepsilon>0$, choisissons $x\in A$ avec $x>\sup A-\varepsilon/2$ et $y\in A$ avec $y<\inf A+\varepsilon/2$. Alors $|x-y|>\sup A-\inf A-\varepsilon$.

### Exercice 26

1. Les distances sont non négatives et l'ensemble est non vide; son infimum existe.
2. Pour tout $a\in A$, $d(x,A)\le|x-a|\le|x-y|+|y-a|$. Prendre l'infimum en $a$ donne $d(x,A)\le|x-y|+d(y,A)$; échanger $x,y$.
3. Comme $x\in A$, $d(x,A)=0$. L'égalité demandée est une identité de compréhension : l'ensemble des $x\in A$ tels que $d(x,A)=0$ est précisément $A$.

### Exercice 27

1. $1\in E$, donc $E$ est non vide; il est minoré par $0$. Soit $m=\inf E$.
2. Pour $x\in E$, $m\le x$, donc $f(m)\le f(x)\le x$. Ainsi $f(m)$ minore $E$ et $f(m)\le m$.
3. Si $x\in E$, alors $f(x)\le x$; comme $f$ est croissante, $f(f(x))\le f(x)$, donc $f(x)\in E$.
4. De $f(m)\le m$ on a $m\in E$. Par (3), $f(m)\in E$, donc $m\le f(m)$. D'où $f(m)=m$.
Sur $[0,1[$ le résultat est faux : $f(x)=(x+1)/2$ est croissante et à valeurs dans $[0,1[$, mais son unique point fixe est $1$, hors du domaine.

### Exercice 28

Posons $\varphi(x)=\sup\{f(t):t\le x\}$. Cet ensemble est non vide et majoré puisque $f$ l'est. Si $x\le y$, l'ensemble définissant $\varphi(x)$ est inclus dans celui de $\varphi(y)$, donc $\varphi$ est croissante; $f(x)\le\varphi(x)$. Enfin, si $\psi$ est croissante et $f\le\psi$, alors pour $t\le x$, $f(t)\le\psi(t)\le\psi(x)$; donc $\varphi(x)\le\psi(x)$. C'est la plus petite majorante croissante, point par point.

### Exercice 29

Pour chaque $x\in[0,1]$, choisissons un intervalle ouvert $I_x$ de la famille contenant $x$. Soit $S$ l'ensemble des $t\in[0,1]$ tels que $[0,t]$ soit recouvert par un nombre fini d'intervalles de la famille. $S$ est non vide, car un intervalle couvrant $0$ couvre $[0,\eta]$ pour un certain $\eta>0$. Posons $c=\sup S$. Si $c<1$, un intervalle de la famille contenant $c$ contient $(c-\eta,c+\eta)$; par la définition du supremum, un $t\in S$ vérifie $t>c-\eta/2$. En ajoutant cet intervalle, on couvre jusqu'à $c+\eta/2$, contradiction. Donc $c=1$. Prenons maintenant un intervalle de la famille contenant $1$ et $t\in S$ assez proche de $1$; cet intervalle et le recouvrement fini de $[0,t]$ couvrent tout $[0,1]$.

### Exercice 30

Soit $S$ l'ensemble des $t\in[0,1]$ pour lesquels $[0,t]$ admet une subdivision pointée $\delta$-fine. Comme $\delta(0)>0$, un petit segment $[0,t]$ marqué en $0$ montre que $S$ est non vide. Posons $c=\sup S$. Si $c<1$, prenons $t\in S$ assez proche de $c$ et ajoutons le segment $[t,c']$ avec point marqué $c$, où $c'>c$ est choisi de sorte que $c'-t\le\delta(c)$. Cela prolonge la subdivision au-delà de $c$, contradiction. Donc $c=1$. Choisissons $t\in S$ tel que $1-t\le\delta(1)$ et ajoutons le segment $[t,1]$ marqué en $1$; on obtient une subdivision de $[0,1]$.

### Exercice 31

Posons $B=\{\ln a:a\in A\}$ et $b=\sup B=\ln(\sup A)$. Le set $B$ est stable par moyenne : si $x,y\in B$, alors $(x+y)/2\in B$. En itérant, tous les points $(1-r)u+rv$, pour $u,v\in B$ et dyadique $r\in[0,1]$, appartiennent à $B$. Les dyadiques étant denses dans $[0,1]$, $B$ est dense entre chacun de ses points. Ainsi $B$ est dense dans $[\inf B,b]$ si $\inf B$ est fini, et dans $]-\infty,b]$ si $B$ n'est pas minoré. Par exponentiation, $A$ est dense dans $[\inf A,\sup A]$ (avec $\inf A=0$ dans le second cas).

Soit $I$ un intervalle ouvert rencontrant $[\inf A,\sup A]$. Comme $A$ possède deux points distincts, on peut choisir un sous-intervalle ouvert $J\subset(\inf A,\sup A)$ inclus dans $I$. Son image logarithmique est un intervalle ouvert non vide $K\subset(\inf B,b)$. Choisissons $u<v$ dans $B$ tels que $[u,v]\subset K$. Pour tout $n$ assez grand, il existe deux fractions dyadiques consécutives $r=k/2^n$ et $r+2^{-n}$ dont les interpolés $(1-r)u+rv$ et $(1-r-2^{-n})u+(r+2^{-n})v$ restent dans $K$. Leurs exponentielles appartiennent à $A\cap I$.

Si tous les éléments de $A\cap I$ étaient rationnels, le quotient de ces deux exponentielles serait rationnel, donc $e^{(v-u)/2^n}\in\mathbb Q$ pour tout $n$ assez grand. Alors $e^{v-u}$ serait une puissance $2^n$-ième rationnelle pour des $n$ arbitrairement grands. Un rationnel positif distinct de $1$ ne peut avoir des racines rationnelles d'ordres arbitrairement grands, comme le montrent ses valuations premières; or $v>u$. Contradiction. Tout intervalle $I$ rencontre donc $A$ en un irrationnel, ce qui prouve que $A\cap(\mathbb R\setminus\mathbb Q)$ est dense dans $[\inf A,\sup A]$.
