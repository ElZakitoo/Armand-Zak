# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td27-equations-differentielles.pdf)

## Autocorrection A

Les constantes sont réelles.

(i) $(e^{x/4}y)'=0$, donc $y=Ce^{-x/4}$.

(ii) $(e^{x^2}y)'=e^x$, donc $y=e^{-x^2}(C+e^x)$.

(iii) Poser $y=z\ln x$. L'équation devient $xz'(\ln x)^2=3x^2(\ln x)^2$, donc $z'=3x$ et


```math
y=(C+\tfrac32x^2)\ln x.
```



(iv) $(y+1)'=-x^2(y+1)$, donc $y=-1+Ce^{-x^3/3}$.

(v) $(y\cos x)'=\cos^3x+1/\cos x$, donc


```math
y=\frac{C+\sin x-\frac13\sin^3x+\ln(\sec x+\tan x)}{\cos x}.
```


Sur l'intervalle considéré, $\cos x>0$ et $\sec x+\tan x>0$.

(vi) Pour $t=\arcsin x$, $z(t)=y(\sin t)$ vérifie $z'-z=1$ :


```math
y=Ce^{\arcsin x}-1.
```



(vii) $(y/\cosh x)'=1+1/\cosh^2x$, donc


```math
y=(C+x)\cosh x+\sinh x.
```



(viii) $(y/x^2)'=\sin x$, donc $y=x^2(C-\cos x)$.

(ix) Pour $t=\ln(1+x)$, $z(t)=y(e^t-1)$ vérifie $z''=2$, donc


```math
y=\ln^2(1+x)+C\ln(1+x)+D.
```



## 1

1. En posant $y=e^{\tau x}g$, l'équation devient $g'+(a+\tau)g=f$. Si $a+\tau\ne0$,


```math
g=\sum_{j=0}^n\frac{(-1)^jf^{(j)}}{(a+\tau)^{j+1}}
```


convient par télescopage, et son degré est $n$. Si $a+\tau=0$, prendre une primitive polynomiale de $f$, de degré $n+1$.

2. (i) La résolution de $g'+3g=x^2-2x+2$ donne


```math
y=Ce^{-x}+e^{2x}\left(\frac{x^2}3-\frac{8x}9+\frac{26}{27}\right).
```


(ii) Écrire le second membre $(\frac12-x)e^x+(-\frac12-x)e^{-x}$ :


```math
y=Ce^{2x}+(x+\tfrac12)e^x+(\tfrac x3+\tfrac5{18})e^{-x}.
```


(iii) Les deux seconds membres sont $x^2e^x$ et $xe^{3x}$ :


```math
y=e^{3x}(C+\tfrac{x^2}2)-e^x(\tfrac{x^2}2+\tfrac x2+\tfrac14).
```



## Autocorrection B

Avec $D=d/dx$, les factorisations et solutions générales sont :

(i) $4D^2+9$ :


```math
y=A\cos(3x/2)+B\sin(3x/2).
```


(ii) $(D+1)^2$ : $y=(A+Bx)e^{-x}$.

(iii) $(D+2)^2$, avec $y=e^{-2x}z$ pour le premier terme forcé :


```math
y=e^{-2x}(A+Bx+x^2/2)+\frac14.
```


(iv) $(D^2-1)(x\sinh x)=2\cosh x$ :


```math
y=Ae^x+Be^{-x}+\frac x2\sinh x.
```


(v) $\sinh x=(e^x-e^{-x})/2$ :


```math
y=e^{-x}(A+Bx-x^2/4)+e^x/8.
```


(vi) Les racines homogènes sont $r_\pm=(3\pm\sqrt5)/2$ :


```math
y=Ae^{r_+x}+Be^{r_-x}+\frac{\cos x-\sin x}{3}.
```


(vii) Avec $y=e^{2x}z$, le second membre impose $z''+z'=\sin3x$ :


```math
y=Ae^x+Be^{2x}-\frac{e^{2x}}{30}(3\sin3x+\cos3x).
```


(viii) Avec $y=e^xz$, $z''+4z=4\cos2x$ :


```math
y=e^x(A\cos2x+B\sin2x+x\sin2x).
```


(ix) $(D-1)(D-3)(xe^{3x})=2e^{3x}$ :


```math
y=Ae^x+(B+\tfrac32x)e^{3x}.
```


(x) Les racines sont $1,-2$; la substitution d'un sinus et d'un cosinus donne


