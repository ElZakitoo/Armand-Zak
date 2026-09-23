# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td09-relations.pdf)

## Exercice 1

1. La relation $R^*$ contient $R$ (chaînes de longueur 1) et est réflexive (chaîne de longueur 0) et transitive (concaténation des chaînes). Si $R=R^*$, elle est réflexive et transitive. Réciproquement, si $R$ possède ces deux propriétés, toute chaîne $x=x_0Rx_1R\cdots Rx_n=y$ implique $xRy$ par récurrence; donc $R^*=R$.
2. Si $R$ est symétrique, inverser une chaîne prouve la symétrie de $R^*$. Avec sa réflexivité et sa transitivité, $R^*$ est une équivalence.
3. Une chaîne ajoute au plus un élément à chaque étape. Donc


```math
A R^* B\iff A\subseteq B\text{ et }B\setminus A\text{ est fini}.
```



## Exercice 2

Posons


```math
R_s=R\cap R^{-1},\qquad R_a=R^{-1}\setminus R.
```


Alors $R_s$ est symétrique. Si $xR_a y$ et $yR_a x$, on aurait $yRx$ et non $xRy$, ainsi que $xRy$ et non $yRx$, contradiction; $R_a$ est antisymétrique. Enfin $xRy$ ssi $xR_s y$ ou $yR_a x$. Le couple est unique : un couple mutualisé doit appartenir à $R_s$; une paire de $R$ dans un seul sens ne peut appartenir à $R_s$ et impose l'orientation de $R_a$.

## Autocorrection A

(i) Pas un ordre : $x\not\preceq x$. (ii) C'est un ordre partiel, non total : $x\preceq y\iff x=y$ ou $x+1\le y$. Aucun minimum ni maximum; les minimaux sont $[0,1[$, aucun maximal. (iii) Pas un ordre : antisymétrie et transitivité échouent, par exemple $2\preceq1$ et $1\preceq2$, mais $2\ne1$. (iv) Sur les nombres premiers, la divisibilité est l'égalité : ordre partiel non total; il n'y a ni minimum ni maximum, et chaque premier est minimal et maximal. (v) L'inclusion sur les parties finies est un ordre partiel, non total; minimum et unique élément minimal : $\varnothing$; aucun maximum ni élément maximal. (vi) La comparaison des cardinaux est réflexive, transitive, totale, mais non antisymétrique : ce n'est pas un ordre. (vii) L'ordre ponctuel est partiel, non total; minimum et unique minimal : la fonction nulle; aucun maximum ni maximal. (viii) La relation «il existe un $x$ tel que $f(x)\le g(x)$» n'est pas un ordre : elle n'est pas antisymétrique. (ix) La comparaison éventuelle est réflexive et transitive, mais non antisymétrique; elle n'est pas totale, par exemple $f(x)=2+\sin x$ et $g(x)=2-\sin x$ se croisent infiniment souvent. Son minimum est la fonction nulle, elle n'a pas de maximum ni d'élément maximal; ses éléments minimaux sont les fonctions nulles à partir d'un certain seuil.

## Exercice 3

1. Sur $\mathbb C$, la relation est réflexive et transitive puisque les exposants $2^n$ se composent. Elle n'est pas antisymétrique : pour $\omega=e^{2i\pi/3}$, on a $\omega^2=\omega^{2^1}$ et $(\omega^2)^2=\omega$, avec $\omega\ne\omega^2$. Ce n'est pas un ordre.
2. Sur $\mathbb R$, la relation est un ordre. Si $y=x^{2^m}$ et $x=y^{2^n}$, alors $x=x^{2^{m+n}}$. Si $m+n>0$, les seules solutions réelles sont $x=0$ ou $x=1$, d'où $x=y$; si $m+n=0$, alors $m=n=0$ et aussi $x=y$. Réflexivité et transitivité suivent des exposants.
3. $A=\{2,3\}$ n'a pas de majorant : tout majorant $z$ devrait être à la fois une puissance itérée de 2 et une puissance itérée de 3, ce qui contredit l'unicité de la décomposition en facteurs premiers.

## Exercice 4

1. La relation est réflexive. Si $(I,f)\preceq(J,g)$ et $(J,g)\preceq(I,f)$, alors $I=J$ et $f=g$; elle est antisymétrique. Enfin, si $(I,f)\preceq(J,g)\preceq(K,h)$, alors $I\subseteq K$ et $h|_I=g|_I=f$, d'où la transitivité.
2. Pour une chaîne $\mathcal C$, posons $U=\bigcup_{(I,f)\in\mathcal C}I$ et $h=\bigcup_{(I,f)\in\mathcal C}f$. La propriété de chaîne assure la compatibilité des fonctions sur les intersections; $h:U\to\mathbb R$ est une fonction et chaque élément de $\mathcal C$ est inférieur à $(U,h)$.

