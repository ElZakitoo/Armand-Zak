# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td08-fonctions-reelles.pdf)

## Autocorrection A

1. La somme est paire pour deux fonctions paires ou deux fonctions impaires; avec une paire et une impaire, aucune parité n'est imposée.
2. Le produit est pair pour deux fonctions de même parité, impair pour une paire et une impaire.
3. Pour h∘f : si h est paire ou f est paire, la composée est paire; si h et f sont impaires, elle est impaire. Sinon, la parité n'est pas déterminée.
4. Si f est paire, h∘f est paire pour tout h. Si f est impaire et h est paire (resp. impaire), h∘f est paire (resp. impaire); sans hypothèse sur la parité de h, aucune parité n'est imposée.
5. La parité de f∘h n'est pas déterminée par celle de f seule. Si h est paire, f∘h est paire; si h est impaire, f∘h a la parité de f.

## Exercice 1

Puisque f³ est strictement décroissante, si x<y alors f³(x)>f³(y). Si f(x)≤f(y), la croissance de f² donnerait


```math
f^3(x)=f^2(f(x))\le f^2(f(y))=f^3(y),
```


contradiction. Donc x<y⇒f(x)>f(y), et f est strictement décroissante.

## Exercice 2

Pour tout k∈Z, $\cos(x+2k\pi)=\cos x$. Ainsi $x\in\cos^{-1}[A]\iff x+2k\pi\in\cos^{-1}[A]$; le domaine est 2π-périodique.

## Exercice 3+

1. Si α=p/q∈Q avec q>0, 2πq est une période. Réciproquement, si T>0 est une période, l'identité


```math
\cos(x+T)-\cos x+\cos(\alpha x+\alpha T)-\cos(\alpha x)=0
```


et la linéarité indépendante des fonctions trigonométriques de fréquences distinctes imposent, pour α≠0,±1, $T\in2\pi\mathbb Z$ et $\alpha T\in2\pi\mathbb Z$. Donc α∈Q. Les cas α=0,±1 sont rationnels.
2. Le raisonnement est identique avec les sinus : pour α≠0,±1, une période commune impose les mêmes conditions; α=0 ou ±1 donnent des fonctions périodiques. En sens direct, si α∈Q, la période 2πq convient.

## Exercice 4

1. $D$ est invariant par translation de T ssi $x\in D\iff x+T\in D$, exactement la condition $1_D(x+T)=1_D(x)$.
2. $1_D$ est paire ssi $x\in D\iff -x\in D$, soit $D=-D$.
3. Une fonction indicatrice impaire doit être nulle : si $1_D(x)=1$, l'imparité donnerait $1_D(-x)=-1$, impossible. Donc ssi $D=\varnothing$.
4. $1_D$ est croissante ssi $x\in D,,y\ge x\Rightarrow y\in D$, c'est-à-dire si D est une partie supérieure de R.

## Exercice 5

Soient deux centres distincts $(a,b),(c,d)$. La symétrie centrale donne $f(2a-x)=2b-f(x)$ et $f(2c-x)=2d-f(x)$. En composant,


```math
f(x+2(c-a))=f(x)+2(d-b).
```


Posons $T=2(c-a)\ne0$, $m=2(d-b)/T$, et $g(x)=f(x)-mx$. Alors $g(x+T)=g(x)$. Donc f est affine plus périodique.

## Autocorrection B

L'expression est $x^{\ln(\ln x)/\ln x}$. Il faut $x>1$, domaine de $\ln(\ln x)$; le dénominateur est alors non nul. Ainsi


```math
x^{\ln(\ln x)/\ln x}=\exp\!\left(\ln x\,\frac{\ln(\ln x)}{\ln x}\right)=\ln x\qquad(x>1).
```



## Exercice 6

Si le marcheur avance à 1 m/s et que l'abscisse x est mesurée en mètres, sa position sur la courbe y=eˣ est à hauteur eˣ mètres et la pente vaut eˣ. À x=20, $e^{20}>3\cdot10^8$ (par exemple $e>2.7$, donc $e^{20}>2.7^{20}>3\cdot10^8$). Une progression horizontale à 1 m/s correspond donc à une vitesse verticale instantanée supérieure à celle de la lumière. La hauteur e²⁰ mètres dépasse aussi la distance moyenne Terre-Lune.

## Exercice 7

À x=0, l'égalité vaut 1=1. La fonction $a^x-(x+1)$ a donc un minimum nul en 0 si l'inégalité est vraie partout; sa dérivée en 0 doit être nulle, donc $\ln a-1=0$, soit a=e. Réciproquement, la convexité de l'exponentielle donne $e^x\ge1+x$ pour tout x.

## Exercice 8

Le nombre de chiffres vaut $\lfloor\log_{10}(2^{82589933}-1)\rfloor+1$. Or $2^{82589933}-1$ est compris entre $10^{24862047}$ et $10^{24862048}$ (calcul de $82589933\log_{10}2=24862047.172878\ldots$). Il a donc 24 862 048 chiffres.

## Exercice 9

Posons $K=\lfloor1777\log_{10}304\rfloor$. Le nombre $304^{1777}$ a K+1 chiffres. La suite $\lfloor n\log_{10}2\rfloor$ part de 0, tend vers l'infini et augmente à chaque étape de 0 ou 1 puisque $0<\log_{10}2<1$. Elle prend donc la valeur K pour un entier n. Alors $2^n$ a le même nombre de chiffres.