```math
y=Ae^x+Be^{-2x}+\frac{-3\cos x+\sin x}{10}.
```


(xi) $\cos^3x=(3\cos x+\cos3x)/4$ :


```math
y=A\cos x+B\sin x+\frac38x\sin x-\frac1{32}\cos3x.
```



## 2

L'opérateur est $(D-1)(D-\alpha)$.

Pour $\alpha\notin\{0,1\}$,


```math
y=Ae^x+Be^{\alpha x}+\frac{e^{(1+\alpha)x}}{\alpha}.
```


Pour $\alpha=1$,


```math
y=(A+Bx)e^x+e^{2x}.
```


Pour $\alpha=0$, le second membre est résonant :


```math
y=A+Be^x+xe^x.
```



## 3

1. $P(x)=3x^2-6$ vérifie $P''+P=3x^2$.
2. $y=A\cos x+B\sin x+3x^2-6$. Les conditions initiales donnent $A=7$, $B=2$ :


```math
y=7\cos x+2\sin x+3x^2-6.
```



## 4

Pour $\omega>0$, poser $h=A\cos(\omega x)+B\sin(\omega x)$.
Si $\theta\ne\omega$, les solutions respectives sont


```math
y=h+\frac{\cos(\theta x)}{\omega^2-\theta^2},\qquad y=h+\frac{\sin(\theta x)}{\omega^2-\theta^2}.
```


Si $\theta=\omega>0$, elles sont


```math
y=h+\frac{x\sin(\omega x)}{2\omega},\qquad y=h-\frac{x\cos(\omega x)}{2\omega}.
```


Pour $\omega=0<\theta$, intégrer deux fois :


```math
y=A+Bx-\frac{\cos(\theta x)}{\theta^2},\qquad y=A+Bx-\frac{\sin(\theta x)}{\theta^2}.
```


Pour $\omega=\theta=0$, elles sont respectivement $y=A+Bx+x^2/2$ et $y=A+Bx$.

## 5

1. a) Écrire $\Phi=(u,v)^{\mathsf T}$ donne $u'=v$, $v'=-u$, donc $u''+u=0$ et


```math
\Phi(x)=R(x)\Lambda,\qquad R(x)=\begin{pmatrix}\cos x&\sin x\\-\sin x&\cos x\end{pmatrix}.
```


b) Comme $R^{-1}=R(-x)$,


```math
\Lambda(x)=R(-x)\binom{f(x)}{f'(x)},\qquad\lambda=f\cos x-f'\sin x,\qquad\mu=f\sin x+f'\cos x.
```


Ces fonctions sont dérivables. En dérivant $f=\lambda\cos x+\mu\sin x$ et en utilisant la seconde égalité,


```math
\lambda'\cos x+\mu'\sin x=0.
```


c) La seconde équation est $-\lambda'\sin x+\mu'\cos x=1/\cos x$, donc $\lambda'=-\tan x$, $\mu'=1$. Prendre $\lambda=\ln\cos x$, $\mu=x$ :


```math
y=A\cos x+B\sin x+\cos x\ln(\cos x)+x\sin x.
```



2. (i) Poser $y=e^{-x}z$. Alors $z''+z'=(x-1)/x^2$, et $z=\ln x$ convient :


```math
y=Ae^{-x}+Be^{-2x}+e^{-x}\ln x.
```


(ii) Poser $y=e^xz$. Alors $z''=\ln x/x$, d'où


```math
y=e^x\left(A+Bx+\frac x2(\ln^2x-2\ln x+2)\right).
```


(iii) $(D-2)^2(2xe^x)=2(x-2)e^x$, donc


```math
y=(A+Bx)e^{2x}+2xe^x.
```


(iv) Pour $y=\lambda\cos2x+\mu\sin2x$, la variation des constantes donne


```math
\lambda'=-\tfrac12\sin2x\cot x=-\cos^2x,\qquad\mu'=\tfrac12\cos2x\cot x.
```


Prendre $\lambda=-x/2-\sin2x/4$ et $\mu=\frac12\ln\sin x-\frac12\sin^2x$. En absorbant le terme $-\sin2x/4$ dans la solution homogène,


```math
y=A\cos2x+B\sin2x-\frac x2\cos2x+\frac12\sin2x\ln(\sin x).
```



## 6

1. Pour $g=\lambda f$,


```math
(1+x^2)g''-2g=(1+x^2)(f\lambda''+2f'\lambda').
```


