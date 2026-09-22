# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td03-ensembles-applications.pdf)

## Autocorrection A



```math
E\not\subseteq F\iff\exists x\;(x\in E\land x\notin F),\qquad
E\ne F\iff\exists x\;(x\in E\land x\notin F)\lor\exists y\;(y\in F\land y\notin E).
```



## Autocorrection B



```math
\mathcal P(\{1,2,3\})=\{\varnothing,\{1\},\{2\},\{3\},\{1,2\},\{1,3\},\{2,3\},\{1,2,3\}\}.
```


Avec $A=\{1,2\}$, $B=\{2,3\}$ :


```math
\varnothing=A\setminus(A\cup B),\quad \{1\}=A\setminus B,\quad \{2\}=A\cap B,\quad \{3\}=B\setminus A,
```




```math
\{1,2\}=A,\quad \{2,3\}=B,\quad \{1,3\}=(A\setminus B)\cup(B\setminus A),\quad \{1,2,3\}=A\cup B.
```



## Autocorrection C

Pour tout $x\in E$, exactement l’une des propositions $x\in A$, $x\notin A$ est vraie, d’où $A\cup(E\setminus A)=E$. De même,


```math
x\in(A\cap B)\cup(A\setminus B)\iff(x\in A\land x\in B)\lor(x\in A\land x\notin B)\iff x\in A.
```


La transitivité de $\subseteq$ donne (iii). Enfin,


```math
A\subseteq B\iff(\forall x\in E,\ x\in A\Rightarrow x\in B)
\iff(\forall x\in E,\ x\notin B\Rightarrow x\notin A)\iff E\setminus B\subseteq E\setminus A.
```



## Exercice 1



```math
\begin{array}{ll}
\text{(i)}\ [a,c]\cup[b,d]=[a,d],&\text{(ii)}\ [a,c]\cap[b,d]=[b,c],\\
\text{(iii)}\ [a,b]\cap[c,d]=\varnothing,&\text{(iv)}\ [a,c]\setminus[b,d]=[a,b[,\\
\text{(v)}\ [a,d]\setminus[b,c]=[a,b[\,\cup\,]c,d],&\text{(vi)}\ [b,c]\setminus[a,d]=\varnothing.
\end{array}
```



## Exercice 2

Les compléments sont pris dans $\Omega$. Par distributivité,


```math
(A\cap B)\cup(A\cap\bar B)\cup(\bar A\cap B)\cup(\bar A\cap\bar B)=\Omega.
```


Et par absorption,


```math
A\cup(\bar A\cap B)\cup(\bar A\cap\bar B\cap C)=A\cup B\cup C.
```



## Exercice 3

1. Le diagramme de Venn hachure les deux régions $A\setminus B$ et $B\setminus A$.
2. Pour tout $x$,


```math
x\in(A\cup B)\setminus(A\cap B)\iff (x\in A\lor x\in B)\land\neg(x\in A\land x\in B),
```


soit exactement $(x\in A\land x\notin B)\lor(x\in B\land x\notin A)$. C'est la condition $x\in A\triangle B$.
3. (i) $A\triangle A=(A\setminus A)\cup(A\setminus A)=\varnothing$. (ii) Prendre $E=\varnothing$, car $A\triangle\varnothing=A$. (iii) Prendre $B=A$, alors $A\triangle B=\varnothing$.

## Autocorrection D

