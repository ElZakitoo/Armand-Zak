# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td18-fonctions-convexes.pdf)

## Autocorrection A

1. Pour $x,y\in I$ et $t\in[0,1]$,


```math
f((1-t)x+ty)\le(1-t)f(x)+tf(y).
```


La croissance de $g$ puis sa convexité donnent


```math
g(f((1-t)x+ty))\le g((1-t)f(x)+tf(y))\le(1-t)g(f(x))+tg(f(y)).
```


2. Si $f$ est concave et $g$ convexe décroissante, alors $g\circ f$ est convexe: $f((1-t)x+ty)\ge(1-t)f(x)+tf(y)$, puis appliquer $g$ décroissante et sa convexité. Si $f$ est concave et $g$ concave croissante, le même raisonnement donne la concavité de $g\circ f$.
3. $f(x)=x^2$ est convexe et $g(u)=e^{-u}$ convexe, mais $g\circ f=e^{-x^2}$ n’est pas convexe car $(g\circ f)''(0)=-2$.

## Autocorrection B

Une bijection convexe sur un intervalle est strictement monotone. Si $f$ est croissante, $f^{-1}$ est concave; si $f$ est décroissante, $f^{-1}$ est convexe. En effet, pour $u=f(x),v=f(y)$, la convexité de $f$ donne $f((1-t)x+ty)\le(1-t)u+tv$. Lorsque $f$ croît, appliquer $f^{-1}$ conserve l’ordre; lorsque $f$ décroît, elle l’inverse. Le résultat suit, en écrivant $x=f^{-1}(u),y=f^{-1}(v)$.

## Exercice 1

1. Si $f$ est convexe et concave, l’inégalité de Jensen est une égalité: $f((1-t)x+ty)=(1-t)f(x)+tf(y)$; en prenant $x,y$ fixes, $f$ est affine. Toute fonction affine est convexe et concave.
2. Les écarts de convexité de $f$ et $g$ sont positifs et leur somme vaut l’écart de convexité de $f+g$, nul puisque cette somme est affine. Chacun des deux écarts est donc nul pour tous $x,y,t$; $f$ et $g$ sont affines.

## Exercice 2

Si $f$ est convexe et impaire, $x\mapsto -f(-x)=f(x)$ est à la fois concave et convexe. Donc $f$ est affine; l’imparité impose $f(0)=0$, ainsi $f(x)=ax$, $a\in\mathbb R$. Toutes ces fonctions conviennent.

## Exercice 3

Une fonction polynomiale est convexe sur $\mathbb R$ si et seulement si $P''(x)\ge0$ pour tout $x$. Si $\deg P$ est impair et au moins $3$, alors $P''$ est de degré impair et change de signe à l’infini. Cela est impossible. Les seuls cas convexes sont les polynômes de degré $1$.

## Exercice 4+

Posons $h(x)=f(1/x)$. Alors $x f(x)=x h(1/x)$. Pour $u,v>0$ et $t\in[0,1]$, avec $w=(1-t)u+tv$,


```math
w h(1/w)=w h\!\left(\frac{(1-t)u}{w}\frac1u+\frac{tv}{w}\frac1v\right)
\le(1-t)u h(1/u)+tv h(1/v),
```


par convexité de $h$, car les deux coefficients à l’intérieur somment à $1$. Ainsi $h$ convexe implique $x\mapsto xf(x)$ convexe. Réciproquement, $h(x)=x g(1/x)$ pour $g(u)=u f(u)$; le même argument montre que la convexité de $g$ implique celle de $h$.

## Exercice 5

1. Si $f'$ croît strictement, le théorème des accroissements finis appliqué sur $[a,(1-t)a+tb]$ et $[(1-t)a+tb,b]$ compare les deux pentes sécantes et donne la stricte convexité. Inversement, si $f$ est strictement convexe et $a<b$, les pentes sécantes de $f$ sur $[a,b]$ sont strictement croissantes; en faisant tendre les extrémités vers $a,b$, $f'(a)<f'(b)$.
2. L’inégalité stricte de Jensen donne


```math
f\left(\sum_i\lambda_i a_i\right)<\sum_i\lambda_i f(a_i)
```


dès que deux des $a_i$ diffèrent, puisque tous les poids sont positifs. L’égalité imposée entraîne $a_1=\cdots=a_n$.
3. Appliquer Jensen à la fonction strictement convexe $x\mapsto-\ln x$ aux nombres $1,2,\ldots,n$:


```math
\frac1n\sum_{k=1}^n-\ln k\ge-\ln\left(\frac{n+1}{2}\right).
```


Donc $n!\le((n+1)/2)^n$. L’égalité n’a lieu que si $n=1$.

## Exercice 6+