Puisque $f$ ne s'annule pas, $g$ est solution exactement lorsque $\lambda''+2(f'/f)\lambda'=0$.
2. Prendre $f=1+x^2$. Alors $\lambda'=C/(1+x^2)^2$, et


```math
\int\frac{dx}{(1+x^2)^2}=\frac{x}{2(1+x^2)}+\frac12\arctan x.
```


Ainsi


```math
y=A(1+x^2)+B\bigl(x+(1+x^2)\arctan x\bigr).
```



## 7

(i) $((1+x^2)y')'=0$, donc $y=A+B\arctan x$.

(ii) Pour $z=y'+y$, l'équation devient $(1+e^x)z'-e^xz=0$, donc $z=C(1+e^x)$. Résoudre ensuite $y'+y=z$ donne


```math
y=A(2+e^x)+Be^{-x}.
```



(iii) Pour $z=e^{x^2}y$, l'équation devient $z''+z=0$, donc


```math
y=e^{-x^2}(A\cos x+B\sin x).
```



(iv) Pour $z=y/(1+e^x)$, le membre gauche devient $(1+e^x)^3(z''-z)$, donc


```math
y=(1+e^x)(Ae^x+Be^{-x}).
```



(v) Pour $z=y'-y$, $xz'-z=1$. Sur chaque demi-droite, $z=Cx-1$; la dérivabilité de $z$ en $0$ impose la même constante des deux côtés. En résolvant $y'-y=Cx-1$,


```math
y=1+Ae^x+B(x+1).
```



(vi) Pour $z=xy$, $z''+2z'+z=0$, donc $z=(A+Bx)e^{-x}$. Comme $z(0)=0$, $A=0$, et par continuité,


```math
y=Be^{-x}.
```



(vii) Pour $z=(1+e^x)y$, $z''+z=xe^x$. Une solution particulière est $z_p=(x-1)e^x/2$ :


```math
y=\frac{A\cos x+B\sin x+(x-1)e^x/2}{1+e^x}.
```



## 8

Une solution ne s'annule pas sur $\mathbb R_+^*$, car l'équation donnerait $x^2=0$. Poser $v=y^2$ :


```math
xv'-v=x^2,\qquad(v/x)'=1,\qquad v=x^2+Cx.
```


La positivité pour tout $x>0$ impose $C\geq0$. Le signe de $y$ est constant, donc les solutions sont exactement


```math
y(x)=\pm\sqrt{x^2+Cx},\qquad C\geq0.
```



## 9

(i) Pour $z(t)=y(e^t)$, $z'=xy'$, $z''=x^2y''+xy'$. Ainsi


```math
z''+2z'+z=e^{2t}+2e^t+1.
```


Les solutions sont


```math
y(x)=\frac{A+B\ln x}{x}+\frac{x^2}{9}+\frac x2+1.
```



(ii) Pour $z(t)=y(\tan t)$,


```math
z''=(1+x^2)^2y''+2x(1+x^2)y'.
```


Donc $z''+4z=0$ et


```math
y=A\cos(2\arctan x)+B\sin(2\arctan x)=\frac{A(1-x^2)+2Bx}{1+x^2}.
```



(iii) Pour $z(t)=y(\sin t)$, $z''=(1-x^2)y''-xy'$. Ainsi $z''+z=0$, d'où


```math
y=A\sqrt{1-x^2}+Bx.
```



## 10

1. Pour $x\ne0$, $(y/x^2)'=1/x^2$, donc $y=-x+Cx^2$ sur chaque demi-droite.
2. L'équation en $0$ impose $y(0)=0$. Pour tous $C_-,C_+\in\mathbb R$,


```math
y(x)=\begin{cases}-x+C_-x^2&x<0,\\0&x=0,\\-x+C_+x^2&x>0\end{cases}
```


est dérivable, avec $y'(0)=-1$, et satisfait l'équation. Ce sont toutes les solutions.
3. La donnée $y(0)=0$ possède une infinité de solutions; une donnée $y(0)\ne0$ n'en possède aucune. L'existence et l'unicité du problème de Cauchy ne valent donc pas sans l'hypothèse de résolution.

## 11

(i) Sur $\mathbb R^*$, $(y/x)'=1$, donc $y=x^2+C_\pm x$. La dérivabilité en $0$ impose $C_-=C_+$ :


```math
y=x^2+Cx.
```



(ii) $(xy)'=x^2$, donc $y=x^2/3+C_\pm/x$ hors de $0$. La continuité en $0$ impose les constantes nulles : $y=x^2/3$.

(iii) Une solution particulière est $-\cosh x$; les solutions hors de $0$ sont $y=C_\pm\sinh x-\cosh x$. La dérivabilité en $0$ identifie les constantes :


```math
y=C\sinh x-\cosh x.
```



(iv) Pour $z=y-1$, $(xe^xz)'=0$. Les expressions $z=C_\pm e^{-x}/x$ ne se prolongent continûment en $0$ que pour $C_\pm=0$. Donc $y=1$.

(v) Pour $x\ne0$, $(e^{|x|}y)'=x$, d'où $y=e^{-|x|}(x^2/2+C_\pm)$. La continuité impose $C_-=C_+=C$; les dérivées à gauche et à droite en $0$ valent $C$ et $-C$. Donc


```math
y=\frac{x^2}{2}e^{-|x|}.
```



(vi) Sur les trois intervalles séparés par $\pm1$, les solutions sont des multiples de $\sqrt{|x^2-1|}$. L'équation impose $y(\pm1)=0$. Tout multiple non nul a un quotient de différence non borné au point adjacent $\pm1$. La dérivabilité impose donc $y=0$ sur les trois intervalles, puis partout.

(vii) Aucune solution dérivable sur $\mathbb R$. En effet, l'équation en $-1$ donne $y(-1)=-\pi/4$. Si $L=y'(-1)$, pour $t\to0$,


```math
y(-1+t)=-\pi/4+Lt+o(t),\qquad\arctan(-1+t)=-\pi/4+t/2+o(t).
```


L'équation hors de $-1$ donne alors


```math
y'(-1+t)=\frac{\arctan(-1+t)-y(-1+t)}{(-1+t)t}\longrightarrow L-\frac12.
```


Le théorème des accroissements finis impose que cette limite soit $y'(-1)=L$, contradiction.

(viii) Sur chaque intervalle entre deux multiples consécutifs de $\pi$, $y=C_k\sin x-\cos x$. La dérivabilité aux multiples de $\pi$ impose $C_{k-1}=C_k$ pour tout $k$. Ainsi


```math
y=C\sin x-\cos x.
```



## 12

Pour $x>0$,


```math
\left|\frac1x\int_0^xf(t)\,dt-f(0)\right|\leq\sup_{0\leq t\leq x}|f(t)-f(0)|\longrightarrow0.
```


L'équation $(xy)'=f$ donne $y(x)=(C+\int_0^xf(t)\,dt)/x$. Une limite finie en $0$ impose $C=0$. L'unique solution prolongeable est donc


```math
y(x)=\frac1x\int_0^xf(t)\,dt,\qquad y(0)=f(0).
```



## 13

Si $y'=1+y^2$ sur $\mathbb R$, alors $(\arctan y)'=1$, donc $\arctan y(x)=x+C$, impossible car le membre gauche est borné. Il n'existe aucune solution sur $\mathbb R$.

## 14

L'ensemble est le noyau de l'application linéaire $f\mapsto f'-f$. Sur chacune des quatre composantes


```math
I_1=]-\infty,-1[,\quad I_2=]-1,0[,\quad I_3=]0,1[,\quad I_4=]1,+\infty[,
```


les solutions sont des multiples de $e^x$. Les quatre fonctions $x\mapsto e^x\mathbf1_{I_j}(x)$ forment une base; la dimension vaut $4$.

## 15

Poser $c=\int_0^1f$. L'équation $f'+f=c$ donne $f(x)=c+Ae^{-x}$. En intégrant sur $[0,1]$,


```math
c=c+A(1-e^{-1})\quad\Longrightarrow\quad A=0.
```


Les solutions sont exactement les fonctions constantes.

## 16

1. La fonction nulle et les fonctions $x\mapsto e^{\lambda x}$, $\lambda\in\mathbb C$, conviennent.
2. $f(0)=f(0)^2$, donc $f(0)\in\{0,1\}$.
3. $f(t)=f(0)f(t)$ impose $f=0$ si $f(0)=0$.
4. Dériver en $s$ donne $f'(s+t)=f'(s)f(t)$.
5. Avec $s=0$ et $\lambda=f'(0)$, $f'=\lambda f$. Si $f(0)=1$, la solution est $f(x)=e^{\lambda x}$.
6. 

```math
E=\{0\}\cup\{x\mapsto e^{\lambda x}:\lambda\in\mathbb C\}.
```



## 17

$f(0)=0$. Dériver l'identité en $s$ puis prendre $s=0$ donne $f'(t)=f'(0)$. Ainsi $f(x)=ax$, $a\in\mathbb R$, et ces fonctions conviennent.

## 18

Pour $s,t>0$, poser $g(u)=f(e^u)$. Alors $g$ est dérivable et $g(u+v)=g(u)g(v)$. D'après 16, dans le cas réel, $g=0$ ou $g(u)=e^{au}$ avec $a\in\mathbb R$. Les solutions sont donc


```math
f=0\quad\text{ou}\quad f(x)=x^a\ (a\in\mathbb R).
```



## 19

Pour $g(x)=e^{-x}f(x)$, l'identité devient $g(s+t)=g(s)+g(t)$. D'après 17, $g(x)=ax$, donc


```math
f(x)=axe^x,\qquad a\in\mathbb R.
```



## 20

Le second membre rend $f$ de classe $C^1$, avec $f'(x)=-f(\pi-x)$, puis de classe $C^2$, avec $f''=-f$. Écrire $f=A\cos x+B\sin x$ dans l'identité portant sur $f'$ donne $A=B$.

En $x=\pi$, l'équation initiale donne $f(\pi)=-1$, donc $A=B=1$. Réciproquement,


```math
\int_0^{\pi-x}(\cos t+\sin t)\,dt=\sin x+1+\cos x.
```


L'unique solution est $f(x)=\cos x+\sin x$.

## 21

L'équation rend $f$ de classe $C^2$. En dérivant puis en utilisant l'équation en $-x$,


```math
f''(x)-f'(-x)=e^x,\qquad f'(-x)+f(x)=e^{-x},
```


d'où $f''+f=2\cosh x$. Ainsi $f=A\cos x+B\sin x+\cosh x$. La substitution dans l'équation initiale impose $A+B=0$ :


```math
f(x)=A(\cos x-\sin x)+\cosh x.
```



## 22

Poser $a_0=a(x_0)$, $b_0=b(x_0)$ et $c=y(x_0)$. La tangente a pour équation


```math
Y=c+(a_0c+b_0)(X-x_0)=c\bigl(1+a_0(X-x_0)\bigr)+b_0(X-x_0).
```


Si $a_0=0$, toutes les tangentes ont la pente $b_0$. Si $a_0\ne0$, elles passent toutes par


```math
\left(x_0-\frac1{a_0},-\frac{b_0}{a_0}\right).
```



## 23

Poser $A(x)=\int_0^xa(t)\,dt$ et $h=(z-y)e^{-A}$. Alors


```math
h'=e^{-A}\bigl(z'-y'-a(z-y)\bigr)\leq0,\qquad h(0)=0.
```


Pour $x\geq0$, $h(x)\leq0$; comme $e^{-A(x)}>0$, $z(x)\leq y(x)$.

## 24

L'opérateur se factorise en $(D+1)(D-iu)$. Ses solutions homogènes $Ae^{-x}+Be^{iux}$ sont bornées sur $\mathbb R_+$.

Si $\alpha\ne u$, une solution particulière est


```math
y_p(x)=\frac{e^{i\alpha x}}{(1+i\alpha)i(\alpha-u)},
```


également bornée. Si $\alpha=u$, les solutions sont


```math
y=Ae^{-x}+Be^{iux}+\frac{x}{1+iu}e^{iux},
```


toutes non bornées à cause du dernier terme. La condition cherchée est $\alpha\ne u$.

## 25

Le dernier $g'$ de la définition imprimée doit être $g$. Avec $w=(f-f')g'$, les fonctions $f=e^x$, $g=e^{-x}$, solutions de $y''-y=0$, sont libres mais donnent $w=0$ : l'équivalence demandée est fausse.

