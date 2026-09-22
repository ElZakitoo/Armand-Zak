# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td02-logique.pdf)

## Autocorrection A

(i) $\neg(P\land\neg Q)\equiv\neg P\lor Q$. (ii) $\neg((P\Rightarrow Q)\land R)\equiv(P\land\neg Q)\lor\neg R$. (iii) $\forall x\ge1,\ a<b+x$. (iv) $a,b,c$ ne sont pas tous égaux.

## Autocorrection B



```math
\forall x\in\mathbb R_+,\ \exists y\in\mathbb R:\ x=y^2.
```



## Exercice 1

(i) $\forall n,\ u_n=0$; négation: $\exists n,\ u_n\ne0$. (ii) $\forall n,\ u_n\le u_{n+1}$; négation: $\exists n,\ u_n>u_{n+1}$. (iii) $\forall n,\ u_n>u_{n+1}$; négation: $\exists n,\ u_n\le u_{n+1}$. (iv) $\forall n,\ u_n<2$; négation: $\exists n,\ u_n\ge2$. (v) $\exists C\in\mathbb R,\forall n,\ u_n<C$; négation: $\forall C,\exists n,\ u_n\ge C$. (vi) $\exists N,\forall n\ge N,\ u_n=u_N$; négation: $\forall N,\exists n\ge N,\ u_n\ne u_N$. (vii) $\exists m,M,\forall n,\ m\le u_n\le M$; négation: $\forall m,M,\exists n,\ u_n<m\lor u_n>M$. (viii) $\exists n,\ u_n=0$; négation: $\forall n,\ u_n\ne0$. (ix) $\forall n\ne m,\ u_n\ne0\lor u_m\ne0$; négation: $\exists n\ne m,\ u_n=u_m=0$.

## Exercice 2

(i) $(\neg P\Rightarrow P)$ vaut $P$ (si $P$ est faux, l’implication est fausse; si $P$ est vrai, elle est vraie). (ii) Si $P$ est faux, l’implication est vraie; si $P$ est vrai, $Q\Rightarrow P$ est vraie. (iii) les deux implications sont fausses exactement lorsque $P$ est vraie et $Q$ fausse. (iv) les deux côtés signifient que $P,Q$ ont la même valeur de vérité. (v) si $H_1\lor H_2$ est vrai, l’une des implications fournit $P$. (vi) si l’antécédent est vrai, $P\Rightarrow(Q\Rightarrow R)$ et $(P\Rightarrow Q)$ sont vrais; pour $P$ vrai, ils imposent successivement $Q$ puis $R$, donc $P\Rightarrow R$. Dans tous les autres cas l’implication globale est vraie.

## Exercice 3

1. $P\lor Q\equiv\neg(\neg P\land\neg Q)$ (De Morgan).
2. $P\Rightarrow Q\equiv\neg(P\land\neg Q)$; $P\Leftrightarrow Q\equiv\neg(P\land\neg Q)\land\neg(Q\land\neg P)$.

## Exercice 4

Par définition $P\uparrow Q=\neg(P\land Q)$.
(i) $P\uparrow P=\neg P$.
(ii) $(P\uparrow Q)\uparrow(P\uparrow Q)=P\land Q$.
(iii) $(P\uparrow P)\uparrow(Q\uparrow Q)=P\lor Q$.
(iv) $P\Rightarrow Q=P\uparrow(Q\uparrow Q)$.
(v) $(P\uparrow(Q\uparrow Q))\uparrow(Q\uparrow(P\uparrow P))$ est la négation de $(P\Rightarrow Q)\land(Q\Rightarrow P)$, donc ce n’est pas l’équivalence; l’équivalence s’écrit en Sheffer comme $[(P\uparrow(Q\uparrow Q))\uparrow(Q\uparrow(P\uparrow P))]\uparrow[(P\uparrow(Q\uparrow Q))\uparrow(Q\uparrow(P\uparrow P))]$.

## Exercice 5

Retourner A et 1. A doit avoir un nombre pair derrière; la carte 1 ne doit pas avoir une voyelle au verso. B peut avoir un nombre pair ou impair; 2 peut avoir voyelle ou consonne sans enfreindre la règle.

## Exercice 6

Le premier compliment porte sans restriction sur la qualité du chant: jamais personne n’a mieux chanté ce rôle. Le second restreint la comparaison aux cantatrices aussi jeunes et aux cheveux aussi beaux; il est donc moins fort sur le chant, même s’il loue aussi l’âge et la beauté.

## Autocorrection C