Par récurrence, l’inégalité médiane implique, pour tout dyadique $t=k/2^m$,


```math
f((1-t)a+tb)\le(1-t)f(a)+tf(b).
```


La continuité de $f$ et la densité des dyadiques étendent l’inégalité à tout $t\in[0,1]$; $f$ est convexe.

## Exercice 7

Pour tout $x,y\in I$, l’hypothèse donne $f(y)\ge f(x)+f'(x)(y-x)$. Pour $z=(1-t)x+ty$, multiplier les deux inégalités (tangentes en $z$) par $1-t$ et $t$, puis sommer:


```math
(1-t)f(x)+tf(y)\ge f(z)+f'(z)((1-t)(x-z)+t(y-z))=f(z).
```



## Autocorrection C

Soient $0\le x\le y$. Écrire $a\pm x$ comme combinaisons convexes de $a-y$ et $a+y$ et additionner les deux inégalités de convexité; on obtient $f(a-x)+f(a+x)\le f(a-y)+f(a+y)$. Donc $g$ croît.

## Exercice 8

Pour $s=x+y>0$, la concavité et $f(0)\ge0$ donnent


```math
f(x)\ge\frac{x}{s}f(s),\qquad f(y)\ge\frac{y}{s}f(s).
```


En sommant, $f(x)+f(y)\ge f(x+y)$. Si $s=0$, l’assertion est immédiate.

## Exercice 9

1. Si $f$ n’est pas constante, il existe $a<b$ tels que la pente $m=(f(b)-f(a))/(b-a)$ est non nulle. La convexité compare toutes les pentes sécantes à $m$: pour $x>b$, $f(x)\ge f(b)+m(x-b)$; pour $x<a$, $f(x)\ge f(a)+m(x-a)$. Selon le signe de $m$, l’une de ces bornes tend vers $+\infty$, contredisant la majoration.
2. Non: $f(x)=-x$ est convexe et majorée par $0$ sur $\mathbb R_+$, sans être constante.

## Exercice 10

1. Un extremum local d’une convexe ne peut être un maximum strict; si $x_0$ est un extremum local, c’est un minimum. Si $f(y)<f(x_0)$ pour un $y$, alors pour $t>0$ assez petit, $f((1-t)x_0+ty)\le(1-t)f(x_0)+tf(y)<f(x_0)$, contradiction au minimum local. Donc $x_0$ est minimum global.
2. L’ensemble des minimiseurs est un intervalle: si $x,y$ minimisent $f$, la convexité donne $f((1-t)x+ty)\le\min f$, donc égalité. Il peut être vide, un singleton ou un intervalle (relativement à $I$).

## Autocorrection D

Par AM-GM,


```math
\sum_{i=1}^n\frac1{x_i}\ge n\left(\prod_i\frac1{x_i}\right)^{1/n}=\frac n{(x_1\cdots x_n)^{1/n}}.
```


Réarranger donne l’inégalité voulue.

## Autocorrection E

La fonction $x\mapsto x^n$ est convexe sur $\mathbb R_+$ pour $n\ge1$; la convexité à poids $1/2$ donne $(\frac{x+y}{2})^n\le\frac{x^n+y^n}{2}$, soit $(x+y)^n\le2^{n-1}(x^n+y^n)$. Pour $n=0$, égalité.

## Exercice 11

Poser $u_i=\ln r_i\ge0$ et $\phi(u)=1/(1+e^u)$. On a


```math
\phi''(u)=\frac{e^u(e^u-1)}{(1+e^u)^3}\ge0.
```


Jensen donne


```math
\frac1{1+\sqrt[n]{r_1\cdots r_n}}=\phi\left(\frac1n\sum_i u_i\right)\le\frac1n\sum_i\phi(u_i),
```


ce qui est l’assertion.

## Exercice 12

La droite passant par $(-A,e^{-A})$ et $(A,e^A)$ est au-dessus du graphe convexe de l’exponentielle:


```math
e^x\le \frac{\sinh A}{A}x+\cosh A\quad(-A\le x\le A).
```


Cette droite minimise l’ordonnée à l’origine parmi les majorants affines: les deux contraintes aux extrémités imposent $\mu\ge\max(e^{-A}+A\lambda,e^A-A\lambda)$, dont le minimum est $\cosh A$, atteint pour $\lambda=\sinh A/A$. Pour $A=0$, prendre $(\lambda,\mu)=(1,1)$.

## Exercice 13