## Exercice 5+

1. $\{1\}$ est une antichaîne maximale, car 1 est comparable à tout élément; elle est de cardinal minimal possible.
2. Pour chaque impair $q\le2n$, les nombres $q,2q,4q,\ldots\le2n$ forment une chaîne. Ces chaînes partitionnent $[1,2n]$; il y en a (n), donc toute antichaîne a au plus (n) éléments. L'ensemble $\{n+1,\ldots,2n\}$ est une antichaîne de cardinal $n$, car le double de chacun de ses éléments dépasse $2n$.

## Exercice 6+

1. Si $m=\max A$, alors $m$ majore $A$; tout majorant de $A$ majore $m$. Ainsi $\sup A=m$.
2. Pour tout $a\in A$, $a\le\sup A$, donc $f(a)\le f(\sup A)$. Cette dernière valeur majore $f[A]$; par minimalité de sa borne supérieure, $\sup(f[A])\le f(\sup A)$.
3. (i) Dans $\mathbb R$, $\sup(]0,1])=1$, $\inf(]0,1])=0$. (ii) Pour la divisibilité dans $\mathbb N$, $\sup\{12,8\}=24$, $\inf\{12,8\}=4$. (iii) Pour $\mathbb N=\{0,1,\ldots\}$ et $A=\{2^n:n\in\mathbb N\}$, on a $\sup A=0$ car tout entier divise 0, et $\inf A=1$ car $1\in A$. (iv) Dans $\mathbb N^*$, $A$ n'a pas de majorant divisible par toutes les puissances de 2; son infimum est 1. (v) Pour $f_a(x)=2a(x-a)+a^2=2ax-a^2$, $\sup_a f_a(x)=x^2$ puisque $x^2-f_a(x)=(x-a)^2$. Donc $\sup A$ est la fonction $x\mapsto x^2$. Aucune borne inférieure réelle à valeurs réelles n'existe, puisque $f_a(0)=-a^2\to-\infty$.
4. Dans $(\mathcal P(\Omega),\subseteq)$, l'infimum d'une famille est son intersection et son supremum son union.
5. L'intersection $X_1\cap X_2$ est stable par somme, donc c'est l'infimum. Le supremum est l'ensemble des sommes finies non vides d'éléments de $X_1\cup X_2$ : il contient les deux ensembles, est stable par somme et est inclus dans tout ensemble stable contenant les deux.

## Exercice 7

1. En partant d'un élément et en descendant tant qu'un élément strictement inférieur existe, la finitude interdit une descente infinie; le dernier élément est minimal. Le dual donne un maximal.
2. Si $x$ est minimal et $y\le f(x)$, alors $f^{-1}(y)\le x$, donc $f^{-1}(y)=x$ et $y=f(x)$. Le raisonnement dual vaut pour les maximaux.
3. (a) Pour trois éléments, les cinq types sont : antichaîne; chaîne; un seul lien et un élément isolé; un minimum sous deux éléments incomparables; deux éléments incomparables sous un maximum.
(b) Les 16 types, à isomorphisme près, sont représentés par les ensembles de couvertures suivants (une flèche indique une couverture) :


```math
\begin{array}{ll}
\varnothing;&1\to2;\\
1\to2,\ 3\to4;&1\to2\to3\quad$4\text{ isolé}$;\\
1\to2,\ 1\to3\quad$4\text{ isolé}$;&1\to3,\ 2\to3\quad$4\text{ isolé}$;\\
1\to2\to3\to4;&1\to2,\ 1\to3,\ 1\to4;\\
2\to1,\ 3\to1,\ 4\to1;&1\to2,\ 2\to3,\ 2\to4;\\
1\to2,\ 3\to2,\ 4\to2;&1\to2,\ 2\to3,\ 1\to4;\\
2\to1,\ 3\to2,\ 4\to1;&1\to2,\ 3\to2,\ 3\to4;\\
1\to2,\ 1\to3,\ 2\to4,\ 3\to4;&1\to3,\ 1\to4,\ 2\to3,\ 2\to4.
\end{array}
```


## Exercice 8