Pour le wronskien $W=fg'-f'g$ :

1. 

```math
W'=fg''-f''g=f(-ag'-bg)-(-af'-bf)g=-aW.
```


Donc, pour tout $x_0$,


```math
W(x)=W(x_0)\exp\!\left(-\int_{x_0}^xa(t)\,dt\right).
```


2. Cette formule donne (i) $\Leftrightarrow$ (ii). Si $f,g$ sont liées, $W=0$. Réciproquement, si $W(x_0)=0$, les deux vecteurs $(f(x_0),f'(x_0))$ et $(g(x_0),g'(x_0))$ sont liés. Il existe donc $(\lambda,\mu)\ne(0,0)$ tel que $h=\lambda f+\mu g$ vérifie $h(x_0)=h'(x_0)=0$. L'unicité de Cauchy donne $h=0$, donc $f,g$ sont liées. Ainsi (ii) $\Leftrightarrow$ (iii).

## 26

Les modes associés aux racines $r$ de $r^2+ar+b$ sont $e^{rx}$, avec aussi $xe^{rx}$ si la racine est double.

Sur $\mathbb R_+$, toutes les solutions sont bornées exactement si toutes les racines ont une partie réelle négative ou nulle, les racines de partie réelle nulle étant simples. Pour une équation quadratique réelle, cela donne