Pour tout $x$, prendre $y=x-1$.

## Autocorrection D

Prendre $x=0$; pour tout $y\in[0,1]$, $0\le y$.

## Exercice 7

(i) Faux: antécédent vrai, conséquent faux. (ii) Vrai: l’antécédent est faux. (iii) Vrai par implication à antécédent faux. (iv) Faux, $x=5/2$ contredit la conclusion. (v) Faux: $x=-1,y=1$ donnent $x<y$ mais $1/x=-1<1=1/y$. (vi) $n^3-n=n(n-1)(n+1)$ est pair, car trois entiers consécutifs comprennent un pair. (vii) Vrai, $x=1/4$ vérifie $0<x<\sqrt x$. (viii) Faux: les zéros de cosinus sont $\pi/2+k\pi$, donc plusieurs. (ix) Faux: si $x=e^{-x}$, alors $x>0$ et $x<1$; cela contredit $x\le x^2$. (x) Vrai: choisir $m=0$ si $n$ impair, $m=1$ si $n$ pair. (xi) Faux, $n=0$ suffit. (xii) Faux: pour tout $\eta>0$, choisir $x<-\eta-2$ donne $x\le\eta$ et $x^2>1$. (xiii) Vrai avec $\eta=1$. (xiv) Vrai avec $\eta=10^{-9}$. (xv) Vrai, choisir $\eta=\sqrt\epsilon$.

## Exercice 8

(i) Fausse; négation: $\exists x,y, x+y\le0$. (ii) Vraie: prendre $y=1-x$. (iii) Fausse; sa négation est $\forall x,\exists y, x+y\le0$; pour chaque $x$, prendre $y=-x$. (iv) Vraie, par exemple $x=1,y=1$. (v) Vraie: prendre $m=0$ si $n$ pair, $m=1$ si $n$ impair. (vi) Fausse; sa négation est $\forall n,\exists m, n+m$ impair; prendre $m$ de parité opposée à $n$. (vii) Vraie: pour $y>0$, prendre $x=\ln y$. (viii) Fausse: $e^x$ n’est pas constant; par exemple $e^0\ne e^1$. Négation: $\forall y>0,\exists x, y\ne e^x$.

## Exercice 9

(i) Fausse: $x=1,y=0$; négation $\exists x,y, xy=0\land x\ne0$. (ii) Vraie si la formule est $xy=0\Rightarrow(x=0\lor y=0)$; l’annulation d’un produit impose l’annulation d’au moins un facteur. (iii) Vraie, tout entier vérifie $n\ge0$ ou $n\le0$. (iv) Fausse: ni tous les entiers ne sont positifs, ni tous négatifs.

## Exercice 10

(i) Contraposée / raisonnement par l’absurde. (ii) Contraposée du principe des zéros isolés (supposer une infinité de zéros et en déduire que $f$ est identiquement nulle). (iii) Réduction aux cas $n\le0$ et $n\ge1$ (disjonction de cas; le texte n’en donne ensuite qu’un cas). (iv) Disjonction selon que le groupe est infini ou fini. (v) Double implication, preuve directe dans chaque sens.

## Exercice 11

1. Si $N\ge7$ est impair, $N-3\ge4$ est pair. Par Goldbach forte, $N-3=p+q$ avec $p,q$ premiers; alors $N=p+q+3$ est somme de trois premiers.
2. La faible vraie n’implique pas la forte: la réciproque logique ne suit pas. On ne peut rien conclure sur la conjecture forte par cette seule implication.

## Exercice 12

Si $x+y>2$ et si tous deux étaient $\le1$, leur somme serait $\le2$; donc $x>1$ ou $y>1$. La réciproque précise est $(x>1\lor y>1)\Rightarrow x+y>2$. Elle est fausse: $x=2,y=-1$.

## Exercice 13+

Si $A>B$, choisir $\epsilon=(A-B)/2>0$ donne $B+\epsilon<A$, contradiction. Donc $A\le B$.

## Exercice 14+

(i)$\Rightarrow$(ii): appliquer (i) à $A+1$ donne $u_n\ge A+1>A$. (ii)$\Rightarrow$(i): appliquer (ii) à $A$ donne $u_n>A$, donc $u_n\ge A$.

## Exercice 15

Si $f$ est strictement croissante, $a\le b$ entraîne $f(a)\le f(b)$. Si $f(a)\le f(b)$, alors $a>b$ est impossible par croissance stricte; donc $a\le b$. Inversement, supposons l’équivalence vraie. Pour $a<b$, elle donne $f(a)\le f(b)$; l’égalité impliquerait aussi $f(b)\le f(a)$, donc $b\le a$, contradiction. Ainsi $f(a)<f(b)$.