1. (a) Si $x\ne y$, la totalité donne $x\prec y$ ou $y\prec x$; la stricte croissance impose des images distinctes. (b) Si $f(x)\prec f(y)$, alors $y\preceq x$ donnerait soit $x=y$, impossible par l'injectivité, soit $y\prec x$, contredisant la croissance stricte. Donc $x\prec y$ et $f^{-1}$ est strictement croissante.
2. Pour l'injectivité, une application constante d'un ensemble à deux éléments incomparable vers un singleton est strictement croissante au sens vide et non injective. Pour l'inverse, l'identité de l'antichaîne à deux éléments vers une chaîne à deux éléments (bijection choisie) est strictement croissante, mais son inverse ne l'est pas.
3. Si $x\le y$, alors $\downarrow x\subseteq\downarrow y$. Si $x<y$, $y\in\downarrow y\setminus\downarrow x$, donc l'inclusion est stricte. L'application $x\mapsto\downarrow x$ est strictement croissante et injective.

## Exercice 9+

1. Définissons $x\preceq y$ si $x\preceq_0 y$ ou si $x\preceq_0 a$ et $b\preceq_0 y$, où $\preceq_0$ est l'ordre initial. Cette relation est réflexive et transitive. Un cycle faisant intervenir une nouvelle comparaison donnerait $b\preceq_0 a$, impossible puisque $a,b$ sont incomparables; elle est donc antisymétrique et vérifie $a\preceq b$.
2. En ajoutant successivement une comparaison entre deux éléments incomparables via 1, on obtient un ordre total prolongeant $\preceq$ (le processus finit, car $E$ est fini). Pour chaque paire ordonnée $(x,y)$ telle que $x\not\preceq y$, choisir un ordre total prolongeant $\preceq$ et vérifiant $y<x$; si $y\preceq x$, tout prolongement convient, sinon on l'obtient par 1. L'intersection de ces ordres totaux vaut $\preceq$.
3. (a) Pour chaque entier $i$ entre $1$ et $n$, ordonner lexicographiquement les vecteurs indicateurs des parties, en plaçant la coordonnée $i$ en premier et en fixant un ordre sur les autres, avec $0<1$. Chaque ordre total respecte l'inclusion. Si $A\not\subseteq B$, un $i\in A\setminus B$ donne $B<A$ dans l'ordre correspondant. L'intersection de ces $n$ ordres est exactement la relation d'inclusion : toute inclusion les respecte, et toute non-inclusion est séparée par l'ordre associé à un indice de différence. Cela prouve bien les deux inclusions entre la relation donnée et l'intersection construite.
(b) Pour $i\in[1,n]$, posons $A_i=[1,n]\setminus\{i\}$, $B_i=\{i\}$. La réalisation doit contenir, pour chaque $i$, un ordre total avec $B_i>A_i$. Un même ordre ne peut satisfaire cela pour deux indices distincts $i,j$: les singletons vérifient $\{j\}\subset A_i$ et $\{i\}\subset A_j$, ce qui imposerait simultanément $\{i\}>\{j\}$ et $\{j\}>\{i\}$. Il faut donc au moins $n$ ordres.

## Autocorrection B

(i) Réflexive et symétrique, mais non transitive. Pour $n=2$, prendre $x=(0,0)$, $y=(0,1)$, $z=(1,1)$. Pour $n>2$, compléter ces triplets par $x_i=0$, $y_i=2$, $z_i=1$ pour $i\ge3$. Dans chaque cas, $x=^*y$ et $y=^*z$, mais $x$ et $z$ ne sont pas en relation. (ii) C'est une équivalence, car les matrices inversibles contiennent l'identité et sont stables par inverse et produit. (iii) L'égalité à partir d'un rang est une équivalence. (iv) La limite $u_n/v_n\to1$ est réflexive, symétrique par inversion, transitive par produit. (v) La disjonction n'est pas réflexive, sauf sur l'ensemble vide. (vi) L'intersection non vide n'est pas réflexive sur l'ensemble vide et n'est pas transitive: $\{0\}$ intersecte $\{0,1\}$, et $\{0,1\}$ intersecte $\{1\}$, mais $\{0\}$ et $\{1\}$ sont disjoints. (vii) La comparabilité par inclusion est réflexive et symétrique, mais non transitive: $\{1\}\subset\{1,2\}\supset\{2\}$. (viii) L'équipotence est une équivalence.

## Exercice 10

L'égalité $z_1^n=z_2^n$ est une équivalence. Si $z=0$, sa classe est $\{0\}$. Si $z\ne0$, $w^n=z^n$ équivaut à $w=z\zeta$ avec $\zeta^n=1$; la classe contient exactement $n$ éléments.

