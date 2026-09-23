# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td16-limites-continuite.pdf)

## Autocorrection A

(i) $|x\sin(x^2)/(1+x^2)|\le x/(1+x^2)\to0$, donc la limite vaut $0$.

(ii) Pas de limite: $x_k=\sqrt{2k\pi}$ donne $1$, $y_k=\sqrt{(2k+1)\pi}$ donne $-1$.

(iii) $\sqrt x(\sqrt{x+1}-\sqrt{x-1})=2\sqrt x/(\sqrt{x+1}+\sqrt{x-1})\to1$.

(iv) $(\ln x+\cos x)^2\to+\infty$.

(v) Si $x>1$, $\lfloor1/x\rfloor=0$, donc la limite vaut $0$.

(vi) $x\lfloor1/x\rfloor\to1$ car $\lfloor t\rfloor/t\to1$ lorsque $t\to\pm\infty$.

(vii) $x^{-1}\ln(1+x)\to0$, donc $(1+x)^{1/x}\to1$.

(viii) $\lim_{x\to0}(1+x)^{1/x}=e$.

(ix) $(x^2+\sin x)/(1+x^2)\to1$.

(x) Par rationalisation,


```math
\sqrt{x+\sqrt{x+\sqrt x}}-\sqrt x=\frac{\sqrt{x+\sqrt x}}{\sqrt{x+\sqrt{x+\sqrt x}}+\sqrt x}\longrightarrow\frac12.
```



(xi) $\ln\left[(\ln x/x)^{1/x}\right]=(\ln\ln x-\ln x)/x\to0$, donc la limite vaut $1$.

(xii) Le numérateur est équivalent à $x^2$ et le dénominateur à $|x|$; la limite vaut $+\infty$.

(xiii) $x^3-3x+2=(x-1)^2(x+2)$ et $2x^2-x-1=(x-1)(2x+1)$. Le quotient vaut $\frac{|x-1|}{x-1}\frac{\sqrt{x+2}}{2x+1}$; limites à gauche et à droite: $-\sqrt3/3$ et $\sqrt3/3$. La limite bilatérale n’existe pas.

(xiv) $(1+1/x)^x\to e$.

(xv) Le numérateur est équivalent à $(1-2)\sqrt x$ et le dénominateur à $(1-\sqrt2)\sqrt x$. La limite vaut $(\sqrt2+1)$.

(xvi) $\frac1{1-x}-\frac2{1-x^2}=\frac{-1}{1+x}\to-1/2$.

(xvii) $\frac{\sqrt x-1}{x-1}=1/(\sqrt x+1)\to1/2$.

(xviii) $\sqrt{x^2+2x}-x=2x/(\sqrt{x^2+2x}+x)\to1$.

(xix) Avec $t=\ln x\to0^+$, $\ln x\ln(\ln x)=t\ln t\to0$.

(xx) $\arccos x\sim\sqrt{2(1-x)}$, donc $(1-x)/\arccos x\to0$.

## Exercice 1

(i) $\lfloor1/x\rfloor\to+\infty$ à droite et $\to-\infty$ à gauche.

(ii) Écrire $\lfloor1/x\rfloor=1/x-\theta_x$, avec $0\le\theta_x<1$. Alors


```math
x\lfloor1/x\rfloor=1-x\theta_x\longrightarrow1
```


à gauche comme à droite.

(iii) De même,


```math
x^2\lfloor1/x\rfloor=x-x^2\theta_x\longrightarrow0
```


à gauche comme à droite.

## Exercice 2

Si $f(x)\to\ell$, alors $\sin x\to0$ donne $f(\sin x)\to\ell$. Réciproquement, pour $y\to0$, posons $x=\arcsin y\to0$; alors $y=\sin x$ et $f(y)=f(\sin x)\to\ell$.

## Exercice 3

Comme $f$ est bijective et croissante, elle est non majorée: pour tout $A$, il existe $x_A$ tel que $f(x_A)>A$. Pour $x\ge x_A$, $f(x)\ge f(x_A)>A$; donc $f(x)\to+\infty$.

## Exercice 4

Pour tout $x$, il existe des indices arbitrairement grands tels que $\xi_n\ge x$. Ainsi $f(x)\le f(\xi_n)$, puis $f(x)\le\ell$ par passage à la limite.

Pour $\varepsilon>0$, choisir $n$ tel que $f(\xi_n)>\ell-\varepsilon$. Alors


```math
x\ge\xi_n\Longrightarrow\ell-\varepsilon<f(\xi_n)\le f(x)\le\ell.
```


Donc $f(x)\to\ell$ en $+\infty$.

Sans croissance, $f(x)=\sin(2\pi x)$ et $\xi_n=n$ donnent $f(\xi_n)=0$, alors que $f$ n'a pas de limite en $+\infty$.

## Exercice 5+

Pour $x\in(a,b)$, la limite monotone à droite existe et vaut


```math
L(x)=\inf\{f(t):x<t<b\}.
```


Pour $a<r<x<s<b$, $f(r)\le L(x)\le f(s)$ : cette limite est finie. Si $x<y$, l'ensemble sur lequel est pris l'infimum pour $y$ est contenu dans celui correspondant à $x$, donc $L(x)\le L(y)$. Ainsi $L$ est bien définie et croissante.