## Exercice 16

1. (i)$\Rightarrow$(ii) car les deux valeurs valent $y_0$. (ii)$\Rightarrow$(i), fixer $x_0$ et prendre $y_0=f(x_0)$. Ce sont les définitions de fonction constante.
2. Si $f$ est croissante et décroissante et $x<y$, alors $f(x)\le f(y)$ et $f(x)\ge f(y)$; donc égalité. Cela donne (i) en fixant $x_0$, et (ii) directement pour $x_1<x_2$, avec échange des indices si besoin.

## Exercice 17+

Si $ax+b\ge0$ pour $0<x<1$, passage à la limite quand $x\to0^+$ puis $x\to1^-$ donne $b\ge0$ et $a+b\ge0$. Réciproquement $ax+b=(1-x)b+x(a+b)\ge0$ pour $0<x<1$.

## Exercice 18

1. (a) En $x=y=0$, $f(0)=f(0)^2-f(0)^2=0$. (b) En $x=0$, $y^2+f(0)=f(y)^2-f(0)f(y)$, donc $f(y)^2=y^2$ et $f(y)\in\{-y,y\}$. (c) En $y=1$, l’équation devient $xf(x)+1+f(x)=f(x+1)^2-f(x)f(1)$. De $x=1,y=1$ on obtient $f(1)=1$. Puis $x=1$ donne $f(y)+y^2+1=(y+1)^2-f(y)$, donc $2f(y)=2y$ et $f(y)=y$.
2. La fonction identité vérifie les deux membres: $x^2+y^2+xy=(x+y)^2-xy$. Elle est l’unique solution.

## Exercice 19

Prendre $x=y=1$ donne $f(1)=2f(1)$, donc $f(1)=0$. Prendre $x=0,y=1$ donne $f(0)=f(0)+f(1)$ (tautologie); pour isoler $f(x)$, prendre $y=0$: $f(0)=f(x)+f(0)$, d’où $f(x)=0$ pour tout $x$. La fonction nulle convient.

## Exercice 20+

$n=0$ impose $x^2\le x+1$, donc $x\in[-1/\varphi,\varphi]$, avec $\varphi=(1+\sqrt5)/2$. Si $x\ge0$, la condition pour tout $n$ équivaut à $x^2\le x+1$, donc $x\in[0,\varphi]$. Si $x=-t<0$, les cas $n$ pair et impair imposent respectivement $t^2\le1-t$ et $t^2\ge1-t$; ensemble, $t=1/\varphi$. Ainsi $x\in\{ -1/\varphi\}\cup[0,\varphi]$.

## Exercice 21

Si $n$ est pair, prendre $m=1$; si $n$ est impair, prendre $m=2$. La somme est impaire et le produit pair.

## Exercice 22

$x^2-x=x(x-1)\ge0$; le produit est positif si $x\le0$ ou $x\ge1$.

## Exercice 23

Si $x\notin\mathbb Q$, la première branche est vraie. Sinon $x=p/q$ avec $p\in\mathbb Z$, $q\in\mathbb N^*$; prendre $n=q$ donne $nx=p\in\mathbb Z$.

## Autocorrection E

Les premières sommes sont $1,4,9,16$; conjecture $\sum_{k=1}^n(2k-1)=n^2$. Initialisation $n=1$. Si la somme vaut $n^2$, ajouter $2n+1$ donne $(n+1)^2$.

## Autocorrection F

Initialement $3^0-2^0=0$ et $3^1-2^1=1$. Si $u_n=3^n-2^n$ et $u_{n+1}=3^{n+1}-2^{n+1}$, alors
$5u_{n+1}-6u_n=3^{n+2}-2^{n+2}$. Par récurrence, la formule est vraie.

## Exercice 24

Initialisation $n=1$: égalité. Si $(1+x)^n\ge1+nx$, alors
$(1+x)^{n+1}\ge(1+nx)(1+x)=1+(n+1)x+nx^2\ge1+(n+1)x$.

## Exercice 25

1. Par binôme, $(3+2\sqrt2)^n=a_n+b_n\sqrt2$ avec $a_n,b_n\in\mathbb N$.
2. Le conjugué vaut $(3-2\sqrt2)^n=a_n-b_n\sqrt2$.
3. Le produit des deux puissances vaut $1$, donc $a_n^2-2b_n^2=1$. Comme $a_n$ croît strictement, ces couples sont distincts pour tous $n\ge1$.