## Exercice 11

1. $X\cup A=Y\cup A$ est une égalité d'images par $X\mapsto X\cup A$, donc définit une équivalence.
2. Les classes sont indexées exactement par les sous-ensembles de $E\setminus A$, puisque $X\cup A=A\cup(X\setminus A)$. Il y en a $2^{|E\setminus A|}$.

## Exercice 12+

Pour $x,y\in\mathbb R$, choisissons $m\in\mathbb N$ tel que $|x-y|/m\le\varepsilon$. Les points $x+k(y-x)/m$ successifs sont à distance au plus $\varepsilon$, donc tous équivalents par transitivité. Ainsi tous les réels sont équivalents : $\approx=\mathbb R^2$.

## Exercice 13+

La condition nécessaire et suffisante est : $\mathcal F\ne\varnothing$ et, pour tous $A,B\in\mathcal F$, il existe $C\in\mathcal F$ tel que $C\subseteq A\cap B$. La réflexivité équivaut à $\mathcal F\ne\varnothing$; la symétrie est automatique. Cette condition implique la transitivité. Réciproquement, supposons qu'aucun $C\in\mathcal F$ soit inclus dans $A\cap B$. Définissons $g=0$, $f=1$ sur $B\setminus A$ et $0$ ailleurs, et $h=0$ sur $B$, $1$ ailleurs. Alors $f=g$ sur $A$ et $g=h$ sur $B$, mais $f$ et $h$ diffèrent en tout point hors de $A\cap B$. Donc elles ne coïncident sur aucun $C\in\mathcal F$, contradiction à la transitivité.

## Exercice 14

1. La relation signifie que la différence symétrique $A\triangle B$ est finie. Cette propriété est réflexive, symétrique et transitive.
2. $[\varnothing]$ est l'ensemble des parties finies de $\mathbb N$; $[\mathbb N]$ est l'ensemble des parties cofinites.
3. Soit $A_i=\{2^i(2k+1):k\in\mathbb N\}$, pour $i\in\mathbb N$. Ces ensembles sont disjoints et infinis; deux distincts ont donc une différence symétrique infinie.
4. Notons $T$ l'ensemble des mots binaires finis, dénombrable, et identifions-le à $\mathbb N$. Pour chaque suite binaire infinie $s$, soit $A_s$ l'ensemble de ses préfixes de longueur positive. Deux suites distinctes ont un préfixe commun initial puis divergent; leurs ensembles de préfixes ont une différence symétrique infinie. Les suites binaires infinies étant en bijection avec $\mathcal P(\mathbb N)$, cela donne la famille requise.

## Exercice 15

Les différences $A_{n+1}\setminus A_n$ sont deux à deux disjointes puisque $(A_n)$ est croissante. Leur réunion vaut $(\bigcup_{n\in\mathbb N}A_n)\setminus A_0$. Elles forment une partition de $\mathbb R$ ssi $A_0=\varnothing$ et $\bigcup_nA_n=\mathbb R$.

## Exercice 16

1. $A_y\cap A_z=\varnothing$ si $y\ne z$, car (f(x)) ne peut prendre deux valeurs distinctes. De plus $\bigcup_{y\in Y}A_y=X$, donc les fibres forment un recouvrement disjoint.
2. C'est une partition (aucune fibre vide) ssi (f) est surjective.

## Exercice 17

Le raisonnement ne traite que les (x) qui ont au moins un voisin (y) tel que (xRy). Par exemple, sur (E=\{0,1\}), la relation vide est symétrique et transitive mais non réflexive. L'implication «pour tous (x,y) tels que (xRy)» ne prouve rien pour un (x) sans voisin.

## Exercice 18