```math
a\geq0,\qquad b\geq0,\qquad(a,b)\ne(0,0).
```


En effet, pour $a,b>0$, les parties réelles sont strictement négatives. Pour $a>0,b=0$, les racines sont $0,-a$; pour $a=0,b>0$, elles sont $\pm i\sqrt b$. Si $a<0$, la somme des parties réelles est positive; si $b<0$, une racine réelle est positive. Enfin $(a,b)=(0,0)$ admet la solution $x$.

Sur $\mathbb R$, toute racine doit être imaginaire pure et simple; la condition est


```math
a=0,\qquad b>0.
```



## 27

Les solutions sont $f=e^x(x^2+Ax+B)$, donc


```math
f'=e^x\bigl(x^2+(A+2)x+A+B\bigr).
```


1. 

```math
f'\geq0\iff(A+2)^2-4(A+B)\leq0\iff B\geq A^2/4+1.
```


Alors $x^2+Ax+B=(x+A/2)^2+B-A^2/4\geq1$, donc $f>0$.
2. Pour $f=x^2e^x$, $f\geq0$ mais $f'=x(x+2)e^x<0$ sur $]-2,0[$. La réciproque est fausse.

## 28

1. Poser $V(x)=\int_0^xv(t)\,dt$ et $w(x)=C+\int_0^xu(t)v(t)\,dt$. Alors $u\leq w$ et, puisque $v\geq0$,