## Exercice 6+

Pour tout point de discontinuité $a$ d’une fonction monotone croissante, les limites à gauche et à droite existent et définissent un intervalle ouvert non vide $(f(a-),f(a+))$. Ces intervalles sont disjoints pour deux points de discontinuité distincts. Choisissons dans chacun un rationnel; cela définit une injection de $D$ dans $\mathbb Q$. Pour une fonction décroissante, appliquer le raisonnement à $-f$.

## Exercice 7

Si $f(x)\to L$ et si $T>0$ est une période, alors pour tout $x$, $f(x)=f(x+nT)\to L$ lorsque $n\to\infty$; donc $f(x)=L$ pour tout $x$. La réciproque est immédiate.

## Exercice 8

Non. Posons $f(x)=0$ si $x=1/n$ pour un entier $n\ge1$, et $f(x)=1$ sinon. Lorsque $x\to0^+$, $\lfloor1/x\rfloor=n\to\infty$ et $1/\lfloor1/x\rfloor$ est un terme de la forme $1/n$, donc l’expression testée tend vers $0$. Pourtant $f(x)$ n’a pas de limite en $0$.

## Exercice 9+

Poser $t=f(x)>0$ et $u(x)=t+1/t-2=(t-1)^2/t\to0$. Si $t\notin[1/2,2]$, alors $u(x)\ge1/2$. Donc $t\in[1/2,2]$ pour $x$ assez proche de $0$, et


```math
(t-1)^2=t\,u(x)\le2u(x)\longrightarrow0.
```


Ainsi $f(x)\to1$.

## Exercice 10+

1. Si $f(x)\to L$, alors $f(2x)\to L$ et $f(x)f(2x)\to L^2=0$, donc $L=0$.
2. Pour $x\ne0$, posons $f(x)=1$ si $\lfloor\log_2|x|\rfloor$ est pair, et $f(x)=0$ sinon. Les parités changent quand $x$ est remplacé par $2x$, donc $f(x)f(2x)=0$, tandis que $f$ prend les valeurs $0$ et $1$ arbitrairement près de $0$.

## Exercice 11+

Pour $n\in\mathbb N$, $f(n)=f(0)+\sum_{k=0}^{n-1}(f(k+1)-f(k))=o(n)$ par Cesàro, puisque les accroissements tendent vers $0$. Si $n\le x<n+1$, la croissance donne $0\le f(x)/x\le f(n+1)/n\to0$. Donc $f(x)/x\to0$.

## Autocorrection B

(i) Domaine $\mathbb R^*$. La fonction tend vers $0$ en $0$; prolongement continu par $f(0)=0$.