## Exercice 10+

Supposons $e^x=f_1(x)+\cdots+f_m(x)$, avec période positive T_i pour chaque f_i. Notons $\tau_T f(x)=f(x+T)$. L'opérateur $\tau_{T_i}-I$ annule f_i; les opérateurs de translation commutent. Ainsi $\prod_{i=1}^m(\tau_{T_i}-I)$ annule la somme. Or sur $e^x$, cet opérateur donne


```math
\left(\prod_{i=1}^m(e^{T_i}-1)\right)e^x\ne0,
```


contradiction.

## Exercice 11



```math
2^{x+4}+3^x=2^{x+2}+3^{x+2}\iff12\,2^x=8\,3^x\iff(3/2)^x=3/2\iff x=1.
```



## Exercice 12+

1. En divisant les deux égalités, $4^x=2^y$, donc $y=2x$. La seconde devient $2^x=5^{2x}$, soit $(2/25)^x=1$; ainsi $(x,y)=(0,0)$.
2. Il faut a>0. Posons L=ln a. Les équations équivalent à $x+2y=L$, $xy=1/2$, donc $4y^2-2Ly+1=0$. Il existe des solutions ssi $|L|\ge2$. Dans ce cas


```math
y=\frac{L\pm\sqrt{L^2-4}}4,\qquad x=\frac{L\mp\sqrt{L^2-4}}2.
```



## Exercice 13+

Les logarithmes imposent x,y>0 et donnent $x^2=2y^3$, tandis que $x-y=2$. Ainsi


```math
2y^3-y^2-4y-4=0\iff(y-2)(2y^2+3y+2)=0.
```


Le second facteur n'a pas de racine réelle (discriminant −7); donc y=2, x=4.

## Exercice 14

Pour x>1,


```math
\ln(x-1)+\ln(x+1)<2\ln x-1\iff\ln(x^2-1)<\ln(x^2/e)\iff x^2<\frac e{e-1}.
```


Les solutions sont $1<x<\sqrt{e/(e-1)}$.

## Exercice 15

1. Avec $\operatorname{ch}x=(e^x+e^{-x})/2$ et $\operatorname{sh}x=(e^x-e^{-x})/2$, développer les produits donne


```math
\operatorname{ch}(x+y)=\operatorname{ch}x\operatorname{ch}y+\operatorname{sh}x\operatorname{sh}y,
\quad\operatorname{sh}(x+y)=\operatorname{ch}x\operatorname{sh}y+\operatorname{sh}x\operatorname{ch}y.
```


2. (a) $\operatorname{th}(x+y)=\frac{\operatorname{th}x+\operatorname{th}y}{1+\operatorname{th}x\operatorname{th}y}$. (b) Pour |a|,|b|<1, $1+ab>0$ et $(1+ab)^2-(a+b)^2=(1-a^2)(1-b^2)>0$; donc $|(a+b)/(1+ab)|<1$.

## Exercice 16

$\operatorname{ch}x+\operatorname{sh}x=e^x$, donc $(\operatorname{ch}x+\operatorname{sh}x)^p=e^{px}=\operatorname{ch}(px)+\operatorname{sh}(px)$.

## Exercice 17

Pour x≠0, appliquer n fois $\operatorname{sh}t=2\operatorname{sh}(t/2)\operatorname{ch}(t/2)$ donne


```math
2^n\prod_{k=1}^n\operatorname{ch}(x/2^k)=\frac{\operatorname{sh}x}{\operatorname{sh}(x/2^n)}.
```


Pour x=0, le produit vaut $2^n$.

## Exercice 18

L'équation équivaut à $(a+b)e^{2x}=b-a$. Si a=b=0, tout x convient. Sinon, une solution existe ssi $(b-a)/(a+b)>0$, soit $|b|>|a|$; elle est alors unique et vaut


```math
x=\frac12\ln\frac{b-a}{a+b}.
```



## Exercice 19

Si y≠0, les sommes géométriques de $e^{x+ky}$ et $e^{-x-ky}$ donnent


```math
\sum_{k=0}^n\operatorname{ch}(x+ky)=\frac{\operatorname{sh}((n+1)y/2)}{\operatorname{sh}(y/2)}\operatorname{ch}(x+ny/2),
```




```math
\sum_{k=0}^n\operatorname{sh}(x+ky)=\frac{\operatorname{sh}((n+1)y/2)}{\operatorname{sh}(y/2)}\operatorname{sh}(x+ny/2).
```


Pour y=0, elles valent respectivement $(n+1)\operatorname{ch}x$ et $(n+1)\operatorname{sh}x$.

## Exercice 20

1. $\sin p+\sin q=2\sin((p+q)/2)\cos((p-q)/2)$, donc la somme est non nulle ssi les deux facteurs sont non nuls.
2. Sous cette condition,


```math
\frac{\cos p-\cos q}{\sin p+\sin q}=-\tan\frac{p-q}2.
```


3. Prendre p=π/4, q=π/3 donne $\tan(\pi/24)$. Par la formule de l'angle moitié, $\tan(\pi/24)=\sqrt6+\sqrt2-\sqrt3-2$.

## Exercice 21

Pour x∈[−1,1], $\arccos(-x)=\pi-\arccos x$. Le graphe est invariant par la symétrie centrale de centre $(0,\pi/2)$.