1. $y\in\bigcup_{x\in[0,1]}]x-1,x+1[$ ssi $\exists x\in[0,1]:x-1<y<x+1$, ssi $-1<y<2$. L'union vaut donc $]-1,2[$.
2. $y\in\bigcap_{x\in[0,1]}]x-1,x+1[$ ssi $\forall x\in[0,1],\ x-1<y<x+1$. Les contraintes extrêmes donnent $0<y<1$; elles suffisent. L'intersection vaut $]0,1[$.

## Exercice 4

$x\in E\iff x\in\{x\}\iff x\in\bigcup_{y\in E}\{y\}$, donc $E=\bigcup_{y\in E}\{y\}$.

## Exercice 5

1. Si $x\in\liminf E_n$, il existe $n$ tel que $x\in E_k$ pour tout $k\ge n$. Pour tout $m$, on peut choisir $k\ge\max(m,n)$, donc $x\in\bigcup_{k\ge m}E_k$. Ainsi $x\in\limsup E_n$.
2. Pour $E_n=[n,+\infty[$, aucun réel n'appartient à tous les termes d'une queue, donc $\liminf E_n=\varnothing$; tout réel appartient à un nombre fini de termes, donc $\limsup E_n=\varnothing$.
3. Posons $E_n=[(-1)^n n,+\infty[$. Les termes pairs sont $[n,+\infty[$, les impairs $[-n,+\infty[$. Une queue contient les deux familles avec bornes tendant vers $+\infty$, d'où $\liminf E_n=\varnothing$. Tout réel est dans tous les termes impairs suffisamment tardifs, mais pas dans les termes pairs assez grands; il appartient donc à une infinité de termes ssi il appartient aux termes impairs (toujours vrai), ainsi $\limsup E_n=\mathbb R$.

## Exercice 6

Fixons $b_0\in B$. Pour tout $a\in A$, $(a,b_0)\in B\times C$, donc $a\in B$. Ainsi $A\subseteq B$. Fixons ensuite $a_0\in A$; pour tout $b\in B$, $(a_0,b)\in B\times C$, donc $b\in C$, soit $B\subseteq C$. Ainsi $A\subseteq C$.

## Exercice 7+

Supposons $E\not\subseteq F$ et $F\not\subseteq E$. Prenons $e\in E\setminus F$, $f\in F\setminus E$. Alors $(e,f)\in E\times F$, mais $(e,f)\notin F\times\Omega$ puisque $e\notin F$, et $(e,f)\notin\Omega\times E$ puisque $f\notin E$, contradiction. Donc $E\subseteq F$ ou $F\subseteq E$.

## Exercice 8

Avec les entiers de von Neumann et $\mathbb N=\{0,1,\ldots\}$, $E=\{0,1,2\}=3\in\mathbb N$. Les réponses sont : (i) vrai; (ii) vrai; (iii) vrai; (iv) vrai; (v) vrai; (vi) vrai, car $1=\{0\}\subseteq E$; (vii) faux; (viii) vrai; (ix) vrai car $0=\varnothing$; (x) vrai; (xi) vrai; (xii) vrai.

## Exercice 9

$\mathcal P(A\cap B)=\mathcal P(A)\cap\mathcal P(B)$, car $X\subseteq A\cap B\iff X\subseteq A$ et $X\subseteq B$. En revanche $\mathcal P(A)\cup\mathcal P(B)\subseteq\mathcal P(A\cup B)$, avec égalité ssi $A\subseteq B$ ou $B\subseteq A$. Sinon, $\{a,b\}$ pour $a\in A\setminus B, b\in B\setminus A$ est dans le membre droit, pas le gauche.

## Exercice 10+

1. Construction de Gray circulaire par récurrence. Pour $n=1$, la liste $\varnothing,\{1\}$ fonctionne. Si $A_0,\ldots,A_{2^n-1}$ est une liste cyclique, pour $n+1$ prendre successivement


```math
A_0,\ldots,A_{2^n-1},\quad A_{2^n-1}\cup\{n+1\},\ldots,A_0\cup\{n+1\}.
```


Chaque paire consécutive diffère d'un élément; les deux raccords aussi. Toutes les parties sont listées une fois.
2. Il existe un cycle hamiltonien contenant le chemin $\varnothing,\{1\},\ldots,[n]$ comme préfixe. Pour $n=2$, le cycle $\varnothing,\{1\},\{1,2\},\{2\},\varnothing$ convient. Supposons construit un cycle en dimension $n$, orienté de sorte que ce chemin soit son début. Soit $V\ne[n-1]$ l'autre voisin de $[n]$ dans ce cycle (le premier est $[n-1]$). Dans deux copies du cycle, avec/sans le nouvel élément $n+1$, supprimons l'arête $[n],V$ dans la première et $[n]\cup\{n+1\},V\cup\{n+1\}$ dans la seconde; ajoutons les arêtes verticales $[n]\leftrightarrow[n]\cup\{n+1\}$ et $V\leftrightarrow V\cup\{n+1\}$. On obtient un seul cycle hamiltonien : le chemin initial jusqu'à $[n]$ se poursuit par l'arête verticale vers $[n+1]$. La liste cyclique obtenue a donc le préfixe requis.

## Autocorrection E

Les assertions équivalentes sont respectivement : (i) $A\cap B=\Omega$; (ii) $A\cup B=\Omega$; (iii) $A\subseteq B$; (iv) $A=B$; (v) $A\cap B=\varnothing$; (vi) $B\subseteq A$; (vii) $A\ne\Omega$; (viii) $A\subseteq B$. Pour (vii), un X non vide disjoint de A existe ssi le complément de A est non vide. Pour (viii), si $A\not\subseteq B$, choisir $X=\{x\}$ avec $x\in A\setminus B$; la réciproque est immédiate.

## Exercice 11



```math
\forall x\in\{z\in X:P(z)\},\ Q(x)\iff\forall x\in X,\ P(x)\Rightarrow Q(x).
```



## Exercice 12

Si $x=y$, alors les deux appartiennent exactement aux mêmes parties. Si $x\ne y$, la partie $A=\{x\}$ vérifie $x\in A$, $y\notin A$, contradiction avec l'implication universelle. Donc l'équivalence demandée est vraie.

## Exercice 13

Compléments dans $\Omega$.

1. $A\cap B=A\cup B$ équivaut aux inclusions réciproques $A\subseteq B$, $B\subseteq A$.
2. Si $B\subseteq C$, monotonie de l'union/intersection donne les deux inclusions. Réciproquement, la première implique $B\setminus A\subseteq C$, la seconde implique $A\cap B\subseteq C$; leur réunion donne $B\subseteq C$.
3. L'égalité des unions et l'égalité des intersections donnent pour chaque $x$ les mêmes deux tests d'appartenance à B et C relativement à A. Plus simplement, si $x\in B\setminus C$, l'égalité des unions force $x\in A$, puis égalité des intersections donne $x\in C$, absurde; symétriquement $C\setminus B=\varnothing$. Donc $B=C$. La réciproque est immédiate.
4. Si $A\subseteq B\subseteq C$, alors $A\cup B=B=B\cap C$. Réciproquement, $A\cup B=B\cap C\subseteq B$ donne $A\subseteq B$; et $B\subseteq B\cap C$ donne $B\subseteq C$.
5. $A\cap B=A\cap C\iff A\cap\overline B=A\cap\overline C$. En effet, $A\cap\overline B=A\setminus(A\cap B)$, et de même pour C; les deux égalités sont donc chacune équivalentes à $A\cap B=A\cap C$.
6. Si $A\subseteq B$, intersecter avec tout $X$ conserve l'inclusion. Pour la réciproque prendre $X=\Omega$.

## Exercice 14

1. Chaque entier naturel est pair ou impair, donc la partition pair/impair donne l'égalité.
2. Si $A=B$, les unions sont égales. Réciproquement, soit $x\in A\setminus B$. Choisir $n\ne x$; alors $x\in A\cup\{n\}$ mais $x\notin B\cup\{n\}$, contradiction. De même, $B\setminus A=\varnothing$, donc $A=B$.
3. Les égalités des intersections avec $[[0,n]]$ pour tout n détectent l'appartenance de chaque entier en choisissant $n$ égal à cet entier; ainsi équivalence avec $A=B$. Avec les unions, ce n'est pas vrai : pour $A=\mathbb N$, $B=\mathbb N\setminus\{0\}$, on a $A\cup[[0,n]]=B\cup[[0,n]]=\mathbb N$ pour tout n, mais $A\ne B$.

## Exercice 15

Choisissons $a\in A$. Par récurrence, pour tout $k\in\mathbb N$, les implications données donnent $a+k\in A$ et $a-k\in A$. Tout entier est de l'une de ces formes, donc $A=\mathbb Z$.

## Exercice 16+

1. (i) Nécessairement $A\subseteq B$; si cette inclusion vaut, $X=B$ convient. (ii) L'égalité $A\cup X=B$ impose $X\subseteq B$, et chaque élément de $B\setminus A$ doit appartenir à X. Réciproquement, ces deux conditions donnent $A\cup X=B$.
2. Il existe une solution ssi $B\subseteq A$, et les solutions sont exactement $B\subseteq X\subseteq B\cup(\Omega\setminus A)$ : les éléments de $A\setminus B$ sont exclus de $X$, et les éléments hors de $A$ sont libres.

## Exercice 17

1. $\{0,1\}\oplus\{1,4\}=\{1,2,4,5\}$.
2. Prenons $a\in A$. Pour tout $r\in\mathbb R$, $r=(r-a)+a$, donc $r\in A\oplus\mathbb R$.
3. (a) Si $x=a+b$ avec $a\in A_1\cap A_2,b\in B$, alors $x\in(A_1\oplus B)\cap(A_2\oplus B)$. (b) Faux : $A_1=\{0,1\}, A_2=\{0,2\}, B=\{0,1\}$. Leur intersection sommée à B vaut $\{0,1\}$, tandis que l'intersection des sommes contient aussi 2.

## Exercice 18

Notons $\widehat E=\{x:\exists y,(x,y)\in E\}$, $\check E=\{x:\forall y,(x,y)\in E\}$.

1. Pour $H=\{(x,y):xy\le1\}$, la projection existentielle vaut $\mathbb R$ (choisir $y=0$); la section universelle vaut $\{0\}$, car $xy\le1$ pour tout y équivaut à $x=0$.
2. (a) Existence commute avec l'union : $\widehat{A\cup B}=\widehat A\cup\widehat B$. (b) Si $x\in\widehat{A\cap B}$, un même $y$ convient aux deux, donc $x\in\widehat A\cap\widehat B$. (c) Inclusion stricte avec $A=\{(0,0)\}, B=\{(0,1)\}$.
3. Les règles analogues pour le quantificateur universel sont $\check{A\cap B}=\check A\cap\check B$ et $\check A\cup\check B\subseteq\check{A\cup B}$, inclusion stricte en général. La première suit de la conjonction des conditions pour tout y; la seconde de $A\subseteq A\cup B$, $B\subseteq A\cup B$. Stricte: $A=\{(0,y):y\ne0\}$, $B=\{(0,0)\}$; $\check{A\cup B}=\{0\}$ mais $\check A=\check B=\varnothing$.

## Exercice 19

1. Pour tout $x$,


```math
x\in(A\setminus B)\cup(A\setminus C)\iff x\in A\land(x\notin B\lor x\notin C)\iff x\in A\setminus(B\cap C).
```


2. (a) Le membre gauche ne change pas si l’on échange C et D, alors que le membre droit devient $ (A\cap C)\cup(B\cap D)$. Une symétrie de l’énoncé exigerait donc aussi l’égalité avec cette autre expression : l’égalité proposée est surprenante. (b) Prendre $\Omega=\{0\}$, $A=C=\Omega$ et $B=D=\varnothing$. Le membre gauche vaut $\Omega$, le membre droit $\varnothing$. (c) Quatre cercles dessinés dans le plan ne représentent pas les 16 combinaisons possibles d’appartenance à quatre ensembles. Le dessin suggère donc une propriété de cette configuration particulière, pas une identité valable pour tous les ensembles.

## Exercice 20

Supposons $f$ non constante. Il existe $x_1,x_2$ tels que $f(x_1)\ne f(x_2)$, donc l'hypothèse impose $g(x_1)=g(x_2)=c$. Pour tout $x$, si $f(x)\ne f(x_1)$, alors $g(x)=c$; si $f(x)=f(x_1)$, alors $f(x)\ne f(x_2)$, donc encore $g(x)=c$. Ainsi g est constante.

## Exercice 21

Pour chaque $x$, les valeurs indicatrices sont dans $\{0,1\}$. Alors : (i) $\min(1_A,1_B)=1_{A\cap B}$; (ii) $\max(1_A,1_B)=1_{A\cup B}$; (iii) $1_A1_B=1_{A\cap B}$; (iv) $1-1_A=1_{\Omega\setminus A}$; (v) $1_A+1_B-1_A1_B=1_{A\cup B}$, par examen des quatre couples de valeurs 0/1; (vi) $(1_A-1_B)^2=1_{A\triangle B}$.

## Autocorrection F

1. $f(n)=2n$ est injective et non surjective (les nombres impairs ne sont pas atteints).
2. $g(n)=n/2$ si n est pair et $g(n)=n$ si n est impair. Elle est surjective car $g(2m)=m$, mais non injective car $g(1)=g(2)=1$.
3. $g\circ f=\mathrm{id}_{\mathbb N}$, donc injective et surjective. $f\circ g(n)=n$ si n est pair et $2n$ si n est impair. Ce composé n'est pas injectif car les images de 1 et 2 valent 2; il n'est pas surjectif car aucune valeur impaire n'est atteinte.

## Autocorrection G

Sur $\mathbb N$, $f(n)=n^2$ est injective et non surjective (par exemple 2 n'est pas un carré). Une application g telle que $f\circ g=\mathrm{id}$ n'existe pas, car elle rendrait f surjective. Une application h telle que $h\circ f=\mathrm{id}$ existe puisque f est injective : par exemple $h(n)=\lfloor\sqrt n\rfloor$ si $\mathbb N$ contient 0; si $\mathbb N=\mathbb N^*$, prendre h(1)=1 et $h(n)=\lfloor\sqrt n\rfloor$ pour n≥2.

## Exercice 22

(i) Sur $\mathbb N$, $n\mapsto n+1$ est injective, non surjective (0 manque). (ii) Sur $\mathbb Z$, $n\mapsto n+1$ est bijective, d'inverse $n\mapsto n-1$. (iii) $(x,y)\mapsto(y,x)$ est bijective, d'inverse elle-même. (iv) $(x,y)\mapsto3y$ est surjective mais non injective. (v) $(x,y)\mapsto(y,0,y-x)$ est injective (on retrouve y puis x), non surjective (deuxième coordonnée nulle). (vi) Sur $\mathbb R$, $z\mapsto z^2+z+1$ n'est pas injective; son image est $[3/4,+\infty[$, donc elle n'est pas surjective. (vii) Sur $\mathbb C$, le même polynôme est non injectif et surjectif, car tout polynôme quadratique complexe atteint toute valeur. (viii) $(x,y)\mapsto(x+y,xy)$ sur $\mathbb R^2$ n'est pas injective (échanger x,y ne change pas l'image); son image est $\{(s,p):s^2-4p\ge0\}$, donc elle n'est pas surjective. (ix) Sur $\mathbb C^2$, cette application n'est pas injective mais est surjective, car $t^2-st+p$ a toujours deux racines complexes. (x) Sur $\mathbb Z$, $n\mapsto n+(-1)^n$ est bijective : 2k+1 est image de 2k et 2k est image de 2k+1, avec antécédent unique. (xi) et (xii) $f\mapsto f(0)$ de $\mathbb R^{\mathbb R}$ vers $\mathbb R$ est surjective mais non injective. (xiii) $X\mapsto X\cap\mathbb R_+$ est surjective sur $\mathcal P(\mathbb R_+)$, mais non injective.

## Exercice 23

1. $g(f(n))=g(n+1)=n$, car $n+1>0$. 2. Non : $f\circ g\ne\mathrm{id}$, par exemple en 0, et g n’est pas injective puisque $g(0)=g(1)=0$.

## Exercice 24

$\pi(n)$ est croissante au sens large : $\pi(n+1)=\pi(n)$ si n+1 est composé et augmente de 1 si n+1 est premier. Ainsi $\pi(3)=\pi(4)=2$, donc elle n'est pas injective. L'infinité des nombres premiers montre qu'elle est non bornée; partant de $\pi(1)=0$ et augmentant par pas de 0 ou 1, elle prend toutes les valeurs de $\mathbb N$. Elle est surjective mais non bijective.

## Exercice 25+

Si $q,r\in\mathbb Q$ et $\sin q=\sin r$, alors $2\cos((q+r)/2)\sin((q-r)/2)=0$. Si le sinus est nul, $(q-r)/2=k\pi$; comme le membre gauche est rationnel, k=0 et q=r. Si le cosinus est nul, $(q+r)/2=\pi/2+k\pi$, impossible car le membre gauche est rationnel et le droit irrationnel. Donc la fonction est injective. Elle n'est pas surjective, car $\sin q=1$ impose $q=\pi/2+2k\pi\notin\mathbb Q$.

## Exercice 26

1. Si f est surjective et $g_1\circ f=g_2\circ f$, pour chaque y choisir x tel que f(x)=y; alors $g_1(y)=g_2(y)$, donc $\phi$ est injective. Si f ne prend pas la valeur y₀, choisir deux valeurs distinctes de G et définir g₁,g₂ identiques sauf en y₀; leurs composées sont égales, donc $\phi$ n'est pas injective.
2. Si f est injective, pour toute $h:E\to G$, poser $g(f(x))=h(x)$, puis choisir une valeur fixe de G hors de f[E]; alors $g\circ f=h$, donc $\phi$ est surjective. Si $f(x_1)=f(x_2)$ avec $x_1\ne x_2$, choisir h telle que $h(x_1)\ne h(x_2)$; aucune composée ne peut valoir h, donc $\phi$ n'est pas surjective.

## Exercice 27+

1. $\psi$ est injective ssi $X\cup Y=\Omega$. Si un point sort de l'union, l'ajouter à A ne change aucune composante. Réciproquement, $A=(A\cap X)\cup(A\cap Y)$.
2. $\psi$ est surjective ssi $X\cap Y=\varnothing$. Nécessité : les deux composantes d'une image ont la même trace sur l'intersection; si celle-ci est non vide, on peut choisir U,V avec traces distinctes. Si X,Y sont disjoints, pour U⊆X,V⊆Y, prendre A=U∪V.
3. Bijectivité ssi $X\cup Y=\Omega$ et $X\cap Y=\varnothing$; l'inverse est $(U,V)\mapsto U\cup V$.

## Exercice 28++

1. Supposons h(k)=f(k)g(k) bijective. Son unique zéro impose que les antécédents de 0 par f et g soient le même k₀. Les antécédents de 1 et −1 par h ont des facteurs de valeur absolue 1; les deux indices où f vaut ±1 sont donc exactement ceux où g vaut ±1. Mais h doit aussi atteindre 2 : ses facteurs doivent avoir modules 1 et 2, impossible puisque tout indice où l'un vaut ±1 est aussi un indice où l'autre vaut ±1. Donc h n'est pas surjective.
2. Oui. Poser f(k₀)=g(k₀)=0. Ensuite, énumérer les valeurs entières restantes et construire f,g par récurrence en affectant successivement une nouvelle valeur de l'une des bijections et en choisissant une valeur non encore utilisée de l'autre. À chaque étape, avec un facteur fixé non nul, seuls un nombre fini de choix donnent un produit déjà obtenu; on peut donc éviter les collisions. En faisant apparaître chaque entier dans chaque énumération, les deux applications sont bijectives et leur produit injectif.

## Exercice 29

(i) Vrai : la restriction d'une injection est injective. (ii) Faux : $E=\{0,1\}$, $A=\{0\}$, $f$ constante. (iii) Faux : $E=F=\{0,1\}$, $f=\operatorname{id}$, $A=\{0\}$. (iv) Vrai : $f[A]=F$ implique $f[E]=F$.

## Exercice 30

Si $f$ est strictement monotone, $x<y$ entraîne $f(x)\ne f(y)$, donc $f$ est injective. Réciproque fausse : échanger les valeurs de $0$ et $1$ dans l'identité définit une bijection non monotone.

## Exercice 31

1. Si $f$ est impaire et bijective, pour $y=f(x)$, $f^{-1}(-y)=f^{-1}(f(-x))=-x=-f^{-1}(y)$. La réciproque s'obtient en appliquant le même raisonnement à $f^{-1}$.
2. Une bijection $\mathbb R\to\mathbb R$ ne peut être paire : $f(-x)=f(x)$ contredit l'injectivité pour $x\ne0$. Ainsi ni $f$ ni son inverse ne peut être paire.

## Exercice 32

La surjectivité de $g\circ f$ entraîne celle de $g$; l'injectivité de $h\circ g$ entraîne celle de $g$. Donc $g$ est bijective. Alors $f=g^{-1}\circ(g\circ f)$ et $h=(h\circ g)\circ g^{-1}$ sont bijectives.

## Exercice 33+

On a $f^n=f$. Si f est injective, $f(f^{n-1}(x))=f(x)$ donne $f^{n-1}(x)=x$; ainsi f est surjective. Si f est surjective, chaque y=f(x) vérifie $f^{n-1}(y)=f^n(x)=f(x)=y$; donc $f^{n-1}=\mathrm{id}$, et f est injective. Pour n=2, si f est injective, f²=f entraîne f=id; réciproquement l'identité est injective. Donc f injective ssi f=id.

## Exercice 34+

(i) Si $g\circ f=\operatorname{id}$, $f(x)=f(y)$ donne $x=y$. Si $f$ est injective, poser $g(f(x))=x$ sur $f[X]$ et prolonger arbitrairement sur $Y\setminus f[X]$ ($X$ non vide). (ii) Si $f\circ h=\operatorname{id}$, $f$ est surjective. Si $f$ est surjective, choisir pour chaque $y$ un antécédent $h(y)$; alors $f\circ h=\operatorname{id}$.

## Exercice 35+

Supposons $f(k)<g(k)$. Choisir $m_1$ tel que $g(m_1)=f(k)$, possible par surjectivité. Alors $f(m_1)\le f(k)$; l'égalité imposerait $m_1=k$ par injectivité, contredisant $g(k)>f(k)$. Donc $f(m_1)<f(k)$. En répétant, on obtient une suite infinie strictement décroissante d'entiers naturels, impossible. Ainsi $f=g$.

## Exercice 36

1. $\sin\mathbb R=[-1,1]$; $\sin\mathbb R_+=[-1,1]$; $\sin[0,2\pi]=[-1,1]$; $\sin[-\pi,\pi]=[-1,1]$; $\sin[0,\pi/2]=[0,1]$; $\sin[-\pi,\pi/2]=[-1,1]$.
2. $\sin^{-1}([-1,1])=\mathbb R$; $\sin^{-1}([0,1])=\bigcup_{k\in\mathbb Z}[2k\pi,(2k+1)\pi]$; $\sin^{-1}([3,4])=\varnothing$; $\sin^{-1}(\mathbb R)=\mathbb R$; $\sin^{-1}\{1\}=\{\pi/2+2k\pi:k\in\mathbb Z\}$; $\sin^{-1}\{-1,1\}=\{\pi/2+k\pi:k\in\mathbb Z\}$.

## Exercice 37

$f(x)=2(x-1)^2-1$.

1. f n'est pas injective (symétrie autour de 1), ni surjective (minimum −1).
2. Sur $[1,+\infty[$, f est strictement croissante, d'image $[-1,+\infty[$; son inverse est $y\mapsto1+\sqrt{(y+1)/2}$.
3. $f([0,1])=[-1,1]$; $f(\mathbb R_-)=[1,+\infty[$; $f(\mathbb R_+)=[-1,+\infty[$; $f([-2,2])=[-1,17]$. De plus $f^{-1}\{1\}=\{0,2\}$, $f^{-1}\{-1\}=\{1\}$,


```math
f^{-1}[0,1]=[0,1-1/\sqrt2]\cup[1+1/\sqrt2,2],\qquad f^{-1}[-2,1]=[0,2].
```



## Exercice 38

1. Si $z+1/z=w$, z est racine de $z^2-wz+1=0$; les racines sont non nulles, donc f est surjective. Comme f(z)=f(1/z), elle n'est pas injective.
2. Pour réel non nul x, $x+1/x\in]-\infty,-2]\cup[2,+\infty[$, et toutes ces valeurs sont atteintes. Si |z|=1, z=e^{it}, alors $z+1/z=2\cos t$, donc $f[U]=[-2,2]$.

## Exercice 39

Les fibres $A_y=f^{-1}\{y\}$ sont disjointes deux à deux et leur union est $X$ : chaque $x$ appartient exactement à la fibre de $f(x)$. Pour $m(z)=|z|$, ce sont les cercles de centre $0$ et rayon $r\ge0$. Pour $\alpha(z)=z/|z|$ sur $\mathbb C^*$, ce sont les demi-droites $\{r\omega:r>0\}$, $|\omega|=1$. Pour $\operatorname{Re}$, ce sont les droites verticales $\{x+it:t\in\mathbb R\}$.

## Exercice 40

La stabilité équivaut à $n\in A\Rightarrow n+1\in A$. Donc $A=\varnothing$, ou bien, si $m=\min A$, $A=\{n\in\mathbb N:n\ge m\}$.

## Exercice 41

1. Si $x$ appartient à l'intersection ou à l'union des $A_i$, la stabilité de chaque $A_i$ entraîne respectivement $f(x)$ dans tous les $A_i$ ou dans au moins un d'eux. Donc intersection et union sont stables.
2. Faux : $f(0)=0$ et $f(n)=n-1$ si $n\ge1$. $A=\{0\}$ est stable, mais $f(1)=0$ montre que son complémentaire ne l'est pas.

## Exercice 42

1. Toujours $f[A\cap B]\subseteq f[A]\cap f[B]$. Si $f$ est injective et $y=f(a)=f(b)$, $a\in A$, $b\in B$, alors $a=b$ et $y\in f[A\cap B]$. Réciproquement, si $f(x)=f(y)$ avec $x\ne y$, choisir $A=\{x\}$, $B=\{y\}$ : l'égalité échoue.
2. La bijectivité donne $f[E\setminus A]=F\setminus f[A]$. Réciproquement, $A=\varnothing$ donne la surjectivité. Si $f(x)=f(y)$ avec $x\ne y$, choisir $A=\{x\}$; alors $f(y)\in f[E\setminus A]$ mais $f(y)\notin F\setminus f[A]$, contradiction.

## Exercice 43+

1. $x\in A\Rightarrow f(x)\in f[A]\Rightarrow x\in f^{-1}(f[A])$. Exemple strict : $f$ constante sur $E=\{0,1\}$, $A=\{0\}$.
2. Si $f$ est injective, l'inclusion précédente est égalité. Réciproquement, l'égalité pour $A=\{x\}$ entraîne $f(y)=f(x)\Rightarrow y=x$.
3. La définition donne $f[f^{-1}[B]]\subseteq B$. Si $f$ n'est pas surjective, choisir $B=\{y\}$ avec $y$ hors de $f[E]$ donne une inclusion stricte.
4. Si $f$ est surjective, tout $y\in B$ possède un antécédent et l'image de la préimage vaut $B$. Réciproquement, appliquer l'égalité à chaque singleton $\{y\}$ montre que $f$ atteint tout $y$.

## Exercice 44+

1. $f$ injective entraîne $\varphi$ injective : $f[A]=f[B]$ implique $A=B$ en remontant chaque égalité d'images par l'injectivité. Réciproquement, $\varphi(\{x\})=\varphi(\{y\})$ entraîne $x=y$. Si $f$ est injective, $\psi(f[A])=f^{-1}(f[A])=A$, donc $\psi$ est surjective. Réciproquement, si $\psi$ est surjective et $f(x)=f(y)$ avec $x\ne y$, aucune préimage ne peut être $\{x\}$, donc $\psi$ n'est pas surjective.
2. Si $f$ est surjective, toute $B\subseteq F$ vérifie $B=f[f^{-1}(B)]$, donc $\varphi$ est surjective; réciproquement, appliquer à $B=\{y\}$. Si $f$ est surjective et $f^{-1}(B)=f^{-1}(C)$, un antécédent de tout $y\in B\triangle C$ contredirait l'égalité, donc $B=C$. Si $f$ n'est pas surjective, un $y_0$ hors image donne $\psi(\varnothing)=\psi(\{y_0\})$, donc $\psi$ n'est pas injective.

## Exercice 45

Une suite décroissante d'entiers naturels possède un minimum $m$. Dès qu'elle atteint $m$, elle y reste; elle est stationnaire.

## Exercice 46

Si les $A_j$ partitionnent $\mathbb N^*$, chaque entier de $1$ à $n$ est compté une fois. Réciproquement, si la somme des effectifs vaut $n$ pour tout $n$, la différence entre les sommes aux rangs $k$ et $k-1$ est le nombre de $A_j$ contenant $k$; elle vaut $1$. Chaque entier appartient donc exactement à un $A_j$.

## Exercice 47+

1. Pour $m=\min_i x_i$ et $M=\max_i x_i$, $m\le x_i\le M$; sommer puis diviser par $n$.
2. Les $n$ fibres $f^{-1}\{j\}$ partitionnent $m$ éléments. Si $f$ est injective, chaque fibre a au plus un élément, donc $m\le n$, contradiction.
3. Pour $N\ge2$, les degrés sont dans $\{0,\ldots,N-1\}$; les degrés $0$ et $N-1$ ne peuvent être pris ensemble. Il reste au plus $N-1$ valeurs pour $N$ inscrits, donc deux ont le même nombre d'amis. Pour $N=0$ ou $N=1$, l'assertion n'est pas vraie.

## Exercice 48++

Si $X=\varnothing$, aucune partie non vide propre n'existe, donc la propriété échoue. Si $X$ est fini non vide, choisir une permutation cyclique $f$ dont l'unique orbite est $X$. Une partie non vide stable par $f$ contient toute l'orbite, donc vaut $X$ : la propriété échoue.

Supposons $X$ infini et fixons $f:X\to X$. Si une orbite $\{f^n(x):n\ge0\}$ est infinie, ses termes sont tous distincts (une répétition rendrait l'orbite finie). Alors $A=\{f^n(x):n\ge1\}$ est non vide, stable et ne contient pas $x$. Sinon toutes les orbites sont finies; choisir une orbite $O$. Elle est stable, non vide et, comme $X$ est infini, propre.

## Exercice 49++

Supposons chaque $A_n\ne\mathbb N$ et posons $B_n=\mathbb N\setminus A_n$. Les $B_n$ sont décroissants, non vides, d'intersection vide puisque $\bigcup_n A_n=\mathbb N$. Chaque $B_n$ est infini : s'il était fini, la suite décroissante non vide $(B_m)_{m\ge n}$ de parties de $B_n$ stabiliserait sur une partie non vide, contredisant l'intersection vide.

Choisir récursivement des éléments distincts $x_n\in B_n$, possible car $B_n$ est infini, puis poser $X=\{x_n:n\in\mathbb N\}$. Pour tout $m$, si $n\ge m$, $x_n\in B_n\subseteq B_m$; donc $X\cap A_m\subseteq\{x_0,\ldots,x_{m-1}\}$ est fini. Cela contredit l'hypothèse pour la partie infinie $X$. Il existe donc $n$ tel que $A_n=\mathbb N$.

## Exercice 50+

1. Pour $n\in\mathbb N$, écrivons de façon unique $n+1=2^a(2b+1)$, avec $a,b\in\mathbb N$. Ainsi $\varphi(a,b)=2^a(2b+1)-1$ est bijective; son inverse associe à $n$ ces deux exposants.
2. Le tableau donne l'ordre des diagonales $a+b=d$, en prenant $b=0,\ldots,d$. Posons $T_d=d(d+1)/2$. Alors $\psi^{-1}(a,b)=T_{a+b}+b$. Pour $n$, l'unique $d$ vérifiant $T_d\le n<T_{d+1}$ donne $b=n-T_d$, $a=d-b$. Ces formules sont inverses l'une de l'autre.
3. Récurrence : $\mathbb N^1\simeq\mathbb N$; si $\mathbb N^r\simeq\mathbb N$, alors $\mathbb N^{r+1}\simeq\mathbb N^r\times\mathbb N\simeq\mathbb N^2\simeq\mathbb N$.
4. $\mathbb N^{(\mathbb N)}=\bigcup_{N\in\mathbb N}\{u:u_n=0\ \forall n>N\}$. Pour chaque $N$, l'ensemble à droite est en bijection avec $\mathbb N^{N+1}$, donc dénombrable d'après 3. Une réunion dénombrable d'ensembles dénombrables est dénombrable. Elle est infinie car les suites ayant un seul terme non nul sont distinctes.
5. Si $(u^{(k)})_{k\in\mathbb N}$ énumérait toutes les suites, poser $v_k=u^{(k)}_k+1$. Alors $v$ diffère de la $k$-ième suite au rang $k$, contradiction.

## Exercice 51+

1. Posons $x_n=1/(n+2)$. Définir $f(x_0)=1$, $f(x_n)=x_{n-1}$ pour $n\ge1$, et $f(x)=x$ ailleurs dans $]0,1[$. C'est une bijection $]0,1[\to]0,1]$.
2. Si $\omega\in A$, rien à prouver. Si $A$ est fini et $\omega\notin A$, les cardinaux diffèrent. Si $A$ est infini, choisir une suite injective $(a_n)$ dans $A$, envoyer $a_0$ sur $\omega$, $a_{n+1}$ sur $a_n$, et fixer les éléments de $A\setminus\{a_n\}$; cela définit une bijection $A\to A\cup\{\omega\}$.

## Exercice 52+

1. À $\varphi:F\times G\to E$, associer $\widetilde\varphi:F\to E^G$, $\widetilde\varphi(x)(y)=\varphi(x,y)$. L'application inverse envoie $u:F\to E^G$ sur $(x,y)\mapsto u(x)(y)$. Ainsi $E^{F\times G}\simeq(E^G)^F$, donc $|E|^{|F||G|}=(|E|^{|G|})^{|F|}$.
2. À $(f:E\to F,g:E\to G)$ associer $x\mapsto(f(x),g(x))$; l'inverse compose par les deux projections. Donc $F^E\times G^E\simeq(F\times G)^E$, et $|F|^{|E|}|G|^{|E|}=(|F||G|)^{|E|}$.

## Exercice 53+++

1. $A_n=\{2n,2n+1\}$. Pour $n\ne m$, ces ensembles disjoints et non vides ne sont pas inclus l'un dans l'autre.
2. $B_X=\{2n:n\in X\}\cup\{2n+1:n\notin X\}$. Si $X\ne Y$, un indice $n$ appartient à l'un seul des deux; les deux inclusions échouent. Donc $B_X\subseteq B_Y\Rightarrow X=Y$.
3. Avec une bijection de codage $p:\mathbb N^2\to\mathbb N$, poser $C_X=\{p(n,m):n\in X,\ m\in\mathbb N\}$. Si $X\ne Y$, choisissons $n\in X\triangle Y$; alors la différence symétrique de $C_X,C_Y$ contient tous les $p(n,m)$, $m\in\mathbb N$, donc est infinie.