```math
w'=uv\leq wv,\qquad(we^{-V})'\leq0.
```


Ainsi $w(x)e^{-V(x)}\leq w(0)=C$, d'où


```math
u(x)\leq Ce^{V(x)}.
```


2. Les équations intégrales et le caractère $k$-lipschitzien donnent


```math
|f(x)-g(x)|\leq|f(0)-g(0)|+k\int_0^x|f(t)-g(t)|\,dt.
```


Appliquer 1 à $u=|f-g|$, $v=k$ et $C=|f(0)-g(0)|$ :


```math
|f(x)-g(x)|\leq e^{kx}|f(0)-g(0)|.
```



## 29

1. La fonction $g$ est bornée. Les solutions de $y'-y=g$ sont


```math
y(x)=e^x\left(C+\int_0^xe^{-t}g(t)\,dt\right).
```


La bornitude en $+\infty$ impose $C=-\int_0^{+\infty}e^{-t}g(t)\,dt$. La fonction obtenue s'écrit


```math
f(x)=-e^x\int_x^{+\infty}e^{-t}g(t)\,dt=-\int_0^{+\infty}e^{-s}g(x+s)\,ds.
```


Elle est solution par dérivation de la première expression, et $|f(x)|\leq\|g\|_\infty$ sur $\mathbb R$. Deux solutions diffèrent de $Ce^x$, qui n'est bornée sur $\mathbb R$ que pour $C=0$.
2. La dernière expression donne $f(x+2\pi)=f(x)$. Plus généralement, toute période de $g$ est une période de $f$; réciproquement, $g=f'-f$ a toute période de $f$.

## 30

Poser $r=f'+f$, avec $r(x)\to0$. Alors


```math
f(x)=e^{-x}f(0)+\int_0^xe^{t-x}r(t)\,dt.
```


Pour $\varepsilon>0$, choisir $A$ tel que $|r(t)|\leq\varepsilon$ pour $t\geq A$. Pour $x\geq A$,


```math
|f(x)|\leq e^{-x}\left(|f(0)|+\int_0^Ae^t|r(t)|\,dt\right)+\varepsilon\int_A^xe^{t-x}\,dt.
```


Le premier terme tend vers $0$, le second est au plus $\varepsilon$. Donc $f(x)\to0$.

## 31

Deux intégrations par parties donnent


```math
\int_0^\pi\bigl(f''(x+t)+f(x+t)\bigr)\sin t\,dt=f(x)+f(x+\pi).
```


L'intégrande est positif ou nul, donc $f(x)+f(x+\pi)\geq0$.