La fonction $\phi(t)=1/(1+\sin t)$ est convexe sur $]0,\pi[$, car


```math
\phi''(t)=\frac{2+\sin t-\sin^2t}{(1+\sin t)^3}>0.
```


Comme $\alpha+\beta+\gamma=\pi$, Jensen donne


```math
\sum_{cyc}\frac1{1+\sin\alpha}\ge3\phi(\pi/3)=\frac6{2+\sqrt3}.
```



## Exercice 14

Soient $\theta_i$ les angles au centre correspondant aux côtés, $\theta_i\in(0,2\pi)$ et $\sum_i\theta_i=2\pi$. L’aire est $\frac{R^2}{2}\sum_i\sin\theta_i$. Posons $c=2\pi/n\le\pi/2$. Pour tout $t\in[0,2\pi]$,


```math
\sin t\le\sin c+\cos c(t-c);
```


sur $[0,\pi]$ c’est la tangente à une fonction concave, et sur $[\pi,2\pi]$ le membre droit est au moins $0$ tandis que $\sin t\le0$. En sommant, $\sum_i\sin\theta_i\le n\sin(2\pi/n)$, avec égalité si tous les $\theta_i=2\pi/n$. Le polygone régulier maximise donc l’aire.

## Exercice 15+

1. Les poids $23/51,7/51,11/51,10/51$ somment à $1$ et vérifient


```math
\frac{23}{51}(4,1,0,0)+\frac7{51}(0,4,1,0)+\frac{11}{51}(0,0,4,1)+\frac{10}{51}(1,0,0,4)=(2,1,1,1).
```


L’AM-GM pondérée appliquée aux quatre monômes donne


```math
x^2yzt\le\frac{23}{51}x^4y+\frac7{51}y^4z+\frac{11}{51}z^4t+\frac{10}{51}t^4x.
```


2. L’assertion imprimée est fausse. Prendre $(x,y,z,t)=(10,1/2,100,1/500)$ donne $xyzt=1$, mais


```math
x+y+z+t=110.502>50+25+20+0.00004=x^2y+y^2z+z^2t+t^2x.
```



## Exercice 16++

Posons $m=(x+y+z)/3$ et $g(u)=f(m+u)-f(m)$. Alors $g$ est convexe et $g(0)=0$. Posons $u=x-m$, $v=y-m$, $w=z-m$, donc $u+v+w=0$. Il suffit de montrer


```math
2\sum_{cyc}g\left(-\frac u2\right)\le g(u)+g(v)+g(w).
```


Parmi $u,v,w$, deux sont de même signe. Si $u,v\ge0$ et $w=-(u+v)$, convexité et $g(0)=0$ donnent $2g(-u/2)\le g(-u)$, $2g(-v/2)\le g(-v)$ et $2g((u+v)/2)\le g(u)+g(v)$. De plus, $g(-u)\le\frac{u}{u+v}g(-(u+v))$ et $g(-v)\le\frac{v}{u+v}g(-(u+v))$, donc $g(-u)+g(-v)\le g(w)$.

Si $u=-a,v=-b,w=a+b$ avec $a,b\ge0$, alors $2g(a/2)\le g(a)$, $2g(b/2)\le g(b)$ et $2g(-(a+b)/2)\le g(-a)+g(-b)$. Par convexité depuis 0, $g(a)+g(b)\le g(a+b)$. Dans les deux cas, en sommant, on obtient l’inégalité. Les cas où un terme est nul sont inclus dans ces deux configurations.

## Exercice 17+

1. La convexité de $t\mapsto t^p/p$ (ou l’AM-GM pondérée) donne, pour $A,B\ge0$,


```math
A^{1/p}B^{1/q}\le\frac Ap+\frac Bq.
```


Prendre $A=a$, $B=b$.
2. (a) Si $\|x\|_p=\|y\|_q=1$, Young appliquée à $|x_i|^p,|y_i|^q$ donne $|x_i y_i|\le |x_i|^p/p+|y_i|^q/q$. Sommer puis $\sum x_i y_i\le\sum|x_i y_i|$ donne la borne $1$.
(b) Si les normes sont non nulles, appliquer (a) aux vecteurs normalisés $x/\|x\|_p,y/\|y\|_q$; les cas nuls sont immédiats.
(c) Oui, avec $q=\infty$: $\sum|x_i y_i|\le\|y\|_\infty\sum|x_i|$.
3. (a) Multiplier $|x_i+y_i|\le|x_i|+|y_i|$ par $|x_i+y_i|^{p-1}$, puis sommer.
(b) Hölder appliquée aux deux sommes de (a) donne


```math
\|x+y\|_p^p\le(\|x\|_p+\|y\|_p)\|x+y\|_p^{p-1}.
```


Si $\|x+y\|_p>0$, diviser; sinon c’est immédiat.

## Exercice 18+

Définir


```math
g(x)=\inf\left\{\sum_{i=1}^m\lambda_i f(x_i):m\ge1,\ \lambda_i\ge0,\ \sum_i\lambda_i=1,\ \sum_i\lambda_i x_i=x\right\}.
```


L’ensemble est non vide (prendre $m=1,x_1=x$), et $0\le g(x)\le f(x)$. En concaténant des combinaisons admissibles pour deux points et en multipliant leurs poids par $1-t,t$, on obtient la convexité de $g$. Si $h$ est convexe et $h\le f$, Jensen donne $h(x)\le\sum_i\lambda_i f(x_i)$ pour chaque combinaison; donc $h(x)\le g(x)$. Ainsi $g$ est le plus grand minorant convexe.

## Exercice 19+

1. Si $f$ est log-convexe,


```math
f((1-t)x+ty)\le f(x)^{1-t}f(y)^t\le(1-t)f(x)+tf(y),
```


donc $f$ est convexe. La réciproque est fausse: $f(x)=1+x^2$ est convexe positive, mais $(\ln f)''=2(1-x^2)/(1+x^2)^2<0$ si $|x|>1$.
2. Si $f$ est log-convexe, $f^\alpha$ l’est pour tout $\alpha>0$, donc convexe. Réciproquement, poser $z=(1-t)x+ty$; de la convexité de $f^\alpha$,


```math
f(z)^\alpha\le(1-t)f(x)^\alpha+tf(y)^\alpha.
```


Prendre le logarithme, diviser par $\alpha$, puis faire tendre $\alpha\to0^+$; le développement $u^\alpha=1+\alpha\ln u+o(\alpha)$ donne $\ln f(z)\le(1-t)\ln f(x)+t\ln f(y)$.
3. La log-convexité de $f$ implique celle de $e^{\beta x}f(x)$, donc sa convexité. Réciproquement, pour tout $\beta$,


```math
f(z)\le(1-t)e^{\beta t(x-y)}f(x)+t e^{-\beta(1-t)(x-y)}f(y).
```


Le minimum du membre droit sur $\beta\in\mathbb R$ vaut $f(x)^{1-t}f(y)^t$ (pour $x\ne y$), d’où la log-convexité; $x=y$ est immédiat.
4. Le produit est log-convexe car son logarithme est la somme des logarithmes. Pour la somme, Hölder donne


```math
f(z)+g(z)\le f(x)^{1-t}f(y)^t+g(x)^{1-t}g(y)^t\le(f(x)+g(x))^{1-t}(f(y)+g(y))^t.
```



## Exercice 20+

Supposons par l’absurde $f f'f''f'''<0$ partout. Aucun facteur ne s’annule et chacun garde un signe constant. Remplacer f par −f laisse le produit inchangé; on peut supposer $f>0$. Si $f'>0$, remplacer f(x) par f(−x) conserve le produit et donne $f'<0$. Alors $f''f'''>0$. Si $f'',f'''>0$, alors $f''(x)\ge f''(0)>0$ pour x≥0, donc $f'(x)\ge f'(0)+xf''(0)$, qui devient positif : contradiction. Si $f'',f'''<0$, alors $f'(x)\le f'(0)<0$ pour x≥0, donc $f(x)\le f(0)+xf'(0)$, qui devient négatif : contradiction. Il existe donc a tel que $f(a)f'(a)f''(a)f'''(a)\ge0$.

## Exercice 21++

Pour chaque $x$, les paramètres donnant $(1-\lambda)f(x)+\lambda g(x)\ge0$ forment un intervalle fermé $I_x\subset[0,1]$, non vide puisque $\max(f(x),g(x))\ge0$. Si $f(x)<0\le g(x)$, alors $I_x=[L_x,1]$ avec $L_x=-f(x)/(g(x)-f(x))$; si $g(x)<0\le f(x)$, alors $I_x=[0,U_x]$ avec $U_x=f(x)/(f(x)-g(x))$; sinon $I_x=[0,1]$.

Montrons que toute borne inférieure $L_x$ est inférieure ou égale à toute borne supérieure $U_y$. Sinon, posons $a=-f(x)>0$, $b=g(x)\ge0$, $c=f(y)\ge0$, $d=-g(y)>0$. L’inégalité $L_x>U_y$ équivaut à $ad>bc$. On peut alors choisir


```math
\frac b{b+d}<t<\frac a{a+c}.
```


Pour $z=(1-t)x+ty$, la convexité donne


```math
f(z)\le-(1-t)a+tc<0,\qquad g(z)\le(1-t)b-td<0,
```


en contradiction avec $\max(f(z),g(z))\ge0$. Ainsi $\sup_xL_x\le\inf_yU_y$ (en omettant les bornes absentes). Tout $\lambda$ entre ces deux nombres appartient à chaque $I_x$ et convient.