(ii) Domaine $]0,+\infty[\setminus\{1\}$. En $0^+$, $x\ln x/(x-1)\to0$; en $1$, le quotient tend vers $1$. Prolongement continu en $0$ par $0$ et en $1$ par $1$.

(iii) Domaine $\mathbb R\setminus\{1\}$. Le quotient vaut $(x+1)(x-1)/|x-1|$; limites en $1^-$ et $1^+$ égales à $-2$ et $2$. Pas de prolongement continu en $1$.

(iv) Domaine $\mathbb R\setminus\{1\}$. Le quotient vaut $|x-1|(x+1)^2\to0$; prolongement par $0$ en $1$.

(v) Domaine $\mathbb R^*$. $|\sin x\sin(1/x)|\le|\sin x|\to0$; prolongement par $0$ en $0$.

(vi) Domaine $\mathbb R^*$. Comme $\cos x\to1$, le produit a le comportement de $\cos(1/x)$; il n’a pas de limite en $0$.

## Exercice 12

Sur chaque intervalle $[n,n+1[$, la fonction vaut $n+(x-n)^2$. Elle est continue sur ces intervalles et ses limites à gauche et à droite en l’entier $n$ valent toutes deux $n$, égales à sa valeur. Elle est continue sur $\mathbb R$.

## Exercice 13

Pour $a>0$ et $x>a$, la croissance donne $f(a)\le f(x)$, tandis que la décroissance de $f(t)/t$ donne $f(x)\le xf(a)/a$. Ainsi $f(x)\to f(a)$ quand $x\downarrow a$. Pour $x<a$, on a $xf(a)/a\le f(x)\le f(a)$; donc $f(x)\to f(a)$ quand $x\uparrow a$. Cela vaut pour tout $a>0$, donc $f$ est continue.

## Exercice 14

L'énoncé est faux sans hypothèse supplémentaire : pour $f(x)=x$, le groupe des périodes vaut $\{0\}$ ; pour une fonction constante, il vaut $\mathbb R$.

Pour toute fonction continue, son groupe $H$ de périodes est un sous-groupe fermé de $\mathbb R$ : si $h_n\in H$ et $h_n\to h$, alors $f(x+h)=\lim_n f(x+h_n)=f(x)$.

Si $H$ possède des éléments positifs arbitrairement petits, il est dense : pour $h\in H$, $h>0$, et $t\in\mathbb R$, un multiple entier de $h$ est à distance au plus $h$ de $t$. Comme $H$ est fermé, $H=\mathbb R$, et $f$ est constante.

Sinon, si $H\ne\{0\}$, poser $T=\inf(H\cap\mathbb R_+^*)>0$. La fermeture donne $T\in H$. Pour $h\in H$,


```math
h-\lfloor h/T\rfloor T\in H\cap[0,T)=\{0\},
```


donc $H=T\mathbb Z$.

Ainsi


```math
H=\{0\},\quad H=T\mathbb Z\ (T>0),\quad\text{ou}\quad H=\mathbb R.
```


La conclusion demandée vaut exactement pour les fonctions continues, périodiques et non constantes.

## Exercice 15

Pour $x<y$, choisissons $a_n,b_n\in D$ tels que $a_n\to x$, $b_n\to y$ et $a_n<b_n$. Alors $f(a_n)\le f(b_n)$; par continuité, $f(x)\le f(y)$. Donc $f$ croît. Le résultat strict reste vrai: si $f(x)=f(y)$ pour $x<y$, la croissance impose que $f$ soit constante sur $[x,y]$, lequel contient deux points distincts de $D$, contradiction à la stricte croissance sur $D$.

## Exercice 16+

### 1

Si $f$ est continue et $x\in\overline A$, choisir $a_n\in A$ tel que $a_n\to x$. Alors $f(a_n)\to f(x)$, donc $f(x)\in\overline{f[A]}$.

Réciproquement, supposons cette inclusion pour toute partie $A$. Si $f$ n'était pas continue en $x$, il existerait $\varepsilon>0$ et $x_n\to x$ tels que $|f(x_n)-f(x)|\ge\varepsilon$. Pour $A=\{x_n:n\ge0\}$, on aurait $x\in\overline A$, mais


```math
\overline{f[A]}\subset\{y:|y-f(x)|\ge\varepsilon\},
```


ce qui contredit $f(x)\in\overline{f[A]}$.

### 2

Le sous-groupe $G=\mathbb Z+2\pi\mathbb Z$ est dense dans $\mathbb R$. En effet, partager $[0,1[$ en $N$ intervalles égaux et considérer les parties fractionnaires de $0,2\pi,\ldots,2N\pi$. Deux d'entre elles appartiennent au même intervalle. Leur différence fournit $h\in G$ avec $0<|h|<1/N$ ; la non-nullité découle de l'irrationalité de $\pi$. Les multiples entiers de tels $h$ approchent tout réel arbitrairement près.

Par continuité de cosinus,


```math
[-1,1]=\cos(\overline G)\subset\overline{\cos G}.
```


Or $\cos(m+2k\pi)=\cos m$ et $\cos(-m)=\cos m$, donc $\cos G=\{\cos n:n\in\mathbb N\}$. Cette partie est dense dans $[-1,1]$.

## Exercice 17+

1. $\varnothing$ et $\mathbb R$ sont ouverts et fermés. $[0,1]$ est fermé, non ouvert; $]0,1[$ est ouvert, non fermé; $[0,1[$ n’est ni ouvert ni fermé; $\mathbb R_+$ est fermé, non ouvert; $\mathbb Q$ n’est ni ouvert ni fermé.
2. Si $F$ est fermé, $f^{-1}[F]$ est fermé: si $x_n\to x$ avec $f(x_n)\in F$, alors $f(x_n)\to f(x)$ et $f(x)\in F$. Si $U$ est ouvert, son complémentaire est fermé et $f^{-1}[U]$ est le complémentaire de $f^{-1}[\mathbb R\setminus U]$, donc est ouvert.
3. Si $X=\overline X$ et $a\notin X$, alors $a\notin\overline X$ ; il existe $\delta>0$ tel que $[a-\delta,a+\delta]\cap X=\varnothing$. Donc $\mathbb R\setminus X$ est ouvert. Réciproquement, si ce complémentaire est ouvert, chaque $a\notin X$ possède un voisinage disjoint de $X$ et n'appartient pas à $\overline X$. Ainsi $\overline X\subset X$, donc $X$ est fermé.

## Exercice 18++

Énumérer sans répétition $\mathbb Q=\{q_0,q_1,\ldots\}$ et $V=\{v_0,v_1,\ldots\}$. Construire des bijections strictement croissantes entre des parties finies de ces ensembles, en prolongeant à chaque étape la précédente.

À une étape paire, prendre le premier $q_i$ non encore associé et choisir un $v_j$ inutilisé entre les images de ses deux voisins déjà associés ; s'il manque un voisin, choisir dans la demi-droite correspondante. La densité de $V$ fournit toujours une infinité de choix. À une étape impaire, prendre le premier $v_j$ non encore associé et procéder de même dans $\mathbb Q$ pour lui trouver un antécédent. La réunion de ces bijections finies est un isomorphisme d'ordre $h:\mathbb Q\to V$.

Définir


```math
\varphi(x)=\sup\{h(q):q\in\mathbb Q,\ q<x\}.
```


Le supremum est fini : choisir des rationnels $r<x<s$, alors $h(r)\le\varphi(x)\le h(s)$. Pour $x<y$, choisir $x<q_1<q_2<y$ ; alors


```math
\varphi(x)\le h(q_1)<h(q_2)\le\varphi(y).
```


La fonction est strictement croissante. La densité de $V$ donne $\varphi(q)=h(q)$ pour chaque rationnel $q$.

Pour $z\in\mathbb R$, poser $x=\sup\{q\in\mathbb Q:h(q)<z\}$. Cet ensemble est non vide et majoré, puisque $V$ est dense et non borné aux deux extrémités. Pour tout $\varepsilon>0$, choisir $v_-,v_+\in V$ tels que $z-\varepsilon<v_-<z<v_+<z+\varepsilon$ ; les antécédents par $h$ encadrent la coupure $x$, et la définition du supremum donne $z-\varepsilon\le\varphi(x)\le z+\varepsilon$. Donc $\varphi(x)=z$.

Ainsi $\varphi$ est une bijection croissante $\mathbb R\to\mathbb R$. Un saut laisserait un intervalle omis dans son image ; elle est donc continue, et le même argument vaut pour son inverse. Enfin $\varphi[\mathbb Q]=h[\mathbb Q]=V$.

## Autocorrection C

Poser $g(x)=e^x-\pi^2\ln(1+x^2)$. Alors $g(0)=1>0$ et


```math
g(1)=e-\pi^2\ln2<3-9/2<0,\qquad g(-1)<g(1)<0.
```


De plus $g(x)\to+\infty$ lorsque $x\to+\infty$. Le théorème des valeurs intermédiaires fournit une racine dans chacun des intervalles $]-1,0[$, $]0,1[$ et $]1,R[$ pour $R$ assez grand.

## Exercice 19

Pour un polynôme $P$ de degré impair à coefficient dominant $a\ne0$, les limites de $P(t)$ aux deux infinis sont $+\infty$ et $-\infty$ dans un certain ordre. La continuité et le théorème des valeurs intermédiaires montrent que toute valeur réelle est atteinte.

## Exercice 20

L’image continue d’un intervalle est un intervalle. Un intervalle inclus dans $\mathbb Z$ est réduit à un point; $f$ est constante.

## Exercice 21

1. $f^2=g^2$ et $f\ne0$ impliquent que $h=g/f$ est continue et prend ses valeurs dans $\{-1,1\}$. L’image de l’intervalle $I$ par $h$ est connexe, donc réduite à un point: $g=f$ ou $g=-f$.
2. (a) Sur $I=\mathbb R$, prendre $g(x)=1$ et $f(x)=1$ si $x\ge0$, $f(x)=-1$ si $x<0$. Alors $g$ est continue, $f$ ne s'annule pas, $f^2=g^2$, mais $f$ n'est continue ni égale à $g$ ou $-g$ sur tout $I$.
(b) $f(x)=x$, $g(x)=|x|$ sur $\mathbb R$.
(c) Sur $I=\{-1,1\}$, $f(x)=x$, $g(x)=1$.

## Exercice 22

La fonction n’est pas continue en $0$, car $\sin(1/x)$ n’y a pas de limite. Elle vérifie pourtant le théorème des valeurs intermédiaires: sur tout intervalle ne contenant pas $0$, elle est continue; si l’intervalle contient $0$ et une valeur $a>0$, il contient une suite de points où $\sin(1/x)$ prend toute valeur de $[-1,1]$ arbitrairement près de $0$. Le cas $a<0$ est analogue; les valeurs entre $0$ et toute valeur prise ailleurs sont aussi atteintes.

## Exercice 23

1. Posons $h(x)=f(x)-x$. Si $f([a,b])\subset[a,b]$, alors $h(a)\ge0$ et $h(b)\le0$; le TVI donne un zéro.
2. Choisissons $x_a,x_b$ tels que $f(x_a)=a$ et $f(x_b)=b$. Si $x_a\le x_b$, $h(x_a)=a-x_a\le0$ et $h(x_b)=b-x_b\ge0$. Si $x_b<x_a$, les signes sont inversés. Dans les deux cas, le TVI fournit un point fixe.

## Exercice 24

$h(x)=f(x)-x$ est continue et strictement décroissante. Quand $x\to-\infty$, $h(x)\to+\infty$, et quand $x\to+\infty$, $h(x)\to-\infty$. Elle s’annule une fois exactement.

## Exercice 25

Si $f(f(a))=a$ et $f(a)=a$, c’est fini. Sinon, posons $b=f(a)\ne a$; alors $f(b)=a$. Si $a<b$, $f(a)-a>0$ et $f(b)-b<0$; si $b<a$, les signes sont inversés. Le TVI appliqué à $f(x)-x$ fournit un point fixe. Sans continuité, sur $\mathbb R$ on peut prendre une involution sans point fixe: $f(x)=x+1$ sur $[2k,2k+1[$ et $f(x)=x-1$ sur $[2k+1,2k+2[$ pour tout $k\in\mathbb Z$; alors $f^2=\mathrm{id}$ mais $f$ n’a aucun point fixe.

## Exercice 26

Choisissons $r$ tel que $\ell<r<1$. Pour $x$ assez grand, $f(x)\le rx<x$, donc $h(x)=f(x)-x<0$. En $0$, $h(0)=f(0)\ge0$. Le TVI donne un point fixe.

## Exercice 27

Posons $g(x)=f(x)-f(x+1/2)$. La périodicité donne $g(x+1/2)=-g(x)$. Si $g$ ne s’annulait pas sur $[x,x+1/2]$, le TVI imposerait un changement de signe sans zéro; donc il existe $x_0$ tel que $g(x_0)=0$.

## Exercice 28+

### 1

Poser $g(x)=f(x+1/n)-f(x)$ sur $[0,1-1/n]$. Si elle n'a pas de zéro, elle garde un signe strict, mais


```math
\sum_{k=0}^{n-1}g(k/n)=f(1)-f(0)=0,
```


contradiction. Pour $n=1$, prendre directement $x=0$.

### 2

Pour $\delta\in]0,1[$ dont l'inverse n'est pas entier, poser


```math
f(x)=\sin^2\left(\frac{\pi x}{\delta}\right)-x\sin^2\left(\frac\pi\delta\right).
```


Alors $f$ est continue et $f(0)=f(1)=0$. La périodicité de $\sin^2$ donne, pour $0\le x\le1-\delta$,


```math
f(x+\delta)-f(x)=-\delta\sin^2\left(\frac\pi\delta\right)<0.
```


L'équation n'a donc aucune solution.

## Exercice 29

La continuité permet de prolonger $f$ en une fonction continue sur $[a,b]$ avec $f(a)=f(b)=\ell$. Si $f$ était injective, une fonction continue injective sur un intervalle serait strictement monotone, ce qui est incompatible avec l’égalité des valeurs aux extrémités.

## Exercice 30

Une fonction continue injective sur $\mathbb R$ est strictement monotone. La composée de deux fonctions strictement monotones de même sens est croissante; ainsi $f\circ f$ est croissante, contrairement à $-\mathrm{id}$.

## Exercice 31

La fonction $g-f$ est continue strictement positive sur le compact $[a,b]$, donc atteint un minimum $\varepsilon>0$. Alors $f(x)+\varepsilon\le g(x)$ partout.

## Exercice 32

$f(\mathbb R)$ est borné; la continuité de $g$ borne $g$ sur l’adhérence compacte de cette image, donc $g\circ f$ est bornée. Comme $f$ est bornée sur tout $\mathbb R$, $f\circ g$ l’est aussi.

## Exercice 33

1. $f$ est bornée sur le compact $[0,T]$, donc sur $\mathbb R$ par périodicité.
2. Sur le cercle de longueur $T$, choisissons un point de maximum et un point de minimum. Les deux arcs qui les relient ont longueurs $d$ et $T-d$; l’un a longueur au plus $T/2$. Son image par continuité contient tous les niveaux entre le minimum et le maximum. En prolongeant cet arc à un intervalle de longueur $T/2$, on obtient $x$ tel que $f([x,x+T/2])=f[\mathbb R]$.

## Exercice 34

Une fonction continue périodique est bornée sur une période compacte; la périodicité étend cette borne à $\mathbb R$.

## Exercice 35

La grille $\{k/n:0\le k\le n\}$ devient dense dans $[0,1]$. Par continuité uniforme, le maximum de $f$ sur cette grille tend vers $\max_{[0,1]}f$.

## Exercice 36+

Il existe $R$ tel que $|x|\ge R$ entraîne $f(x)>f(0)$. Sur le compact $[-R,R]$, $f$ atteint son minimum; ce minimum est aussi le minimum global.

## Exercice 37

La fonction est bornée sur tout intervalle compact $[0,R]$. Pour $x$ assez grand, $|f(x)-\ell|<1$, ce qui borne la queue; donc $f$ est bornée.

## Exercice 38

La continuité de $f$ sur $[0,x]$ assure que $M(x)=\max_{0\le t\le x}f(t)$ est bien défini. L'inclusion $[0,x]\subset[0,y]$ pour $x\le y$ donne sa croissance.

Fixer $R>0$ et noter $\omega_R(h)=\sup\{|f(s)-f(t)|:s,t\in[0,R],\ |s-t|\le h\}$. La continuité uniforme sur ce compact donne $\omega_R(h)\to0$. Pour $0\le x\le y\le R$, si $t\le x$, alors $f(t)\le M(x)$ ; si $x\le t\le y$, alors $f(t)\le f(x)+\omega_R(y-x)\le M(x)+\omega_R(y-x)$. Ainsi


```math
0\le M(y)-M(x)\le\omega_R(y-x).
```


Donc $M$ est continue sur chaque $[0,R]$, puis sur $\mathbb R_+$.

## Exercice 39+

Si $f$ est injective, tout élément de son image a exactement un antécédent. Sinon, choisir $a<b$ avec $f(a)=f(b)=c$. La fonction n'est pas constante sur $[a,b]$, sinon la fibre de $c$ serait infinie. Quitte à remplacer $f$ par $-f$, son maximum $M$ sur $[a,b]$ vérifie $M>c$.

Ce maximum est atteint en un unique point de $]a,b[$. En effet, si $p<q$ étaient deux points de maximum, il existerait $r\in]p,q[$ avec $f(r)<M$, sinon la fibre de $M$ serait infinie. Choisir $t$ avec $\max(c,f(r))<t<M$. Le théorème des valeurs intermédiaires donnerait quatre antécédents distincts de $t$, dans $]a,p[$, $]p,r[$, $]r,q[$ et $]q,b[$, contradiction.

Enfin, aucun point extérieur à $[a,b]$ ne peut prendre la valeur $M$ : un niveau $t\in]c,M[$ aurait alors deux antécédents dans $]a,b[$ et un troisième entre cet autre point et l'extrémité voisine $a$ ou $b$. Ainsi $M$ possède exactement un antécédent dans $\mathbb R$.

## Exercice 40+

Non. Pour un irrationnel $\alpha\in(0,1)$, la fonction $f(q)=1/|q-\alpha|$ est continue sur $\mathbb Q\cap[0,1]$ relativement à ce domaine et non bornée.

## Exercice 41

Pour $x,y\ge0$, $|\sqrt x-\sqrt y|\le\sqrt{|x-y|}$; la fonction racine carrée est uniformément continue.

## Exercice 42

$f(x)=\sin(x^2)$ est bornée mais non uniformément continue: pour $x_n=\sqrt{2\pi n+\pi/2}$ et $y_n=\sqrt{2\pi n+3\pi/2}$, $|x_n-y_n|\to0$ alors que $|f(x_n)-f(y_n)|=2$.

## Exercice 43

Soit $\varepsilon>0$. Choisissons $R$ tel que $|f(x)|<\varepsilon/3$ pour $x\ge R$. Sur le compact $[0,R+1]$, $f$ est uniformément continue; choisissons $\delta<1$ correspondant à $\varepsilon$. Si $|x-y|<\delta$, soit les deux points sont dans ce compact, soit ils sont tous deux $>R$; dans le second cas $|f(x)-f(y)|<2\varepsilon/3$. Donc $f$ est uniformément continue.

## Exercice 44+

L'uniforme continuité fournit $\delta>0$ tel que $|f(x)-f(y)|\le1$ dès que $|x-y|<\delta$. Choisir un entier $N$ tel que $1/N<\delta$. En découpant $[x,x+1]$ en $N$ morceaux,


```math
|f(x+1)-f(x)|\le\sum_{j=0}^{N-1}|f(x+(j+1)/N)-f(x+j/N)|\le N.
```


Pour $x=n+r$, $n\in\mathbb N$, $0\le r<1$,


```math
f(x)\le f(r)+nN\le\max_{[0,1]}f+Nx.
```


On peut donc prendre $a=N$ et $b=\max_{[0,1]}f$.

## Exercice 45

Si $f(x)>g(x)$ pour tout $x$, choisir $x$ où $g$ atteint son maximum $M$: alors $f(x)>M$, contredisant $f[I]\subset g[I]\subset(-\infty,M]$. Si $f(x)<g(x)$ partout, un minimum de $g$ fournit la contradiction inverse. Donc $f-g$ s’annule.

## Exercice 46

Les deux fonctions atteignent leur maximum commun $M$. En un point $x$ où $f(x)=M$, $f(x)-g(x)\ge0$; en un point $y$ où $g(y)=M$, $f(y)-g(y)\le0$. Le TVI donne un zéro de $f-g$.

## Exercice 47+

Supposons qu’il n’existe aucun point où $f=g$. Par connexité, soit $f<g$ partout, soit $g<f$ partout. Supposons $f<g$. La fonction $f$ possède un point fixe $x_0$ puisque $f([0,1])\subset[0,1]$. Alors $g(x_0)>x_0$ et, par commutation, $f(g^n(x_0))=g^n(f(x_0))=g^n(x_0)$ pour tout $n$. La suite $g^n(x_0)$ croît strictement et est bornée par $1$; elle converge vers $L$. Par continuité, $g(L)=L$ et $f(L)=L$, contradiction à l’absence de point d’égalité. Le cas $g<f$ est symétrique.

## Exercice 48

L'énoncé est faux sans hypothèse de régularité. Compléter la famille $\mathbb Q$-libre $(1,\sqrt2)$ en une base de Hamel de $\mathbb R$ sur $\mathbb Q$. Définir l'application $\mathbb Q$-linéaire par $f(1)=0$, $f(\sqrt2)=1$ et $f(b)=0$ sur les autres éléments de cette base. Elle est additive. Si elle valait $\lambda x$, l'égalité $f(1)=0$ imposerait $\lambda=0$, contredisant $f(\sqrt2)=1$.

Avec l'hypothèse supplémentaire de continuité en $0$, l'additivité donne $f(q)=qf(1)$ pour tout rationnel $q$. Pour $q_n\in\mathbb Q$ tendant vers $x$,


```math
f(x)-q_nf(1)=f(x-q_n)\longrightarrow0,
```


donc $f(x)=xf(1)$.

## Exercice 49

Pour le carré ponctuel, $f(x)^2=f(x)$ équivaut à $f(x)\in\{0,1\}$. L'image continue de l'intervalle $\mathbb R$ est un intervalle ; elle est donc réduite à un point. Les solutions sont


```math
\boxed{f\equiv0\quad\text{ou}\quad f\equiv1}.
```



Si $f^2$ désigne plutôt l'itérée $f\circ f$, les solutions sont les rétractions continues sur les intervalles fermés non vides de $\mathbb R$. En effet, $I=f(\mathbb R)$ est un intervalle et $f_{|I}=\operatorname{id}_I$. Toute limite finie de points de $I$ est encore fixe par continuité, donc $I$ est fermé. Réciproquement, une fonction continue à valeurs dans un tel $I$, égale à l'identité sur $I$, vérifie $f\circ f=f$.

## Exercice 50

Pour tout $x$ et tout $n$, $f(x)=f(x/2^n)$. Comme $x/2^n\to0$ et $f$ est continue en $0$, $f(x)=f(0)$. La fonction est constante.

## Exercice 51+

Si $|x|<1$, les itérés successifs de $x\mapsto x^2$ tendent vers $0$, donc $f(x)=f(0)$. Si $x>1$, les racines carrées itérées tendent vers $1$ et $f(x)=f(\sqrt x)=f(\sqrt[4]x)=\cdots\to f(1)$. Pour $x<-1$, $f(x)=f(x^2)=f(1)$. La continuité en $1$ et en $0$ impose $f(0)=f(1)$; ainsi $f$ est constante.

## Exercice 52+

$f\circ f=\mathrm{id}$ rend $f$ injective; continue et injective sur un intervalle, elle est strictement monotone. Elle ne peut être décroissante sur $\mathbb R_+$: une fonction décroissante non négative y est bornée par $f(0)$, alors qu’elle est surjective. Elle est donc croissante; $f(f(x))=x$ et la croissance impliquent $f(x)=x$ (si $f(x)>x$, alors $f(f(x))>f(x)$; si $f(x)<x$, l’inégalité inverse donne aussi contradiction). Donc $f=\mathrm{id}$.

## Exercice 53+++

Poser $\alpha=(1+\sqrt5)/2$ et $\beta=(1-\sqrt5)/2$. Ces deux nombres vérifient $r^2=r+1$, donc $f(x)=\alpha x$ et $f(x)=\beta x$ conviennent.

Réciproquement, $f(a)=f(b)$ donne $f(f(a))=f(f(b))$, puis $f(a)+a=f(b)+b$ ; donc $a=b$. Ainsi $f$ est injective, puis strictement monotone par continuité. L'équation en $0$ donne $f(f(0))=f(0)$ ; l'injectivité implique $f(0)=0$.

La fonction est surjective. En effet, par monotonie, elle possède des limites aux deux infinis. Si l'une de ces limites était finie, disons $f(x)\to L$ lorsque $x\to+\infty$ ou $-\infty$, la continuité donnerait $f(f(x))\to f(L)$, tandis que $f(x)+x$ serait non borné. Les deux limites sont donc infinies et de signes opposés.

Pour $x\ne0$, définir $x_k=f^{\circ k}(x)$ pour tout $k\in\mathbb Z$, les itérées négatives utilisant l'inverse de $f$. L'équation donne


```math
x_{k+2}=x_{k+1}+x_k.
```


Il existe donc $A,B\in\mathbb R$ tels que $x_k=A\alpha^k+B\beta^k$ pour tout $k\in\mathbb Z$ ; les deux constantes sont déterminées par $x_0=x$ et $x_1=f(x)$.

Si $f$ est croissante, elle et son inverse préservent le signe. Tous les $x_k$ ont donc le signe de $x$. Lorsque $k\to-\infty$, $\alpha^k\to0$ tandis que $\beta^k$ alterne de signe et croît en valeur absolue. Il faut donc $B=0$, puis $f(x)=\alpha x$.

Si $f$ est décroissante, les $x_k$ alternent de signe. Lorsque $k\to+\infty$, $\alpha^k\to+\infty$ et $\beta^k\to0$. Si $A\ne0$, les $x_k$ auraient finalement un signe constant, contradiction. Donc $A=0$, puis $f(x)=\beta x$.



```math
\boxed{f(x)=\frac{1+\sqrt5}{2}x\quad(\forall x),\qquad\text{ou}\qquad f(x)=\frac{1-\sqrt5}{2}x\quad(\forall x)}.
```



## Exercice 54

Pour $0<a<b$, posons $h_n=(b-a)/n$ et $p_n=\lfloor a/h_n\rfloor$. La croissance de la suite $(f(kh_n))_{k\ge0}$ donne $f(p_nh_n)\le f((p_n+n)h_n)$. Or $p_nh_n\to a$ et $(p_n+n)h_n\to b$. Par continuité, $f(a)\le f(b)$; $f$ croît. Sans continuité, $f=\mathbf 1_{\mathbb R\setminus\mathbb Q}$ convient: pour $x$ rationnel, $f(nx)=0$; pour $x$ irrationnel, $f(nx)=1$, donc chaque suite est constante, mais $f$ n’est pas croissante.

## Exercice 55

### 1

Prendre $I_0=\mathbb R$, $I_1=[0,+\infty[$ et $I_2=[0,1]$. Tout intervalle non trivial est de l'un des trois types : aucune extrémité incluse, une extrémité incluse, ou deux extrémités incluses. Des changements affines, puis selon le cas $t\mapsto\tan t$, $t\mapsto\ln t$ ou $t\mapsto t/(1+t)$, donnent un homéomorphisme avec l'exemple correspondant.

Ces trois exemples ne sont pas homéomorphes : le nombre de points dont la suppression laisse l'espace connexe vaut respectivement $0,1,2$. Un homéomorphisme préserve cette propriété.

### 2

Pour une application surjective quelconque, il n'y a aucune restriction sur $(k,\ell)$ : chacun de ces intervalles a le cardinal de $\mathbb R$, donc il existe même une bijection $I_k\to I_\ell$.

## Exercice 56

Fixons $y\in\mathbb R$ et supposons que ses antécédents soient finis. Au-delà du plus grand antécédent, $f-y$ garde un signe constant par continuité. Si ce signe est positif, $f$ est minorée sur cette demi-droite; si négatif, elle y est majorée. Sur le segment initial, elle est bornée. Dans l’un ou l’autre cas, $f$ serait globalement minorée ou majorée, contrairement à sa surjectivité sur $\mathbb R$. Donc chaque réel est atteint une infinité de fois.

## Exercice 57+

Les hypothèses donnent


```math
f(\mathbb R)=f(\mathbb Q)\cup f(\mathbb R\setminus\mathbb Q)\subset f(\mathbb Q)\cup\mathbb Q.
```


Le membre de droite est dénombrable. Mais l'image continue de $\mathbb R$ est un intervalle ; un intervalle dénombrable est réduit à un point. Donc $f$ serait constante, de valeur $c$. Les deux inclusions imposeraient simultanément $c\notin\mathbb Q$ et $c\in\mathbb Q$, contradiction.

## Exercice 58+

Comme $\cos x_n\to0$, la distance de $x_n$ à l’ensemble $\{\pi/2+k\pi:k\in\mathbb Z\}$ tend vers $0$. Les écarts entre points consécutifs de cet ensemble valent $\pi$, alors que $x_{n+1}-x_n\to0$; l’indice $k$ du point le plus proche est donc constant à partir d’un rang. Ainsi $x_n$ converge vers ce point.

## Exercice 59+

Fixons $a<b$ et posons $S=\{t\in[a,b]: f(s)\ge f(a)\text{ pour tout }s\in[a,t]\}$. L’ensemble contient un voisinage à droite de $a$. Soit $c=\sup S$. La continuité assure $f(s)\ge f(a)$ pour $s\in[a,c]$; l’hypothèse locale en $c$ prolonge cette inégalité à droite, donc $c=b$. Ainsi $f(b)\ge f(a)$ et $f$ croît. Sans continuité, prendre $f(x)=0$ si $x<0$ et $f(x)=-1$ si $x\ge0$. Chaque point a un voisinage à droite où $f$ est constante, mais $f$ n’est pas croissante.

## Exercice 60

La fonction de Thomae est continue en tout irrationnel: pour $\varepsilon>0$, les rationnels de dénominateur réduit $q<1/\varepsilon$ sont localement évitables autour de l’irrationnel, et les autres ont valeur $1/q<\varepsilon$. Elle est discontinue en tout rationnel $p/q$, car sa valeur $1/q>0$ alors que des irrationnels tendant vers ce point ont valeur $0$.

## Exercice 61+

1. La fonction de Dirichlet $1_{\mathbb Q}$ est discontinue partout.
2. $f(x)=x\,1_{\mathbb Q}(x)$ est continue en $0$ puisque $|f(x)|\le|x|$. En tout $x\ne0$, les limites le long des rationnels et des irrationnels valent respectivement $x$ et $0$, donc elle est discontinue.
3. $f(x)=\operatorname{dist}(x,\mathbb Z)\,1_{\mathbb Q}(x)$. Aux entiers, $|f(x)|\le\operatorname{dist}(x,\mathbb Z)\to0$; hors des entiers, les limites le long des rationnels et irrationnels diffèrent. Elle est continue exactement sur $\mathbb Z$.

## Exercice 62+

En groupant les termes deux à deux,


```math
\left|\frac1n\sum_{k=1}^n(-1)^kf(k/n)\right|\le\frac1n\sum_{j=1}^{\lfloor n/2\rfloor}|f(2j/n)-f((2j-1)/n)|+\frac{\|f\|_\infty}{n}.
```


La continuité uniforme rend chaque différence $o(1)$ uniformément; la somme divisée par $n$ tend donc vers $0$.

## Exercice 63++

### 1

Poser $f(x)=1-x$ pour $x\le0$ et $f(x)=1/(x+1)$ pour $x\ge0$. Les deux expressions valent $1$ en $0$ ; $f$ est continue et non bornée en $-\infty$. Pour tout $x$, $f(x)>0$, donc


```math
f(f(x))=\frac1{1+f(x)}\in]0,1[.
```


La composée est bornée.

### 2

Poser $I=f(\mathbb R)$, $J=f(I)=f^{\circ2}(\mathbb R)$ et $K=f(J)=f^{\circ3}(\mathbb R)$. Ce sont des intervalles, avec $K\subset J\subset I$. Par hypothèse $K$ est borné, donc $f$ est bornée sur $J$.

Supposons $J$ non majoré. Il contient alors une demi-droite $[a,+\infty[$, sur laquelle $f$ est bornée. Comme $I$ est un intervalle non majoré, deux cas sont possibles.

Si $I$ est aussi non minoré, alors $I=\mathbb R$, d'où $J=I=\mathbb R$ et $K=\mathbb R$, contradiction.

Sinon $m=\inf I$ est fini. La fonction $f$ est bornée sur le compact $[\min(m,a),a]$, ainsi que sur $[a,+\infty[$ ; elle est donc bornée sur $I\subset[m,+\infty[$. Cela rend $J=f(I)$ borné, contradiction.

Le cas où $J$ est non minoré se traite symétriquement, avec une demi-droite $]-\infty,a]$ et, si nécessaire, la borne supérieure finie de $I$. Ainsi $J$ est borné, c'est-à-dire $f\circ f$ est bornée.