## Exercice 26+

Initialiser avec $12=3\cdot4$, $13=2\cdot4+5$, $14=4+2\cdot5$, $15=3\cdot5$. Si $n=4a+5b$ pour $n\ge12$, alors $n+4=4(a+1)+5b$. Récurrence par pas de 4, avec les quatre bases couvrant les classes modulo 4.

## Exercice 27+

0. La première assertion autorise un choix distinct de $a_i$ pour chaque $n$; la seconde exige une même suite compatible pour tous les préfixes. La seconde implique la première, la réciproque ne découle pas de la seule quantification.
1. Pour $n=1$, prendre $a_1=1$. Pour $n\ge2$, posons $t_i=1/n$ pour $1\le i<n$ et $s=\sum_{i<n}t_i^2=(n-1)/n^2<1$. Le vecteur rationnel


```math
\left(\frac{2t_1}{1+s},\ldots,\frac{2t_{n-1}}{1+s},\frac{1-s}{1+s}\right)
```


a des coordonnées strictement positives et de norme $1$, puisque $4s+(1-s)^2=(1+s)^2$. En multipliant ses coordonnées par un dénominateur commun $D$, on obtient des entiers positifs $a_i$ vérifiant $\sum a_i^2=D^2$.
2. Poser $a_1=3$, $q_1=3$ et, pour $n\ge1$, $a_{n+1}=(q_n^2-1)/2$, $q_{n+1}=(q_n^2+1)/2$. Les $q_n$ restent impairs, et $q_n^2+a_{n+1}^2=q_{n+1}^2$. Ainsi les préfixes ont pour sommes $q_n^2$; les premiers termes sont $3,4,12,84,\ldots$.
   
## Exercice 28

L’hérédité échoue pour $n=1$: les deux familles de taille $1$ sont $u_1$ et $u_2$, sans élément commun. On ne peut pas déduire $u_1=u_2$ par transitivité; l’intersection des deux sous-familles, essentielle à l’argument, est vide à cette étape.

## Exercice 29++

Si $n$ est pair, le cycle est biparti et chaque route change de classe de parité. Après toute suite d’instructions, les images des deux classes restent de parités opposées: elles ne peuvent être toutes confondues.

Soit $n$ impair, $V=\{0,\ldots,n-1\}$, les villes étant numérotées dans l’ordre du cycle. Poser


```math
a(k)=k+1\ (0\leq k<n-1),\qquad a(n-1)=n-2,
```




```math
b(0)=n-1,\qquad b(k)=k-1\ (1\leq k\leq n-2),\qquad b(n-1)=0.
```


À chaque ville, les deux routes vont vers ses deux voisins. Sous $a$, toute ville atteint le cycle $n-2\leftrightarrow n-1$ en au plus $n-2$ étapes. Ainsi


```math
a^{n-2}(V)=\{n-2,n-1\}.
```


Sous $b$, $n-2$ descend jusqu’à $0$ en $n-2$ étapes, et $0\leftrightarrow n-1$ est un cycle de longueur $2$. Comme $n-2$ est impair,


```math
b^{n-2}(n-2)=b^{n-2}(n-1)=0.
```


Le mot $a^{n-2}b^{n-2}$ mène donc toutes les villes à $0$. Les valeurs possibles sont exactement les $n$ impairs.

## Exercice 30+

1. Récurrence: déplacer les $n-1$ petits disques du piquet 1 au 2, le grand du 1 au 3, puis les $n-1$ petits du 2 au 3.
2. Si $T_n$ est le minimum, $T_n=2T_{n-1}+1$, $T_0=0$. Donc $T_n=2^n-1$. Le grand disque doit bouger une fois, et avant/après son déplacement les $n-1$ autres doivent être déplacés entièrement, ce qui donne aussi la borne inférieure.

## Exercice 31+

Noter $g_i$ le gain d’essence sur le tronçon suivant le dépôt $i$; $\sum g_i=0$. Poser $S_0=0$, $S_k=\sum_{i=1}^k g_i$, et choisir le dépôt suivant un indice où $S_k$ est minimal (ou le dépôt initial si le minimum est $S_0$). Tout cumul partiel du tour depuis ce point est non négatif; le réservoir ne devient jamais négatif.

## Exercice 32++