1. Par transitivité, $R\circ R\subseteq R$. Pour $xRy$, la réflexivité $yRy$ donne $x(R\circ R)y$; donc $R\circ R=R$.
2. $R\circ S$ est réflexive. Si $R,S$ commutent, son inverse est $S\circ R=R\circ S$, donc il est symétrique; sa composée avec lui-même vaut $R\circ R\circ S\circ S=R\circ S$, donc il est transitif. Réciproquement, si $R\circ S$ est une équivalence, alors $S\circ R=(R\circ S)^{-1}=R\circ S$.
3. Exemple indépendant : sur $E=\{0,1\}^2$, $R$ signifie «même première coordonnée» et $S$ «même seconde coordonnée». Exemple non indépendant : sur $E=\{0,1,2\}$, prendre $R=S$ défini par les classes $\{\{0,1\},\{2\}\}$; un élément de chaque classe n'a pas de $c$ commun.
4. Si $xRy$ et $ySz$, l'indépendance appliquée à $a=z,b=x$ fournit $c$ tel que $zRc$ et $xSc$. Par symétrie, $cRz$, donc $x(S\circ R)z$. Ainsi $R\circ S\subseteq S\circ R$; l'inclusion inverse suit de la symétrie.
5. Si $R,S$ commutent, $T=R\circ S$ est une équivalence d'après 2. Ses classes $E_i$ sont des unions de classes de $R$ et de $S$, car $R,S\subseteq T$. Si $a,b\in E_i$, alors $aTb$, donc il existe $c$ tel que $aRc$ et $cSb$; par symétrie de $S$, $bSc$. Les restrictions sont indépendantes. Réciproquement, sur chaque bloc $E_i$, l'indépendance implique la commutation par 4. Il n'y a pas de couples reliés entre blocs, donc les relations commutent sur $E$.

## Exercice 19+

1. La relation induite par l'ordre quotient est réflexive et transitive, car l'ordre sur $E/\sim$ l'est.
2. (a) La relation $x\sim y\iff x\preceq y\land y\preceq x$ est réflexive et symétrique. Si $x\sim y$ et $y\sim z$, la transitivité donne $x\preceq z$ et $z\preceq x$, donc $x\sim z$. (b) Posons $[x]\preceq^\bullet[y]\iff x\preceq y$. Si $x\sim x'$, $y\sim y'$, la transitivité assure que $x\preceq y\iff x'\preceq y'$; la définition est bien posée. Elle est réflexive, transitive et antisymétrique par construction, donc c'est un ordre, et l'équivalence demandée est sa définition.
3. (i) Pour la divisibilité sur $\mathbb Z$, les classes sont $\{0\}$ et $\{n,-n\}$ pour $n\ge1$; l'ordre quotient est la divisibilité des valeurs absolues. (ii) Les classes des parties finies sont indexées par leur cardinal $n\in\mathbb N$; l'ordre quotient est l'ordre usuel. (iii) Deux parties sont équivalentes ssi leurs intersections avec $\mathbb R_-$ sont égales. Le quotient s'identifie à $\mathcal P(\mathbb R\setminus\mathbb R_-)$, ordonné par inclusion.

## Exercice 20++

1. La réflexivité est immédiate. Deux couples sont comparables en comparant d'abord leurs premières coordonnées, puis les secondes si les premières sont égales; cela donne totalité et antisymétrie. La transitivité découle de la transitivité des deux ordres, donc $\le_{lex}$ est un ordre total.
2. Si $(f_-,f_+)$ sont le prédécesseur et le successeur de $f\in F$, alors $(e,f_-)$ et $(e,f_+)$ sont le prédécesseur et le successeur de $(e,f)$ dans l'ordre lexicographique : tout couple ayant première coordonnée différente est avant ou après toute la fibre $\{e\}\times F$. L'absence d'extrémités vient de celle de $F$.
3. (a) La discrétion fournit les voisins $(x_-,x_+)$; ils sont uniques par totalité. (b) La relation $\leftrightarrow$ est réflexive et symétrique. Si $x\leftrightarrow y$ et $y\leftrightarrow z$, les deux intervalles concernés sont finis; leur réunion contient l'intervalle entre les extrêmes et est finie, donc $x\leftrightarrow z$. (c) Posons $x_0=x$, puis $x_{k+1}=(x_k)_+$ et $x_{k-1}=(x_k)_-$. Cela définit une suite strictement croissante indexée par $\mathbb Z$. Chaque élément équivalent à $x$ est à distance finie dans cet ordre discret, donc est l'un des $x_k$; l'image est exactement $[x]_{\leftrightarrow}$. (d) Chaque classe est un intervalle convexe; deux classes distinctes sont ordonnées sans ambiguïté par leurs représentants. Cette comparaison définit un ordre total sur le quotient $X^\bullet$, et la projection est croissante. (e) Dans chaque classe, choisissons un représentant $r_C$. Le (c) donne l'unique entier $k$ tel que $x=(r_C)_k$. L'application $x\mapsto(C,k)$ est bijective et respecte l'ordre : entre classes, l'ordre est celui de $C$; dans une classe, c'est l'ordre usuel de $k\in\mathbb Z$. C'est l'isomorphisme avec $X^\bullet\times\mathbb Z$ muni de l'ordre lexicographique.