## Exercice 22

1. Si A=arctan(√2), alors A∈(π/4,π/2) et $\tan(2A)=-2\sqrt2$. Donc $\arctan(2\sqrt2)=\pi-2A$, d'où la somme demandée vaut π.
2. Pour t>0, $\arctan t+\arctan(1/t)=\pi/2$. La somme cherchée est donc $\pi/2+\pi-\bigl(\arctan(2\sqrt2)+2\arctan(\sqrt2)\bigr)=\pi/2$.

## Exercice 23

(i) $2\ln\frac1{2-x}=-2\ln(2-x)$, domaine ]−∞,2[; fonction strictement croissante, zéro en 1 et limite +∞ en 2−. (ii) $\sqrt[3]{x-2}-1$, domaine R, graphe de la racine cubique translaté de (2,1). (iii) $4/(2x+1)+3$, domaine R\{−1/2}; asymptotes x=−1/2 et y=3.

## Exercice 24

(i) $f(x)=x^3/(x^2-3)$, $D=\mathbb R\setminus\{\pm\sqrt3\}$. Fonction impaire, asymptote oblique $y=x$, asymptotes verticales $x=\pm\sqrt3$.


```math
f'(x)=\frac{x^2(x^2-9)}{(x^2-3)^2}.
```


Donc $f$ croît sur $]-\infty,-3]$ et $[3,+\infty[$, décroît sur $[-3,-\sqrt3[$, $]-\sqrt3,\sqrt3[$ et $]\sqrt3,3]$. Aux points $\pm3$, $f(-3)=-9/2$, $f(3)=9/2$; $f(0)=0$.

(ii) $f(x)=\ln(x^2-1)$, $D=]-\infty,-1[\cup]1,+\infty[$, fonction paire,


```math
f'(x)=\frac{2x}{x^2-1}.
```


Elle décroît de $+\infty$ à $-\infty$ sur $]-\infty,-1[$, puis croît de $-\infty$ à $+\infty$ sur $]1,+\infty[$.

(iii) $f(x)=\sqrt{\ln|x|/x}$. La condition $\ln|x|/x\ge0$ donne $D=[-1,0[\cup[1,+\infty[$. Sur $]-1,0[\cup]1,+\infty[$,


```math
f'(x)=\frac{1-\ln|x|}{2x^2\sqrt{\ln|x|/x}}.
```


Ainsi $f$ croît sur $[-1,0[$ et $[1,e]$, puis décroît sur $[e,+\infty[$, avec $f(-1)=f(1)=0$, $f(e)=1/\sqrt e$, $\lim_{x\to0^-}f(x)=+\infty$, et $\lim_{x\to+\infty}f(x)=0$.

(iv) $f(x)=\tan(2x)/\tan x=2/(1-\tan^2x)$, sur


```math
D=\mathbb R\setminus\bigl(\{k\pi/2:k\in\mathbb Z\}\cup\{\pi/4+k\pi/2:k\in\mathbb Z\}\bigr).
```


La fonction est $\pi$-périodique et paire. Les points $x=k\pi$ sont des trous amovibles (limite 2), les points $x=\pi/2+k\pi$ sont des trous amovibles (limite 0), et $x=\pi/4+k\pi/2$ sont des pôles. Sur son domaine,


```math
f'(x)=\frac{4\tan x(1+\tan^2x)}{(1-\tan^2x)^2},
```


donc elle est strictement décroissante là où $\tan x<0$, croissante là où $\tan x>0$; les pôles sont les points exclus $\pi/4+k\pi/2$.

(v) $f(x)=x\arctan(1/x)$, $D=\mathbb R^*$; elle est paire. Pour $x\ne0$,


```math
f'(x)=\arctan(1/x)-\frac{x}{1+x^2}.
```


Cette dérivée a le signe de $x$, car pour $u>0$, $\arctan u>u/(1+u^2)$. Donc $f$ décroît sur $]-\infty,0[$, croît sur $]0,+\infty[$, avec limites $1$ à $\pm\infty$ et $0$ en $0$.

(vi) $f(x)=\sin(3x)+3\sin x=2\sin x(3-2\sin^2x)$. Le facteur $3-2\sin^2x$ est strictement positif; les zéros sont $k\pi$ et le signe est celui de $\sin x$. En dérivant,


```math
f'(x)=3\cos(3x)+3\cos x=6\cos x\cos(2x).
```


La fonction est $2\pi$-périodique. Sur $[0,2\pi]$, $(f')(x)=6\cos x\cos(2x)$ est successivement de signe $+,-,+,-,+,-,+$ sur les intervalles séparés par $0,\pi/4,\pi/2,3\pi/4,5\pi/4,3\pi/2,7\pi/4,2\pi$. Les valeurs aux points critiques sont respectivement $2\sqrt2,2,2\sqrt2,-2\sqrt2,-2,-2\sqrt2$; aux bornes $f(0)=f(2\pi)=0$.

## Exercice 25+

La fonction $\phi(t)=te^t$ est strictement croissante sur $\mathbb R_+$, car $\phi'(t)=e^t(1+t)>0$. De $W(x)e^{W(x)}=x$, soit $\phi(W(x))=x$, on déduit que W=φ⁻¹ est strictement croissante.

## Exercice 26+

1. Poser t=e^x>0 : $(a-1)t^2+(b-2)t+(c+1)=0$ pour tout t>0, donc $(a,b,c)=(1,2,-1)$.
2. Comme $\arcsin x=\pi/2-\arccos x$, l'identité équivaut à $(a-b+1)\arccos x+(b\pi/2+c-\pi+1)=0$ pour tout x. Donc $a-b=-1$ et $b\pi/2+c=\pi-1$. Les solutions sont $(a,b,c)=(t-1,t,\pi-1-t\pi/2)$, t∈R.

## Exercice 27+

1. Poser θ=arctan(sh x). Alors $\sin \theta=\operatorname{th}x$, puisque $\sqrt{1+\operatorname{sh}^2x}=\operatorname{ch}x>0$. Ainsi $\arccos(\operatorname{th}x)=\pi/2-\theta$, et la somme vaut π/2.
2. $\operatorname{th}x=5/13$ donne $e^{2x}=9/4$, donc $x=\ln(3/2)$.
3. Le triangle rectangle de côtés 5,12,13 donne $\sin(\arctan(5/12))=5/13$, donc les angles sont complémentaires.

## Exercice 28

1. Posons A=arctan a, B=arctan b. Si ab<1, la somme A+B∈(−π/2,π/2), donc $\arctan a+\arctan b=\arctan((a+b)/(1-ab))$. Si ab>1, le membre gauche diffère de cette arctangente de ±π selon le signe de a+b; le cas a+b=0 donne 0.
2. Pour x≠1, $(1+x)/(1-x)$ : si x<1, $\arctan((1+x)/(1-x))=\pi/4+\arctan x$; si x>1, la valeur est $-3\pi/4+\arctan x$. En x=1, l'expression n'a pas de sens.

## Exercice 29

1. Posons θ=arctan(1/√n)∈(0,π/2). Alors $\sin \theta=1/\sqrt{n+1}$, car $\sin \theta=\tan \theta/\sqrt{1+\tan^2\theta}$. D'où l'égalité.
2. Le triangle rectangle de côtés $1,\sqrt n,\sqrt{n+1}$ donne directement $\tan \theta=1/\sqrt n$ et $\sin \theta=1/\sqrt{n+1}$; θ est dans ]0,π/2[, donc les valeurs principales sont égales.

## Exercice 30

1. Domaine $\cos x\ne0,\sin x\ne1$. La différence vaut $(1+\sin x)/\cos x-\cos x/(1-\sin x)=0$, car $\cos^2x=(1-\sin x)(1+\sin x)$.
2. Domaine $\cos x\ne0$; $(1-\tan^2x)/(1+\tan^2x)=\cos(2x)$.
3. Domaine $\sin x\ne0$. En posant c=cos x et en utilisant $\sin^2x=(1-c)(1+c)$, le premier quotient devient $ (1-3c)/(1-c)$, donc la différence vaut 0.
4. Domaine $]-1,1[$, $\tan(\arcsin x)=x/\sqrt{1-x^2}$.
5. Domaine [−1,1], $\sin(\arccos x)=\sqrt{1-x^2}$.
6. Pour tout x, $\cos(\arctan x)=1/\sqrt{1+x^2}$.
7. Domaine [−1,1], $\cos(2\arccos x)=2x^2-1$.
8. Domaine [−1,1], $\cos(2\arcsin x)=1-2x^2$.
9. Domaine [−1,1], $\sin(2\arccos x)=2x\sqrt{1-x^2}$.
10. Pour tout x, $\cos(2\arctan x)=(1-x^2)/(1+x^2)$.
11. Pour tout x, $\sin(2\arctan x)=2x/(1+x^2)$.
12. Domaine $x\in[-1,1]\setminus\{−1/\sqrt2,1/\sqrt2\}$; $\tan(2\arcsin x)=2x\sqrt{1-x^2}/(1-2x^2)$.


## Exercice 31

1. Pour tout x, $\arctan(x+1)-\arctan x\in(0,\pi/2)$, et sa tangente vaut $1/(x^2+x+1)$. Donc la différence vaut $\arctan(1/(x^2+x+1))$.
2. Avec x=k, cette différence est le k-ième terme. La somme télescope : $S_n=\arctan(n+1)-\arctan0=\arctan(n+1)$.
3. $S_n\to\pi/2$.

## Exercice 32

1. $x+1/x\ge2$ par AM-GM.
2. Pour 0<x<1, $(x+2)/(1-x)\ge2$ car l'inégalité équivaut à 3x≥0. Pour 1<x<4, $|(x+2)/(1-x)|=(x+2)/(x-1)\ge2\iff x\le4$.
3. $r(x)=(x+1)/(x^2+3)$ sur [0,2]. Sa dérivée est $-(x+3)(x-1)/(x^2+3)^2$, donc son maximum est r(1)=1/2, et son minimum est min(r(0),r(2))=1/3.
4. La même dérivée montre les extrema globaux en x=−3 et x=1; $r(-3)=-1/6$, $r(1)=1/2$.

## Exercice 33

1. $e^x\ge1+x$ par convexité, tangente en 0.
2. Pour x>0, x≠1, poser $t=(x-1)/(x+1)$. Ou étudier $F(x)=\ln x-2(x-1)/(x+1)$: $F'(x)=(x-1)^2/(x(x+1)^2)\ge0$, F(1)=0; le quotient $(x+1)/(x-1)\ln x\ge2$ suit par les signes de x−1 et ln x.
3. $x\ln x-(x-1)\le(x-1)^2\iff\ln x\le x-1$, après division par x>0.
4. Soit $H(x)=(x-2)e^x+x+2$. H(0)=H'(0)=0 et $H''(x)=xe^x\ge0$; donc H'≥0 puis H≥0 pour x≥0.
5. Pour n≥2, $\ln(1+1/n)\le1/n$, et $-\ln(1-1/n)\ge1/n$. Exponentier donne $(1+1/n)^n\le e\le(1-1/n)^{-n}$.

## Exercice 34

1. $|\sin x|=|\int_0^x\cos t\,dt|\le|x|$.
2. Pour t≥0, $(\arcsin t)'=1/\sqrt{1-t^2}\ge1$; intégrer de 0 à |x| et utiliser l'imparité.
3. $1-\cos x=2\sin^2(x/2)$, donc $0\le1-\cos x\le x^2/2$ par (i).
4. Pour x≥0, $(\tan x)'=1/\cos^2x\ge1$; intégrer depuis 0 puis utiliser l'imparité.

## Exercice 35

Posons $H(x)=\frac23\sin x+\frac13\tan x-x$. H(0)=H'(0)=0 et


```math
H''(x)=\frac23\left(\frac{\sin x}{\cos^3x}-\sin x\right)>0\quad(0<x<\pi/2),
```


car $0<\cos x<1$. Donc H(x)>0.

## Exercice 36+

Posons $G(x)=3\ln(\sin x/x)-\ln(\cos x)$ sur (0,π/2). Alors G(0+)=0 et


```math
G'=3\cot x-3/x+\tan x>0
```


car, après multiplication par $x\sin x\cos x>0$, cette inégalité équivaut à $H(x)=x(3-2\sin^2x)-3\sin x\cos x>0$. Or H(0)=0 et $H'=4\sin x(\sin x-x\cos x)>0$, puisque $\tan x>x$. Donc G>0 et $\cos x<(\sin x/x)^3$.

## Exercice 37

Soit $S(x)=\sum_{k=1}^{2p+1}(-1)^{k+1}x^k/k$. Pour x>−1,


```math
S'(x)-\frac1{1+x}=\frac{x^{2p+1}}{1+x}.
```


Comme S(0)=ln(1+0)=0, $S(x)-\ln(1+x)=\int_0^x t^{2p+1}/(1+t)\,dt\ge0$ aussi bien pour x≥0 que pour −1<x<0.

## Exercice 38+

Classons les 13 angles $\theta=\arctan a$, a∈A, dans ]−π/2,π/2[. Les 12 écarts consécutifs ont une somme strictement inférieure à π; l'un a donc longueur $0<\delta<\pi/12$. Pour les valeurs correspondantes a>b, $1+ab>0$ et


```math
\frac{a-b}{1+ab}=\tan(\arctan a-\arctan b)=\tan\delta<\tan(\pi/12)=2-\sqrt3.
```



## Exercice 39

1. $x\ln x=1$ impose x>1. La fonction x ln x y est strictement croissante, tend de 0 à +∞; il existe une unique solution.
2. Le membre droit $1/\operatorname{ch}x$ est positif, donc tout point fixe vérifie x>0. Sur $\mathbb R_+$, h(x)=1/ch x−x est continue strictement décroissante, h(0)=1 et h(1)<0; elle a un unique zéro.
3. Pour x≤0, le membre gauche $e^{-x^2}>0$ et le droit $e^x-1\le0$, donc aucune solution. Sur [0,+∞[, le premier membre décroît strictement de 1 à 0 tandis que le second croît strictement de 0 à +∞; il existe une unique solution.

## Exercice 40

Posons t=sin x+cos x∈[−√2,√2]. Comme $\sin^3x+\cos^3x=t(1-(t^2-1)/2)=t(3-t^2)/2$, l'équation vaut $(t-1)^2(t+2)=0$. Dans l'intervalle possible, t=1. Ainsi $\sin x+\cos x=1$, soit $x=2k\pi$ ou $x=\pi/2+2k\pi$.

## Exercice 41

1. $\cos(2x-\pi/3)=\cos(x+\pi/4)$, donc $x=7\pi/12+2k\pi$ ou $x=\pi/36+2k\pi/3$.
2. $\sin4x+\cos4x=1\iff4x\equiv0$ ou $\pi/2\pmod{2\pi}$. Donc $x=k\pi/2$ ou $x=\pi/8+k\pi/2$.
3. $\sin x+\sin3x=2\sin2x\cos x=0$, d'où $x=k\pi/2$.
4. $\sin x+\sin2x+\sin3x=\sin2x(1+2\cos x)$. Donc $x=k\pi/2$ ou $x=\pm2\pi/3+2k\pi$.
5. Aucune solution, car $3(\cos x-\sin x)\le3\sqrt2<6$.
6. $\sin2x+\sqrt3\cos2x=0\iff2x=-\pi/3+k\pi$, donc $x=-\pi/6+k\pi/2$.

## Exercice 42

Sur le domaine de définition, $\tan x\tan2x=1\iff\sin x\sin2x=\cos x\cos2x\iff\cos3x=0$. Ainsi $x=\pi/6+k\pi/3$, en excluant les x pour lesquels $\cos x=0$, soit k≡1 (mod 3). Les valeurs restantes vérifient aussi $\cos2x\ne0$.

## Exercice 43

1. Domaine |x|≤1/2; le membre gauche appartient à [−π/6,π/6], tandis que $\arccos x\ge\arccos(1/2)=\pi/3$. Aucune solution.
2. x∈[−1,0]. La fonction $F(x)=\arcsin(x+1)-\arcsin x$ atteint son minimum en x=−1/2 (sa dérivée s'annule seulement là); ce minimum vaut π/3. Il ne peut donc valoir π/6 : aucune solution.
3. La tangente de la somme donne $3x/(1-2x^2)=1$, soit $2x^2+3x-1=0$. Comme la somme vaut π/4, il faut x>0; seule solution $x=(-3+\sqrt{17})/4$.
4. $x=\sin(\arccos(1/3)-\arccos(1/4))=(2\sqrt2-\sqrt{15})/12$.
5. $2x/(1+x^2)=\sqrt3/2$, d'où $x=1/\sqrt3$ ou $x=\sqrt3$.
6. $\arctan2+\arctan3=3\pi/4\notin[-\pi/2,\pi/2]$; aucune solution.

## Autocorrection D

(i) $(\cos3x)^{(n)}=3^n\cos(3x+n\pi/2)$.

(ii) $(x^5e^{3x})^{(n)}=e^{3x}\sum_{k=0}^{\min(n,5)}\binom nk\frac{5!}{(5-k)!}x^{5-k}3^{n-k}$.

(iii) $(e^x\cos x)^{(n)}=2^{n/2}e^x\cos(x+n\pi/4)$.

(iv) Pour x>0, $(x^\alpha)^{(n)}=\alpha(\alpha-1)\cdots(\alpha-n+1)x^{\alpha-n}$.

(v) $(x^2\sin x)^{(n)}=x^2\sin(x+n\pi/2)+2nx\sin(x+(n-1)\pi/2)+n(n-1)\sin(x+(n-2)\pi/2)$.

(vi) $(\cos^3x)^{(n)}=\frac14[3\cos(x+n\pi/2)+3^n\cos(3x+n\pi/2)]$, car $\cos^3x=(3\cos x+\cos3x)/4$.

(vii) Pour x≠±1,


```math
\left(\frac1{x^2-1}\right)^{(n)}=\frac{(-1)^nn!}{2}\left(\frac1{(x-1)^{n+1}}-\frac1{(x+1)^{n+1}}\right).
```



(viii) Pour n=0, la fonction est $\ln(1+x)/x$, de domaine $]-1,0[\cup]0,+\infty[$. Pour n≥1 et x>−1,


```math
(x^{n-1}\ln(1+x))^{(n)}=\sum_{k=0}^{n-1}\binom nk\frac{(n-1)!}{(n-1-k)!}x^{n-1-k}\frac{(-1)^{n-k-1}(n-k-1)!}{(1+x)^{n-k}}.
```



## Exercice 44

Sur x≠0, utiliser le développement localement convergent $x^{n-1}e^{1/x}=\sum_{m=0}^\infty x^{n-1-m}/m!$. Après n dérivations, les termes m<n s'annulent et, pour m≥n, le coefficient dérivé vaut $(-1)^n/(m-n)!$. Ainsi


```math
f_n^{(n)}(x)=(-1)^n x^{-n-1}\sum_{j=0}^\infty\frac{x^{-j}}{j!}=\frac{(-1)^n e^{1/x}}{x^{n+1}}.
```



## Exercice 45+

1. Pour $f=\arctan$, $f'=\cos^2(f)$. Une récurrence par dérivation, avec les formules trigonométriques, donne


```math
f^{(n)}(x)=(n-1)!\cos^n(f(x))\sin\!\left(n\left(\frac\pi2+f(x)\right)\right),\qquad n\ge1.
```


La formule est vraie pour n=1; en la dérivant et en utilisant $f'=\cos^2 f$, on obtient celle d'indice n+1.
2. Pour n=0, f s'annule en x=0. Pour n≥1, cos(f(x))>0 et les zéros vérifient $n(\pi/2+f(x))=k\pi$, k=1,…,n−1. Ils sont


```math
x=\tan\left(\frac{k\pi}{n}-\frac\pi2\right),\quad k=1,\ldots,n-1;
```


pour n=1, il n'y en a aucun.

## Exercice 46+

Posons $P_0(t)=t$ et $P_{n+1}(t)=(1+t^2)P_n'(t)$. Comme $d/dx=(1+\tan^2x)d/dt$ pour t=tan x, $\tan^{(n)}x=P_n(\tan x)$. Chaque P_n a des coefficients non négatifs : c'est vrai pour P₀, et la récurrence le conserve (la dérivée d'un polynôme à coefficients positifs en t≥0 reste positive). Pour x∈[0,π/2[, tan x≥0; toutes les dérivées sont donc positives ou nulles. La formule récurrente établit aussi la lissité.

## Exercice 47+

Sur [0,1[, $g=\arcsin$ vérifie $g'=1/\sqrt{1-x^2}>0$ et $g''/g'=x/(1-x^2)$. La dérivée de ce quotient vaut


```math
f(x)=\left(\frac{g''}{g'}\right)'=\frac{1+x^2}{(1-x^2)^2}=\sum_{k=0}^\infty(2k+1)x^{2k}.
```


La série a des coefficients non négatifs; ses dérivées le sont sur [0,1[, donc f est absolument monotone. Le quotient $r=g''/g'=x/(1-x^2)$ l'est aussi, car r(0)=0 et r'=f≥0 avec toutes dérivées positives. Comme $(g')'=rg'$, une récurrence utilisant la formule de Leibniz montre que toutes les dérivées de g' sont positives. Enfin g≥0 sur [0,1[, donc arcsin est absolument monotone sur cet intervalle.

## Exercice 48

La dérivée n-ième de $x^{2n}$ vaut $(2n)!x^n/n!$. D'autre part, en dérivant $x^n x^n$ par Leibniz,


```math
(x^{2n})^{(n)}=n!x^n\sum_{k=0}^n\binom nk^2.
```


En identifiant, $\sum_{k=0}^n\binom nk^2=\binom{2n}{n}$.

## Exercice 49+

D'une part, en dérivant par rapport à α la formule $(x^\alpha)^{(n)}=\alpha(\alpha-1)\cdots(\alpha-n+1)x^{\alpha-n}$ en α=n, on obtient


```math
(x^n\ln x)^{(n)}=n!(\ln x+H_n),\qquad H_n=\sum_{k=1}^n\frac1k.
```


D'autre part, la formule de Leibniz, dérivant x^n k fois et ln x n−k fois, donne


```math
(x^n\ln x)^{(n)}=n!\ln x+n!\sum_{k=1}^n\frac{(-1)^{k-1}}k\binom nk.
```


Égaler ces expressions donne l'identité demandée.

## Autocorrection C

Dans le tableau, D est le domaine réel de l'expression et D′ un sous-ensemble ouvert de points où elle est dérivable. Les paramètres a,b sont strictement positifs.

| Expression | D | D′ et dérivée |
|---|---|---|
| (a) $e^{-a/x^2}$ | $\mathbb R^*$ | D; $2a x^{-3}e^{-a/x^2}$ |
| (b) $\cos(ax^2+bx+1)/\sin x$ | $\sin x\ne0$ | D; $-[(2ax+b)\sin(ax^2+bx+1)\sin x+\cos(ax^2+bx+1)\cos x]/\sin^2x$ |
| (c) $(1+a/x)^x$ | $]-\infty,-a[\cup]0,+\infty[$ | D; $f[\ln(1+a/x)-a/(x+a)]$ |
| (d) $\sqrt{1+\cos^2x}$ | $\mathbb R$ | D; $-\sin x\cos x/\sqrt{1+\cos^2x}$ |
| (e) $(ax+b)^x$ | $x>-b/a$ | D; $f[\ln(ax+b)+ax/(ax+b)]$ |
| (f) $x-a\sqrt x$ | $[0,+\infty[$ | $]0,+\infty[$; $1-a/(2\sqrt x)$ |
| (g) $\arctan(e^x)$ | $\mathbb R$ | D; $e^x/(1+e^{2x})$ |
| (h) $\arcsin(x^2-1)$ | $[-\sqrt2,\sqrt2]$ | $]-\sqrt2,0[\cup]0,\sqrt2[$; $2x/\sqrt{1-(x^2-1)^2}$ |
| (i) $\arccos(1/(1+x))$ | $]-\infty,-2]\cup[0,+\infty[$ | $]-\infty,-2[\cup]0,+\infty[$; $1/((1+x)^2\sqrt{1-(1+x)^{-2}})$ |
| (j) $\arctan\sqrt{(1-\sin x)/(1+\sin x)}$ | $\sin x\ne-1$ | D privé des $x$ tels que $\sin x=1$; $-\operatorname{sgn}(\cos x)/2$ |
| (k) $\cos^3x/(1-\cos x)^2$ | $x\ne2k\pi$ | D; $-\sin x\cos^2x(3-\cos x)/(1-\cos x)^3$ |
| (l) $\sin(\ln x+1/x)$ | $]0,+\infty[$ | D; $(1/x-1/x^2)\cos(\ln x+1/x)$ |
| (m) $(x+1)/\sin(2x)$ | $\sin(2x)\ne0$ | D; $[\sin(2x)-2(x+1)\cos(2x)]/\sin^2(2x)$ |
| (n) $\sin((2x+5)^2)$ | $\mathbb R$ | D; $4(2x+5)\cos((2x+5)^2)$ |
| (o) $\arccos((1+x)/(1-x))$ | $]-\infty,0]$ | $]-\infty,0[$; $-2/((1-x)^2\sqrt{1-((1+x)/(1-x))^2})$ |
| (p) $\sqrt{\arcsin x-\pi/6}$ | $[1/2,1]$ | $]1/2,1[$; $1/(2\sqrt{\arcsin x-\pi/6}\sqrt{1-x^2})$ |
| (q) $\arcsin(\tan x)$ | $x\in\bigcup_k[-\pi/4+k\pi,\pi/4+k\pi]$ | Intérieurs de ces intervalles; $\sec^2x/\sqrt{1-\tan^2x}$ |
| (r) $\operatorname{sh}x\sin x$ | $\mathbb R$ | D; $\operatorname{ch}x\sin x+\operatorname{sh}x\cos x$ |
| (s) $\sqrt{x+\sqrt x}$ | $[0,+\infty[$ | $]0,+\infty[$; $(1+1/(2\sqrt x))/(2\sqrt{x+\sqrt x})$ |
| (t) $\ln(1+\operatorname{ch}x)$ | $\mathbb R$ | D; $\operatorname{sh}x/(1+\operatorname{ch}x)$ |
| (u) $x^x$ | $]0,+\infty[$ | D; $x^x(\ln x+1)$ |
| (v) $\cos x\ln(1+x)$ | $]-1,+\infty[$ | D; $-\sin x\ln(1+x)+\cos x/(1+x)$ |
| (w) $\ln(\tan(x/2))$ | $\bigcup_k]2k\pi,(2k+1)\pi[$ | D; $1/\sin x$ |
| (x) $\arctan(\operatorname{ch}x)$ | $\mathbb R$ | D; $\operatorname{sh}x/(1+\operatorname{ch}^2x)$ |
| (y) $1/\operatorname{sh}(\arcsin x)$ | $[-1,1]\setminus\{0\}$ | $]-1,0[\cup]0,1[$; $-\frac{\operatorname{ch}(\arcsin x)}{\operatorname{sh}^2(\arcsin x)\sqrt{1-x^2}}$ |
| (z) $\sin x/(\cos x+2)^4$ | $\mathbb R$ | D; $[\cos x(\cos x+2)+4\sin^2x]/(\cos x+2)^5$ |

| Expression | D | D′ et dérivée |
|---|---|---|
| (α) $\ln(\arctan x)$ | $]0,+\infty[$ | D; $1/((1+x^2)\arctan x)$ |
| (β) $(\operatorname{ch}x)^x$ | $\mathbb R$ | D; $(\operatorname{ch}x)^x[\ln(\operatorname{ch}x)+x\operatorname{th}x]$ |
| (γ) $x^3\cos(5x+1)$ | $\mathbb R$ | D; $3x^2\cos(5x+1)-5x^3\sin(5x+1)$ |
| (δ) $1/\sin(x^2)$ | $\sin(x^2)\ne0$ | D; $-2x\cos(x^2)/\sin^2(x^2)$ |
| (ε) $\ln(e^x+1)$ | $\mathbb R$ | D; $e^x/(e^x+1)$ |
| (ζ) $e^{x^3+2x^2+3x+4}$ | $\mathbb R$ | D; $(3x^2+4x+3)e^{x^3+2x^2+3x+4}$ |
| (η) $e^{\sqrt{x^2+x+1}}$ | $\mathbb R$ | D; $(2x+1)e^{\sqrt{x^2+x+1}}/(2\sqrt{x^2+x+1})$ |
| (θ) $(e^{1/x}+1)/(e^{1/x}-1)$ | $\mathbb R^*$ | D; $2e^{1/x}/(x^2(e^{1/x}-1)^2)$ |
| (ι) $\cos(2x)/(x^2-2)$ | $x\ne\pm\sqrt2$ | D; $[-2(x^2-2)\sin(2x)-2x\cos(2x)]/(x^2-2)^2$ |
| (κ) $\ln(\cos(2x))$ | $\cos(2x)>0$ | D; $-2\tan(2x)$ |
| (λ) $|x|\sqrt{x^2-2x+1}/(x-1)$ | $\mathbb R\setminus\{1\}$ | $\mathbb R\setminus\{0,1\}$; dérivée 1 si x<0 ou x>1, −1 si 0<x<1 |
| (μ) $\ln(x-\sqrt{x^2-1})$ | $[1,+\infty[$ | $]1,+\infty[$; $-1/\sqrt{x^2-1}$ |
| (ν) $\ln\sqrt{(x+1)/(x-1)}$ | $]-\infty,-1[\cup]1,+\infty[$ | D; $-1/(x^2-1)$ |
| (ξ) $\ln(\ln x)$ | $]1,+\infty[$ | D; $1/(x\ln x)$ |
| (ο) $\ln(\ln(\ln x))$ | $]e,+\infty[$ | D; $1/(x\ln x\ln(\ln x))$ |
| (π) $\sin x\sin(1/x)$ | $\mathbb R^*$ | D; $\cos x\sin(1/x)-\sin x\cos(1/x)/x^2$ |
| (ρ) $\sqrt{1+x^2\sin^2x}$ | $\mathbb R$ | D; $(x\sin^2x+x^2\sin x\cos x)/\sqrt{1+x^2\sin^2x}$ |
| (σ) $\ln((1+\sin x)/(1-\sin x))$ | $\cos x\ne0$ | D; $2/\cos x$ |
| (τ) $e^{\cos x}/x$ | $\mathbb R^*$ | D; $-e^{\cos x}(x\sin x+1)/x^2$ |
| (υ) $x/(x^2+1)$ | $\mathbb R$ | D; $(1-x^2)/(x^2+1)^2$ |
| (φ) $\arcsin(1/\operatorname{ch}x)$ | $\mathbb R$ | $\mathbb R^*$; $-\operatorname{sgn}(x)/\operatorname{ch}x$ |
| (χ) $x/\sin x$ | $\sin x\ne0$ | D; $(\sin x-x\cos x)/\sin^2x$ |
| (ψ) $\ln(\arcsin(x^2))$ | $[-1,0[\cup]0,1]$ | $]-1,0[\cup]0,1[$; $2x/[\arcsin(x^2)\sqrt{1-x^4}]$ |
| (ω) $\ln(e^x+\sin x)$ | $\{x:e^x+\sin x>0\}$ | D; $(e^x+\cos x)/(e^x+\sin x)$ |