1. Insertion inductive: pour un chemin hamiltonien $E_1\to\cdots\to E_k$, insérer la nouvelle équipe à un endroit convenable; si elle bat $E_1$, la placer devant; sinon, si $E_k$ la bat, la placer après; autrement prendre le premier indice $i$ tel que $E_i$ bat la nouvelle et la nouvelle bat $E_{i+1}$.
2. Chaque équipe gagne $(n-1)/2$ matchs dans un tournoi équilibré, donc $n$ impair. Réciproquement, pour $n=2k+1$, numéroter modulo $n$ et faire battre par $i$ les équipes $i+1,\ldots,i+k$. Chacune gagne et perd $k$ matchs.

## Exercice 33

1. $\forall M\in\mathbb R,\exists x\in\mathbb R:|f(x)|>M$ (ou prendre $M\ge0$).
2. $f(x)=\sin x$ est bornée par 1; $f(x)=x$ ne l’est pas car choisir $x>M$.
3. Toutes les fonctions $\mathbb R\to\mathbb R$: pour chaque $x$, prendre $M=|f(x)|$.
4. Si $|f(x)|\le M$, prendre $a=-M,b=M$; réciproquement $a\le f(x)\le b$ donne $|f(x)|\le\max(|a|,|b|)$.
5. Si $|f|\le M$, alors $-2M\le f(x)-f(y)\le2M$. Réciproquement, fixer $y=0$: $a+f(0)\le f(x)\le b+f(0)$, donc $f$ bornée.

## Exercice 34

1. $(f+g)(x+T)=f(x)+g(x)$.
2. $f(x)=\sin(2\pi x/T)$ convient.
3. Appliquer deux fois la période $T$.
4. Réciproque fausse: $\sin(\pi x/T)$ est $2T$-périodique mais pas $T$-périodique.
5. Répéter l’égalité $n$ fois.
6. (a) Pour $0\le x\le T$, croissance et périodicité donnent $f(0)\le f(x)\le f(T)=f(0)$, donc constante. (b) Répéter l’argument ou utiliser $f(x+kT)=f(x)$ et la croissance pour chaque intervalle de longueur $T$. (c) Pour tout réel $x$, choisir $n$ avec $x\in[0,nT]$ après translation de période; alors $f(x)=f(0)$.

## Exercice 35+

1. Si $u_n$ croît, pour tout $m\ge n$, $u_m\ge u_n$; prendre $M=n$.
2. Pour les deux suites, prendre le maximum des deux seuils $M_1,M_2$; au-delà les deux termes sont au moins leurs termes de rang fixé, donc leur somme aussi.
3. Pour $n$ pair, tout rang impair $m$ arbitrairement grand vérifie $(-1)^m=-1<1=(-1)^n$; la condition pseudo-croissante échoue.
4. $v_n=n+(-1)^n$ n’est pas croissante car $v_0=1>v_1=0$. Elle est pseudo-croissante car $v_m\ge m-1\to+\infty$.
5. (a) Fixer $k$, appliquer les deux propriétés et prendre le plus grand des seuils; alors simultanément $u_n\ge u_k$ et $u_n\le u_k$. (b) Pour $i,j$, prendre $N$ supérieur aux seuils associés aux valeurs $u_i,u_j$; choisir $n\ge N$ donne $u_i=u_n=u_j$.

## Exercice 36+

1. $1,1,2,3,5,8,13,21,34,55$.
2. Un pavage commence soit par un domino vertical (reste $2\times(n-1)$), soit par deux horizontaux superposés (reste $2\times(n-2)$). Le nombre $P_n$ vérifie $P_n=P_{n-1}+P_{n-2}$, $P_1=1,P_2=2$, donc $P_n=F_{n+1}$.
3. Fixer $m$ et récurrer sur $n$ avec $F_{n+m}=F_{n+m-1}+F_{n+m-2}$; la formule suit des récurrences de Fibonacci et des cas $n=2,3$.
4. L’identité de Cassini est $F_n^2-F_{n-1}F_{n+1}=(-1)^{n+1}$. Elle se démontre par récurrence: $F_{n+1}^2-F_nF_{n+2}=F_{n+1}F_{n-1}-F_n^2$, donc le signe alterne.
5. Posons $S_m=\sum_{k=1}^m F_kF_{k+1}$. Par induction, $S_{2n-1}=F_{2n}^2$: le passage de $n$ à $n+1$ ajoute $F_{2n+1}(F_{2n}+F_{2n+2})=F_{2n+2}^2-F_{2n}^2$. Puis $S_{2n}=F_{2n}^2+F_{2n}F_{2n+1}=F_{2n}F_{2n+2}=F_{2n+1}^2-1$, par Cassini.
