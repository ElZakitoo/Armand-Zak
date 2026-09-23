# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td26-integration.pdf)

## Autocorrection A

Sur chaque intervalle de définition, $C\in\mathbb R$.

(i) $-\frac14e^{-2x^2}+C$.

(ii) $\frac12(\ln x)^2+C$.

(iii) $-\arctan(\cos x)+C$.

(iv) $\sin(\ln x)+C$.

(v) $\frac1{2\cos^2x}+C$.

(vi) $-\frac13(1-x^2)^{3/2}+C$.

(vii) $\frac16\sin^6x+C$.

(viii) $-\cos x+\frac23\cos^3x-\frac15\cos^5x+C$.

(ix) $\tan x-x+C$.

(x) $-\frac1{3(\ln x)^3}+C$.

(xi) $\ln|\sin x|+C$.

(xii) $\frac13\ln|1+x^3|+C$.

(xiii) $-\ln(1+\cos^2x)+C$.

(xiv) $2\sqrt{\tan x}+C$.

(xv) $2\ln(1+\sqrt x)+C$.

(xvi) $\ln x\ln(\ln x)-\ln x+C$.

(xvii) $e^{e^x}+C$.

(xviii) $\arctan(\ln x)+C$.

(xix) $2\sqrt{1+\ln x}+C$.

(xx) $-\frac15e^{-x}(\sin2x+2\cos2x)+C$.

(xxi) $\frac12(\cosh x\sin x-\sinh x\cos x)+C$.

## Autocorrection B

À une constante additive près :

(i) $\frac13\ln\left|\frac{x-5}{x-2}\right|$.

(ii) $2\ln|x-5|-\ln|x-2|$.

(iii) $x+\frac{31}3\ln|x-5|-\frac73\ln|x-2|$.

(iv) $\frac2{\sqrt3}\arctan\frac{2x-1}{\sqrt3}$.

(v) $4\arctan x+\frac12\ln(1+x^2)$.

(vi) $\frac2{\sqrt7}\arctan\frac{4x+1}{\sqrt7}$.

(vii) $-\frac1{x-3}$.

(viii) $x-2\ln|x+2|-\frac1{x+2}$.

(ix)


```math
\frac12\ln|x-1|-\frac1{18}\ln|x+1|-\frac49\ln|x-2|-\frac1{3(x-2)}.
```



(x) $\frac14\ln\left|\frac{1+x}{1-x}\right|+\frac12\arctan x$.

(xi) $-\frac{x^2}2+\frac14\ln\left|\frac{1+x^2}{1-x^2}\right|$.

(xii) $\frac12\arctan(x^2)$.

(xiii)


```math
\frac13\ln|x-1|-\frac16\ln(x^2+x+1)-\frac1{\sqrt3}\arctan\frac{2x+1}{\sqrt3}.
```



## 1

(i)


```math
\frac{t+1}{t(t-1)^3}=-\frac1t+\frac1{t-1}-\frac1{(t-1)^2}+\frac2{(t-1)^3},
```




```math
I=\left[\ln\frac{t-1}t+\frac1{t-1}-\frac1{(t-1)^2}\right]_2^3
=\ln\frac43+\frac14.
```



(ii)


```math
I=\frac13[\arctan(t^3)]_0^1=\frac\pi{12}.
```



(iii)


```math
\frac{t^4}{t^2+2t+5}=t^2-2t-1+\frac{6(2t+2)-7}{(t+1)^2+4},
```




```math
I=-\frac53+6\ln\frac85-\frac72\left(\frac\pi4-\arctan\frac12\right).
```



(iv)


```math
\frac{t}{(t+1)^2(2t+1)}=\frac1{t+1}+\frac1{(t+1)^2}-\frac2{2t+1},
```




```math
I=\left[\ln\frac{t+1}{2t+1}-\frac1{t+1}\right]_0^\infty=1-\ln2.
```



(v)


```math
\frac1{(t^2+4)(t+2)^2}=-\frac{t}{16(t^2+4)}+\frac1{16(t+2)}+\frac1{8(t+2)^2},
```




```math
I=\left[-\frac1{32}\ln(t^2+4)+\frac1{16}\ln(t+2)-\frac1{8(t+2)}\right]_0^\infty=\frac1{16}.
```



(vi)


```math
\frac{t}{t^3+1}=-\frac1{3(t+1)}+\frac{t+1}{3(t^2-t+1)},
```




```math
I=\left[-\frac13\ln(t+1)+\frac16\ln(t^2-t+1)
+\frac1{\sqrt3}\arctan\frac{2t-1}{\sqrt3}\right]_0^\infty
=\frac{2\pi}{3\sqrt3}.
```



## 2

(i) $\frac1{1+it}=\frac{1-it}{1+t^2}$, donc


```math
F(t)=\arctan t-\frac i2\ln(1+t^2).
```



(ii) $j=-\frac12+i\frac{\sqrt3}2$, donc


```math
\frac1{t-j}=\frac{t+\frac12+i\frac{\sqrt3}2}{t^2+t+1},
\qquad F(t)=\frac12\ln(t^2+t+1)+i\arctan\frac{2t+1}{\sqrt3}.
```



## 3

Par $x=\pi-t$,


```math
I=\int_0^\pi(\pi-t)\cos^2t\,dt,\qquad
2I=\pi\int_0^\pi\cos^2t\,dt=\frac{\pi^2}2.
```




```math
I=\frac{\pi^2}4,\qquad J=\int_0^\pi x\,dx-I=\frac{\pi^2}4.
```



## 4



```math
\cos t\cos2t\cos3t=\frac14(1+\cos2t+\cos4t+\cos6t).
```


La moyenne vaut $\frac14$.

## Autocorrection C

(i)


```math
\int_0^1t^2e^t\,dt=[(t^2-2t+2)e^t]_0^1=e-2.
```



(ii)


```math
\int_1^et^2\ln t\,dt=\left[\frac{t^3}3\ln t-\frac{t^3}9\right]_1^e=\frac{2e^3+1}9.
```



(iii)


```math
\int_0^\pi t\sin3t\,dt=\left[-\frac t3\cos3t+\frac19\sin3t\right]_0^\pi=\frac\pi3.
```



(iv)


```math
\int_0^1\frac t{\sqrt{t+1}}\,dt
=[2t\sqrt{t+1}]_0^1-2\int_0^1\sqrt{t+1}\,dt
=\frac{4-2\sqrt2}3.
```



(v)


```math
\int_1^2\frac{\ln t}{(1+t)^2}\,dt
=\left[-\frac{\ln t}{1+t}\right]_1^2+\int_1^2\frac{dt}{t(1+t)}
=\frac53\ln2-\ln3.
```



(vi)


```math
\int_0^1t^3e^{t^2}\,dt
=\left[\frac{t^2}2e^{t^2}\right]_0^1-\int_0^1te^{t^2}\,dt=\frac12.
```



(vii)


```math
I=-\frac\pi8+\int_0^1\frac{dx}{(x+1)(x^2+1)},
```




```math
\frac1{(x+1)(x^2+1)}=\frac1{2(x+1)}+\frac{1-x}{2(x^2+1)},
\qquad I=\frac14\ln2.
```



(viii)


```math
\int_0^1(\arcsin x)^2\,dx
=\left[x(\arcsin x)^2+2\arcsin x\sqrt{1-x^2}-2x\right]_0^1
=\frac{\pi^2}4-2.
```



(ix)


```math
\int_0^{\sqrt3}x^2\arctan x\,dx
=\left[\frac{x^3}3\arctan x-\frac{x^2}6+\frac16\ln(1+x^2)\right]_0^{\sqrt3}
=\frac\pi{\sqrt3}-\frac12+\frac13\ln2.
```



## 5



```math
\Im\frac{e^{(2+3i)x}}{2+3i}
=\frac{e^{2x}}{13}(2\sin3x-3\cos3x).
```


Par deux intégrations par parties, en notant $I=\int e^{2x}\sin3x\,dx$ :


```math
I=\frac12e^{2x}\sin3x-\frac32J,\qquad
J=\frac12e^{2x}\cos3x+\frac32I.
```


Donc $13I=e^{2x}(2\sin3x-3\cos3x)$, à constante près.



```math
\Re\left(\frac{e^{(1+i)x}}{2(1+i)}+\frac{e^{(-1+i)x}}{2(-1+i)}\right)
=\frac12(\sinh x\cos x+\cosh x\sin x).
```


Avec $K=\int\cosh x\cos x\,dx$ et $L=\int\sinh x\sin x\,dx$ :


```math
K=\sinh x\cos x+L,\qquad L=\cosh x\sin x-K.
```



## 6

À constante près, par intégration par parties :

(i) $x\arctan x-\frac12\ln(1+x^2)$.

(ii) $\frac{x^3}3\left((\ln x)^2-\frac23\ln x+\frac29\right)$.

(iii) $e^x(x^2-2x+2)$.

(iv) $x\tan x+\ln|\cos x|$.

(v) $x\ln(1+x^2)-2x+2\arctan x$.

(vi) $x\arcsin x+\sqrt{1-x^2}$.

(vii) $x\sinh x-\cosh x$.

(viii) $\frac{x^2}4-\frac{x\sin2x}4-\frac{\cos2x}8$.

(ix) $\frac{x^2+1}2\arctan x-\frac x2$.

## 7

1.


```math
I_{p,q}=\left[\frac{t^{p+1}}{p+1}(1-t)^q\right]_0^1
+\frac q{p+1}\int_0^1t^{p+1}(1-t)^{q-1}\,dt
=\frac q{p+1}I_{p+1,q-1}.
```



2.


```math
I_{p,0}=\frac1{p+1},\qquad
I_{p,q}=\frac{q!}{(p+1)\cdots(p+q)}\,\frac1{p+q+1}
=\frac{p!q!}{(p+q+1)!}.
```



3.


```math
I_{p,q}=\sum_{k=0}^q(-1)^k\binom qk\int_0^1t^{p+k}\,dt
=\sum_{k=0}^q\binom qk\frac{(-1)^k}{p+k+1}.
```



## Autocorrection D

(i) $u=\sqrt{t+1}$ :


```math
2\int_1^{\sqrt2}(u^2-1)\,du=\frac{4-2\sqrt2}3.
```



(ii) $u=\sqrt x$ :


```math
2\int_0^1u^3e^u\,du=2[e^u(u^3-3u^2+6u-6)]_0^1=12-4e.
```



(iii) $u=t^2-1$ :


```math
\frac12\int_3^8u^{-2}\,du=\frac5{48}.
```



(iv) $x=\sin u$ :


```math
\int_{-\pi/2}^{\pi/2}\cos^2u\,du=\frac\pi2.
```



(v) $u=\sqrt{e^x-1}$ :


```math
2\int_0^1\frac{u^2}{1+u^2}\,du=2-\frac\pi2.
```



(vi) $u=\ln t$ :


```math
\int_0^\pi e^u\sin u\,du
=\frac12[e^u(\sin u-\cos u)]_0^\pi=\frac{e^\pi+1}2.
```



(vii) $u=\sqrt x$ :


```math
2\int_{1/\sqrt3}^1\frac{du}{1+u^2}=\frac\pi6.
```



(viii) $u=\ln x$ :


```math
\int_0^{\ln2}u^2e^u\,du
=[e^u(u^2-2u+2)]_0^{\ln2}=2(\ln2)^2-4\ln2+2.
```



(ix) $u=x^3$ :


```math
\frac13\int_0^1\frac{du}{1+u^2}=\frac\pi{12}.
```



(x) $x=\sin u$ :


```math
\int_{-\pi/2}^{\pi/2}\sin^2u\cos^2u\,du=\frac\pi8.
```



(xi) $u=e^x$ :


```math
\int_1^e\frac{du}{u(1+u)}=\ln\frac{2e}{1+e}.
```



(xii) $u=\sqrt x$, puis $u=(1+\sin v)/2$ :


```math
2\int_{1/2}^1\sqrt{u(1-u)}\,du
=\frac12\int_0^{\pi/2}\cos^2v\,dv=\frac\pi8.
```



(xiii) $u=\cos t$ :


```math
\int_{-1}^1\frac{du}{3+u^2}=\frac\pi{3\sqrt3}.
```



(xiv) $u=1/t$ :


```math
\int_{1/2}^1\ln(1+u)\,du
=[(1+u)\ln(1+u)-(1+u)]_{1/2}^1
=\frac72\ln2-\frac32\ln3-\frac12.
```



## 8

À constante près :

(i) $u=\sqrt{e^x-1}$ : $2\arctan\sqrt{e^x-1}$.

(ii) $u=\sqrt{1+x}$ : $\frac23(1+x)^{3/2}-2\sqrt{1+x}$.

(iii) $u=e^x$ : $2\arctan(e^x)$.

(iv) $u=\ln x$ : $\frac x2(\sin(\ln x)-\cos(\ln x))$.

(v) $x=\sin u$ : $\frac12(x\sqrt{1-x^2}+\arcsin x)$.

(vi) $u=\sqrt{x^2-1}$ : $\arctan\sqrt{x^2-1}$, pour $|x|>1$.

(vii) $u=\ln t$ : $\frac12\ln(1+(\ln t)^2)$.

(viii)


```math
\frac{\cos x}{\sin x+\cos x}
=\frac12+\frac12\frac{\cos x-\sin x}{\sin x+\cos x},
```


donc $\frac x2+\frac12\ln|\sin x+\cos x|$.

## 9

1. $\frac12(\ln x)^2$.

2. $\beta=1/(\alpha+1)$, $x=t^\beta$ :


```math
x^\alpha\ln x\,dx=\beta^2\ln t\,dt,
```




```math
F(x)=\beta^2(t\ln t-t)
=x^{\alpha+1}\left(\frac{\ln x}{\alpha+1}-\frac1{(\alpha+1)^2}\right).
```



## 10

1. $t=\tan(x/2)$ :


```math
\frac{dx}{\sin x+\tan x}=\frac{1-t^2}{2t}\,dt,\qquad
F(x)=\frac12\ln\left|\tan\frac x2\right|-\frac14\tan^2\frac x2.
```


Avec $u=\cos x$ :


```math
-\frac{u}{(1-u)(1+u)^2}
=-\frac1{4(1-u)}-\frac1{4(1+u)}+\frac1{2(1+u)^2},
```




```math
F(x)=\frac14\ln\left|\frac{1-\cos x}{1+\cos x}\right|
-\frac1{2(1+\cos x)}.
```


Les deux primitives diffèrent d'une constante.

2. (i) $u=\cos x$ :


```math
\int_{\pi/3}^{\pi/2}\frac{dx}{\sin x}
=\int_0^{1/2}\frac{du}{1-u^2}=\frac12\ln3.
```



(ii) $u=\cos x$ :


```math
\int_{-1}^1\frac{du}{4-u^2}=\frac12\ln3.
```



(iii) $u=\sin x$ :


```math
\int_{-1/2}^{1/2}\frac{du}{(1-u^2)^2}
=\left[\frac{u}{2(1-u^2)}+\frac14\ln\frac{1+u}{1-u}\right]_{-1/2}^{1/2}
=\frac23+\frac12\ln3.
```



(iv) $t=\tan(x/2)$ :


```math
2\int_0^1\frac{dt}{3+t^2}=\frac\pi{3\sqrt3}.
```



## 11

1. Par $t=\pi/2-u$, les deux intégrales sont égales ; leur somme vaut $\pi/2$. Chacune vaut $\pi/4$.

2. Avec $t=\sin u$ :


```math
\int_0^1\frac{dt}{\sqrt{1-t^2}+t}
=\int_0^{\pi/2}\frac{\cos u}{\cos u+\sin u}\,du=\frac\pi4.
```



## 12



```math
I=\int_{1/x}^x\frac{\ln t}{1+t^2}\,dt
\overset{t=1/u}=\int_{1/x}^x\frac{-\ln u}{1+u^2}\,du=-I.
```


Donc $I=0$.

## 13

$x\ln x\to0$ en $0^+$ : prolongement continu par $0$. Avec $u=x^2$,


```math
I=\frac14\int_0^1\frac{\ln u}{(1+u)^2}\,du
=\frac14\left[\frac{u\ln u}{1+u}\right]_0^1-\frac14\int_0^1\frac{du}{1+u}
=-\frac14\ln2.
```



## 14

1. Par $t=a+b-u$,


```math
I=\int_a^btf(t)\,dt=\int_a^b(a+b-u)f(u)\,du,\qquad
I=\frac{a+b}2\int_a^bf.
```



2. $f(t)=(1+\sin t)^{-1}=f(\pi-t)$ et, avec $u=\tan(t/2)$,


```math
\int_0^\pi f(t)\,dt=2\int_0^\infty\frac{du}{(1+u)^2}=2.
```


L'intégrale demandée vaut $\pi$.

## 15

1.


```math
\left(\frac{t}{(1+t^2)^{n+1}}\right)'
=\frac{2n+2}{(1+t^2)^{n+2}}-\frac{2n+1}{(1+t^2)^{n+1}},
```




```math
I_{n+1}(x)=\frac{x}{2(n+1)(1+x^2)^{n+1}}+\frac{2n+1}{2n+2}I_n(x).
```



2. $I_0(x)=\arctan x$. Par récurrence, $J_n=\lim_{x\to\infty}I_n(x)$ existe et


```math
J_0=\frac\pi2,\qquad J_{n+1}=\frac{2n+1}{2n+2}J_n,\qquad
J_n=\frac\pi2\,\frac{(2n)!}{4^n(n!)^2}.
```



## 16



```math
\frac1{c-a}\int_a^cf
=\frac{b-a}{c-a}\left(\frac1{b-a}\int_a^bf\right)
+\frac{c-b}{c-a}\left(\frac1{c-b}\int_b^cf\right).
```


Les coefficients sont positifs et de somme $1$ : la moyenne est au plus le maximum.

## 17

Soit $T>0$ une période de $f$ et $F$ une primitive.


```math
F(x+T)-F(x)=\int_x^{x+T}f=\int_0^Tf.
```


Si $\int_0^Tf=0$, toute primitive est $T$-périodique.
Réciproquement, une primitive périodique est bornée ; or


```math
F(nT)=F(0)+n\int_0^Tf.
```


Donc $\int_0^Tf=0$.

## 18

Pour $a<b$,


```math
\int_a^bf=\int_a^b|f|
\iff\int_a^b(|f|-f)=0
\iff |f|-f=0
\iff f\geq0.
```


La deuxième équivalence utilise la continuité et la positivité. Si $a=b$, toute fonction convient.

## 19

$g(x)=f(x)-x$ est continue et $g(0)\geq0$. Sans zéro, $g>0$ sur $[0,1]$, donc


```math
\int_0^1f(x)\,dx>\int_0^1x\,dx=\frac12,
```


contradiction.

## 20



```math
F(x)=\int_a^xf(t)\,dt=0,\qquad f=F'=0.
```



## 21



```math
\int_0^1f^2(f-1)^2
=\int_0^1f^4-2\int_0^1f^3+\int_0^1f^2=0.
```


L'intégrande continue est positive : $f(x)\in\{0,1\}$. Par le théorème des valeurs intermédiaires, $f=0$ ou $f=1$.

## 22



```math
\alpha\leq f\leq\beta
\implies(f-\alpha)(f-\beta)\leq0
\implies f^2\leq(\alpha+\beta)f-\alpha\beta.
```


En intégrant, $\int_0^1f^2\leq-\alpha\beta$.

## Autocorrection E



```math
m=\frac1{b-a}\int_a^bf,\qquad
G(x)=\int_a^xf-m(x-a),\qquad G(a)=G(b)=0.
```


Par Rolle, $\exists c\in(a,b)$ tel que $0=G'(c)=f(c)-m$.

## Autocorrection F



```math
\frac1x\int_0^xf(t)\,dt=\int_0^1f(xu)\,du\longrightarrow f(0),
```


car $\sup_{0\leq u\leq1}|f(xu)-f(0)|\to0$.

## 23

1.


```math
\frac1{x^2}\int_0^xtf(t)\,dt=\int_0^1u f(xu)\,du\longrightarrow\frac{f(0)}2.
```



2. Si $f$ est continue par morceaux,


```math
\lim_{x\to0^+}\frac1{x^2}\int_0^xtf(t)\,dt=\frac{f(0^+)}2,\qquad
\lim_{x\to0^-}\frac1{x^2}\int_0^xtf(t)\,dt=\frac{f(0^-)}2.
```


La limite existe si et seulement si $f(0^-)=f(0^+)$. La valeur choisie pour $f(0)$ n'intervient pas.

## 24

Pour une primitive $F$ de $f$,


```math
F(x+T)-F(x)=\text{constante}
\implies f(x+T)-f(x)=0.
```



## 25

1. La linéarité de l'intégrale donne celle de $P_0$. De plus,


```math
\ker P_0=\{0\},\qquad
\operatorname{Im}P_0=\{F\in C^1(\mathbb R):F(0)=0\}.
```


En effet, $(P_0f)'=f$ ; réciproquement $F=P_0(F')$ si $F(0)=0$.

2.


```math
P_af(x)=\int_a^xf,\qquad \ker P_a=\{0\},\qquad
\operatorname{Im}P_a=\{F\in C^1(\mathbb R):F(a)=0\}.
```



3. Toute primitive est $P_0f+C$, et


```math
\int_0^1(P_0f+C)=0
\iff C=-\int_0^1P_0f.
```


Ainsi $\Pi f=P_0f-\int_0^1P_0f$ est définie de façon unique et linéaire.
Son image est $\{G\in C^1(\mathbb R):\int_0^1G=0\}$ et son noyau $\{0\}$.

## 26

Soit $F$ une primitive de $f$.



```math
G_1(x)=F(x^2)-F(2x),\qquad G_1'(x)=2xf(x^2)-2f(2x).
```




```math
G_2(x)=x(F(x)-F(0)),\qquad
G_2'(x)=\int_0^xf(t)\,dt+xf(x).
```




```math
G_3(x)=\int_x^{2x}f(u)\,du=F(2x)-F(x),\qquad
G_3'(x)=2f(2x)-f(x).
```




```math
G_4(x)=\int_{\pi x}^{2\pi x}\frac{\cos u}{u}\,du,\qquad
G_4'(x)=\frac{\cos(2\pi x)-\cos(\pi x)}x\quad(x>0).
```


Ces dérivées sont continues sur leurs domaines.

## 27

1. $\sinh t/t\to1$ en $0$ : $\varphi$ est continue et paire. Donc $f$ est bien définie et


```math
f(-x)=\int_{-x}^{-2x}\varphi(t)\,dt=-\int_x^{2x}\varphi(u)\,du=-f(x).
```



2.


```math
f'(x)=2\varphi(2x)-\varphi(x)
=\begin{cases}
\dfrac{\sinh(2x)-\sinh x}{x},&x\ne0,\\
1,&x=0.
\end{cases}
```



3. $\sinh$ est strictement croissante : $f'(x)>0$ partout.
Pour $x\geq0$, $\varphi\geq1$, donc $f(x)\geq x$.
Ainsi $f$ croît strictement de $-\infty$ à $+\infty$, avec $f(0)=0$.

## 28

Pour $a<x<b$,


```math
F(x)=\int_a^x(x-t)f(t)\,dt+\int_x^b(t-x)f(t)\,dt,
```




```math
F'(x)=\int_a^xf(t)\,dt-\int_x^bf(t)\,dt.
```


Pour $x<a$, $F'(x)=-\int_a^bf$ ; pour $x>b$, $F'(x)=\int_a^bf$.
Les dérivées se raccordent en $a,b$ : $F\in C^1(\mathbb R)$.
Sur $(a,b)$, $F''=2f$.

## 29



```math
H(x)=\int_0^xe^{t^2}\,dt,\qquad H'(x)=e^{x^2}>0.
```


$H$ est lisse, strictement croissante et tend vers $\pm\infty$ aux deux extrémités ; c'est une bijection de $\mathbb R$ sur $\mathbb R$.


```math
\int_x^ye^{t^2}\,dt=1
\iff H(y)=H(x)+1
\iff y=H^{-1}(H(x)+1).
```


$H^{-1}$ est lisse puisque $H'$ ne s'annule pas. Ainsi


```math
\varphi=H^{-1}\circ(H+1)\in C^\infty(\mathbb R),\qquad
\varphi'(x)=e^{x^2-\varphi(x)^2}.
```



## Autocorrection G

Sur $[\pi/6,\pi/3]$, $1/\sqrt3\leq\tan x\leq\sqrt3$. Donc


```math
\frac1{\sqrt3}\int_{\pi/6}^{\pi/3}\frac{dx}x
\leq\int_{\pi/6}^{\pi/3}\frac{\tan x}x\,dx
\leq\sqrt3\int_{\pi/6}^{\pi/3}\frac{dx}x.
```


Les deux bornes sont $\ln2/\sqrt3$ et $\sqrt3\ln2$.

## Autocorrection H



```math
t-1\leq\lfloor t\rfloor\leq t
\implies\frac{x^2}2-x\leq\int_0^x\lfloor t\rfloor\,dt\leq\frac{x^2}2.
```


Donc $\int_0^x\lfloor t\rfloor\,dt\sim x^2/2$.

## 30



```math
\int_e^\pi\frac{dx}x=\ln\pi-1<\frac{\pi-e}e.
```


Donc $e\ln\pi<\pi$, puis $\pi^e<e^\pi$.

## 31

1.


```math
X^4(1-X)^4=(1+X^2)(X^6-4X^5+5X^4-4X^2+4)-4.
```


Donc $Q=X^6-4X^5+5X^4-4X^2+4$ et $\alpha=-4$.

2.


```math
I=\frac17-\frac46+\frac55-\frac43+4-4\arctan1
=\frac{22}7-\pi>0.
```



3. $\frac12\leq(1+x^2)^{-1}\leq1$, et


```math
\int_0^1x^4(1-x)^4\,dx=\frac{4!4!}{9!}=\frac1{630}.
```


Ainsi $1/1260\leq I\leq1/630$, d'où


```math
\frac{1979}{630}\leq\pi\leq\frac{3959}{1260}.
```



## 32

Pour $0\leq t\leq1$,


```math
t\leq\frac{1+t^2}2\leq\frac{1+t}2.
```


Donc


```math
\frac1{n+1}\leq\int_0^1\left(\frac{1+t^2}2\right)^n\,dt
\leq\frac2{n+1}\left(1-\frac1{2^{n+1}}\right)\leq\frac2{n+1}.
```



## 33

Pour $x>1$,


```math
\int_x^{2x}\frac t{\ln t}\,dt\geq\frac{x^2}{\ln(2x)}
\longrightarrow+\infty.
```


Pour chaque entier $k\geq1$ et $t\in[k\pi+\pi/4,k\pi+3\pi/4]$,


```math
\sin^2t\geq\frac12,\qquad\arctan t\geq\frac\pi4.
```


Chaque intervalle fournit au moins $\pi^2/16$ à l'intégrale ; le nombre d'intervalles inclus dans $[0,x]$ tend vers l'infini.

## 34



```math
F(x)=\int_0^xf(t)\,dt\geq0,\qquad F'\leq KF.
```




```math
\bigl(e^{-Kx}F(x)\bigr)'=e^{-Kx}(F'-KF)\leq0.
```


Cette fonction est positive et vaut $0$ en $0$ : $F=0$, puis $f=F'=0$.

## 35

1. Pour $C=1/\varepsilon$,


```math
f(x)^2-f(a)^2=2\int_a^xff'
\leq\frac1\varepsilon\int_a^bf^2+\varepsilon\int_a^b(f')^2,
```


par $2|uv|\leq\varepsilon^{-1}u^2+\varepsilon v^2$.

2. Il existe $c\in[a,b]$ tel que $f(c)^2\leq(b-a)^{-1}\int_a^bf^2$. Pour tout $x$,


```math
f(x)^2\leq f(c)^2+2\int_a^b|ff'|
\leq\left(\frac1{b-a}+\frac1\varepsilon\right)\int_a^bf^2
+\varepsilon\int_a^b(f')^2.
```


Prendre $D=(b-a)^{-1}+\varepsilon^{-1}$.

## 36

Pour $n\in\mathbb N^*$,


```math
a_n=-\frac1n\int_0^{2\pi}f'(t)\sin(nt)\,dt.
```


Sur chaque période, en posant $a=2k\pi/n$,


```math
\int_a^{a+2\pi/n}f'(t)\sin(nt)\,dt
=\int_0^{\pi/n}\bigl(f'(a+s)-f'(a+\pi/n+s)\bigr)\sin(ns)\,ds\leq0,
```


car $f'$ est croissante. En sommant pour $0\leq k<n$, $a_n\geq0$.

## 37

Posons $m=\int_0^1g\in[a,b]$. Si $a<m<b$, une droite d'appui en $m$ donne un réel $p$ tel que


```math
f(y)\geq f(m)+p(y-m)\qquad(a\leq y\leq b).
```


Donc


```math
\int_0^1f(g(t))\,dt\geq f(m)+p\left(\int_0^1g-m\right)=f(m).
```


Si $m=a$, la fonction positive $g-a$ a une intégrale nulle ; $g=a$ sauf éventuellement aux points de la subdivision, et l'égalité suit. Même argument pour $m=b$.

L'argument vaut dès que $f\circ g$ est intégrable. Pour l'intégrale de Riemann, la continuité de $f$ aux bornes suffit ; sans cette hypothèse, l'intégrale de Lebesgue donne le même résultat.

## 38

1. Pour $0\leq u\leq1$,


```math
f(a+u(b-a))\leq(1-u)f(a)+uf(b),
```




```math
f\left(\frac{a+b}2\right)\leq
\frac{f(a+u(b-a))+f(b-u(b-a))}2.
```


En intégrant en $u$ :


```math
f\left(\frac{a+b}2\right)
\leq\frac1{b-a}\int_a^bf
\leq\frac{f(a)+f(b)}2.
```



2. Posons $M=\|f''\|_\infty$, $m=(a+b)/2$ et $h=b-a$.
Taylor donne $|f(x)-f(m)-f'(m)(x-m)|\leq M(x-m)^2/2$ ; ainsi


```math
\left|\int_a^bf-hf(m)\right|
\leq\frac M2\int_a^b(x-m)^2\,dx=\frac{Mh^3}{24}.
```


Si $\ell$ est la corde reliant $(a,f(a))$ à $(b,f(b))$, alors


```math
|f(x)-\ell(x)|\leq\frac M2(x-a)(b-x).
```


En effet, les fonctions $\frac M2(x-a)(b-x)\pm(f-\ell)$ sont concaves et nulles aux bornes. Donc


```math
\left|\int_a^bf-\frac h2(f(a)+f(b))\right|\leq\frac{Mh^3}{12}.
```



3. Sur chacun des $n$ intervalles $[k/n,(k+1)/n]$, appliquer 2 puis sommer :


```math
\left|\int_0^1f-\frac1n\sum_{k=0}^{n-1}f\left(\frac{2k+1}{2n}\right)\right|
\leq\frac M{24n^2},
```




```math
\left|\int_0^1f-\frac1n\left(\frac{f(0)}2+\sum_{k=1}^{n-1}f\left(\frac kn\right)+\frac{f(1)}2\right)\right|
\leq\frac M{12n^2}.
```


Ce sont les aires des rectangles de hauteur prise au milieu et des trapèzes reliant deux valeurs successives.

## 39

1. Pour une fonction continue par morceaux, soit $M$ le supremum de $|f|$ après exclusion des valeurs isolées aux points de subdivision. Alors


```math
\|f\|_p\leq M.
```


Pour tout $\varepsilon>0$ avec $\varepsilon<M$, il existe un intervalle de longueur $\delta>0$ sur lequel $|f|\geq M-\varepsilon$, donc


```math
\|f\|_p\geq(M-\varepsilon)\delta^{1/p}\longrightarrow M-\varepsilon.
```


Ainsi $\|f\|_p\to M$. Pour $f$ continue, $M=\|f\|_\infty$ ; une valeur isolée ne compte pas dans l'intégrale.

2. On prend $q=p/(p-1)$ ; la fraction imprimée dans l'énoncé est inversée.

(a) La concavité de $\ln$, avec poids $1/p,1/q$, donne


```math
\frac1p\ln a+\frac1q\ln b\leq\ln\left(\frac ap+\frac bq\right),
```


donc $a^{1/p}b^{1/q}\leq a/p+b/q$. Les cas $a=0$ ou $b=0$ sont immédiats.

(b) Si $\|f\|_p=\|g\|_q=1$, appliquer Young à $a=|f|^p$, $b=|g|^q$ :


```math
\int_0^1|fg|\leq\frac1p\int_0^1|f|^p+\frac1q\int_0^1|g|^q=1.
```


Par homogénéité,


```math
\left|\int_0^1fg\right|\leq\int_0^1|fg|\leq\|f\|_p\|g\|_q.
```


Si une norme est nulle, le produit est nul en dehors des points de subdivision.

(c) Si $p_1<p_2$, Hölder appliquée à $|f|^{p_1}$ et $1$, avec exposants $p_2/p_1$ et $p_2/(p_2-p_1)$, donne


```math
\int_0^1|f|^{p_1}\leq\left(\int_0^1|f|^{p_2}\right)^{p_1/p_2},
\qquad\|f\|_{p_1}\leq\|f\|_{p_2}.
```



3. (a)


```math
|f+g|^p\leq(|f|+|g|)|f+g|^{p-1}.
```



(b) En intégrant puis en appliquant Hölder,


```math
\|f+g\|_p^p\leq(\|f\|_p+\|g\|_p)
\left(\int_0^1|f+g|^{(p-1)q}\right)^{1/q}
=(\|f\|_p+\|g\|_p)\|f+g\|_p^{p-1}.
```


Si $\|f+g\|_p>0$, on divise ; sinon l'inégalité est immédiate.

## 40



```math
|I_n|\leq\int_0^1\frac{t^n|\sin nt|}{1+t^3}\,dt
\leq\int_0^1t^n\,dt=\frac1{n+1}\longrightarrow0.
```



## 41

1. $0\leq I_n\leq\int_0^1x^n\,dx=1/(n+1)$, donc $I_n\to0$.

2.


```math
I_n+I_{n+1}=\int_0^1x^n\,dx=\frac1{n+1},
```




```math
\sum_{k=0}^N\frac{(-1)^k}{k+1}
=\sum_{k=0}^N(-1)^k(I_k+I_{k+1})
=I_0+(-1)^NI_{N+1}\longrightarrow\ln2.
```



## 42

1. Le raccord en $1/n$ vaut $0$ des deux côtés, donc $f_n$ est continue.


```math
\int_0^1f_n(x)\,dx=2n\int_0^{1/n}(1-nx)\,dx=1.
```



2. Pour $x>0$, $f_n(x)=0$ dès $n>1/x$, tandis que $f_n(0)=2n\to+\infty$.
La limite ponctuelle vaut $0$ hors de $0$. Son intégrale impropre, ou celle de son prolongement par $0$, vaut $0$, alors que


```math
\lim_n\int_0^1f_n=1.
```


La limite ponctuelle n'est pas une fonction réelle finie au point $0$.

## 43

Soit $M=\|f\|_\infty$. Pour $0<\delta<1$,


```math
\left|\int_0^1f(x^n)\,dx-f(0)\right|
\leq\sup_{0\leq u\leq(1-\delta)^n}|f(u)-f(0)|+2M\delta.
```


À $\delta$ fixé, le premier terme tend vers $0$, puis $\delta\to0$ :


```math
\int_0^1f(x^n)\,dx\longrightarrow f(0).
```



## 44

1. $|u_n|\leq\|f\|_\infty/(n+1)\to0$.

2. Par parties,


```math
u_n=\frac{f(1)}{n+1}-\frac1{n+1}\int_0^1t^{n+1}f'(t)\,dt
=\frac{f(1)}{n+1}+O(n^{-2})
\sim\frac{f(1)}n.
```



3.


```math
\int_0^1t^n\sin\frac{\pi t}2\,dt\sim\frac1n,
```




```math
\int_0^1t^n\cos\frac{\pi t}2\,dt
=\frac{\pi}{2(n+1)}\int_0^1t^{n+1}\sin\frac{\pi t}2\,dt
\sim\frac{\pi}{2n^2}.
```



## 45

1.


```math
\int_a^bf(t)\cos(nt)\,dt
=\left[\frac{f(t)\sin(nt)}n\right]_a^b
-\frac1n\int_a^bf'(t)\sin(nt)\,dt,
```


donc la valeur absolue est au plus $(2\|f\|_\infty+(b-a)\|f'\|_\infty)/n$.

2. Par continuité uniforme, pour tout $\varepsilon>0$, choisir une fonction en escalier $g$ telle que $\|f-g\|_\infty\leq\varepsilon$.
Chaque intégrale de $\cos(nt)$ sur un intervalle tend vers $0$, donc $\int_a^bg(t)\cos(nt)\,dt\to0$.


```math
\limsup_n\left|\int_a^bf(t)\cos(nt)\,dt\right|
\leq(b-a)\varepsilon.
```


Puis $\varepsilon\to0$.

## Autocorrection I

(i) $\int_0^1\sin(\pi x)\,dx=2/\pi$.

(ii) $\int_0^1x/(1+x^2)\,dx=\frac12\ln2$.

(iii) $\int_1^2dx/x=\ln2$ ; les deux extrémités présentes dans la somme ne changent pas la limite.

## 46

(i)


```math
\frac1{n^2}\sum_{k=1}^nke^{-k/n}
=\frac1n\sum_{k=1}^n\frac kn e^{-k/n}
\longrightarrow\int_0^1xe^{-x}\,dx=1-\frac2e.
```



(ii)


```math
\frac1{n^2}\sum_{k=1}^n(\ln(k^k)-\ln(n^k))
=\frac1n\sum_{k=1}^n\frac kn\ln\frac kn
\longrightarrow\int_0^1x\ln x\,dx=-\frac14,
```


avec le prolongement $x\ln x=0$ en $0$.

(iii) $\int_0^1\cos^2(\pi x)\,dx=\frac12$.

(iv)


```math
n\sum_{k=1}^n\frac1{(n+k)^2}
=\frac1n\sum_{k=1}^n\frac1{(1+k/n)^2}
\longrightarrow\int_0^1\frac{dx}{(1+x)^2}=\frac12.
```



(v)


```math
\frac{\sum_{k=1}^n\sqrt k}{n\sqrt n}
\longrightarrow\int_0^1\sqrt x\,dx=\frac23.
```



(vi) Le logarithme de la suite tend vers


```math
\int_0^1\ln(1+x^2)\,dx
=[x\ln(1+x^2)-2x+2\arctan x]_0^1
=\ln2-2+\frac\pi2.
```


La limite vaut $2e^{\pi/2-2}$.

(vii)


```math
\sum_{k=1}^n\frac1{\sqrt{4n^2-k^2}}
\longrightarrow\int_0^1\frac{dx}{\sqrt{4-x^2}}=\frac\pi6.
```



(viii)


```math
\frac1n\prod_{k=1}^n(n+k)^{1/n}
=\exp\left(\frac1n\sum_{k=1}^n\ln(1+k/n)\right)
\longrightarrow\exp\left(\int_0^1\ln(1+x)\,dx\right)=\frac4e.
```



## 47



```math
\frac e{4n}\left(\frac{(2n)!}{n!}\right)^{1/n}
=\frac e4\exp\left(\frac1n\sum_{k=1}^n\ln(1+k/n)\right)
\longrightarrow\frac e4e^{2\ln2-1}=1.
```



## 48

1.


```math
S_n=\left(\frac1n\sum_{k=1}^nf(k/n)\right)^2
\longrightarrow\left(\int_0^1f\right)^2.
```



2. Par symétrie des indices,


```math
2T_n=S_n+\frac1{n^2}\sum_{k=1}^nf(k/n)^2.
```


Le dernier terme est au plus $\|f\|_\infty^2/n$, donc


```math
T_n\longrightarrow\frac12\left(\int_0^1f\right)^2.
```



## 49



```math
\left|\frac1n\sum_{k=0}^{n-1}f(k/n)
\left(g((k+1)/n)-g(k/n)\right)\right|
\leq\|f\|_\infty\,\omega_g(1/n)\longrightarrow0,
```


où $\omega_g$ est le module de continuité uniforme de $g$.
La somme avec $g(k/n)$ tend vers $\int_0^1fg$ ; c'est donc la limite demandée.

## 50



```math
n\sum_{k=1}^n\frac1{n^2+k^2}
=\frac1n\sum_{k=1}^n\frac1{1+(k/n)^2}\longrightarrow\frac\pi4,
```




```math
n\sum_{k=n+1}^{2n}\frac1{k^2}
=\frac1n\sum_{k=n+1}^{2n}\frac1{(k/n)^2}\longrightarrow\int_1^2\frac{dx}{x^2}=\frac12.
```


Les équivalents sont $\pi/(4n)$ et $1/(2n)$.

## 51

1. Posons $F(x)=\int_a^xf$ et $S=F(b)>0$. Comme $F'=f>0$, $F$ est une bijection de $[a,b]$ sur $[0,S]$.


```math
x_k=F^{-1}(kS/n)\qquad(0\leq k\leq n)
```


définit l'unique subdivision demandée.

2. La fonction $u\mapsto f(F^{-1}(Su))$ est continue sur $[0,1]$. Donc


```math
\frac1n\sum_{k=0}^nf(x_k)
\longrightarrow\int_0^1f(F^{-1}(Su))\,du
=\frac1S\int_a^bf(x)^2\,dx.
```


La limite vaut $\displaystyle\frac{\int_a^bf^2}{\int_a^bf}$.

## Autocorrection J

(i) Pour $x\geq0$, les restes intégraux donnent


```math
\ln(1+x)-x+\frac{x^2}2
=\int_0^x\frac{(x-t)^2}{(1+t)^3}\,dt\geq0,
```




```math
\ln(1+x)-x+\frac{x^2}2-\frac{x^3}3
=-\int_0^x\frac{(x-t)^3}{(1+t)^4}\,dt\leq0.
```



(ii) Pour $0\leq x\leq\pi/2$,


```math
\sin x-x+\frac{x^3}6
=\frac1{3!}\int_0^x(x-t)^3\sin t\,dt\geq0,
```




```math
\sin x-x+\frac{x^3}6-\frac{x^5}{120}
=-\frac1{5!}\int_0^x(x-t)^5\sin t\,dt\leq0.
```



## 52

Toutes les dérivées de $\sin$ et $\cos$ sont majorées en valeur absolue par $1$. Taylor-Lagrange donne


```math
\left|\sin x-\sum_{k=0}^n\frac{(-1)^kx^{2k+1}}{(2k+1)!}\right|
\leq\frac{|x|^{2n+2}}{(2n+2)!}\longrightarrow0,
```




```math
\left|\cos x-\sum_{k=0}^n\frac{(-1)^kx^{2k}}{(2k)!}\right|
\leq\frac{|x|^{2n+1}}{(2n+1)!}\longrightarrow0.
```



## 53

1. Pour $0\leq x\leq1$, les restes intégraux donnent $x-x^3/6\leq\sin x\leq x$.
Les termes étant positifs,


```math
x^2-\frac{x^4}3\leq\left(x-\frac{x^3}6\right)^2\leq\sin^2x\leq x^2.
```



2.


```math
0\leq\sum_{k=1}^n\frac1{n+k}
-\sum_{k=1}^n\sin^2\frac1{\sqrt{n+k}}
\leq\frac13\sum_{k=1}^n\frac1{(n+k)^2}\leq\frac1{3n}.
```


La somme harmonique tend vers $\ln2$ ; la limite cherchée est $\ln2$.

## 54

1. Pour $t\geq0$,


```math
\frac1{1+t}=\sum_{k=0}^{n-1}(-t)^k+\frac{(-t)^n}{1+t}.
```


En intégrant de $0$ à $x$,


```math
\ln(1+x)-\sum_{k=1}^n\frac{(-1)^{k-1}}k x^k
=(-1)^n\int_0^x\frac{t^n}{1+t}\,dt,
```


d'où une valeur absolue au plus $x^{n+1}/(n+1)$.

2. Avec $x=1$, la somme tend vers $\ln2$, avec erreur au plus $1/(n+1)$.

3. $\ln(1/2)=-\ln2$ et $\ln4=2\ln2$ : prendre l'opposé ou le double des sommes précédentes ; erreurs au plus $1/(n+1)$ et $2/(n+1)$.

## 55

1. Le degré impair assure une racine réelle $a$ de $P$. Pour tout $k$,


```math
|f^{(k)}(a)|\leq|P(a)|=0.
```


Fixons $x$ et $M=\max_{t\in[\min(a,x),\max(a,x)]}|P(t)|$. Taylor-Lagrange à tout ordre donne


```math
|f(x)|\leq M\frac{|x-a|^{n+1}}{(n+1)!}\longrightarrow0.
```


Donc $f=0$.

2. Non : $P(X)=1+X^2$ et $f(x)=1$ vérifient toutes les inégalités.

## 56

1. Les ensembles $\{|f(x)|:x\in\mathbb R\}$ et $\{|f''(x)|:x\in\mathbb R\}$ sont non vides et majorés ; $M_0,M_2$ existent et sont finis.

2.


```math
|f(x_0+h)-f(x_0)-hf'(x_0)|\leq\frac{M_2h^2}2,
```


donc


```math
|f'(x_0)|\leq\frac{2M_0}h+\frac{M_2h}2.
```



3. Si $M_0M_2>0$, prendre $h=2\sqrt{M_0/M_2}$ :


```math
|f'(x_0)|\leq2\sqrt{M_0M_2}.
```


Si $M_0=0$, $f=0$. Si $M_2=0$, laisser $h\to\infty$ dans la borne précédente : $f'=0$.

## 57

1.


```math
\int_0^{2\pi}e^{in\theta}\,d\theta=
\begin{cases}2\pi,&n=0,\\0,&n\in\mathbb Z\setminus\{0\}.\end{cases}
```



2. (a) Si $P(X)=\sum_{k=0}^da_kX^k$,


```math
\frac1{2\pi}\int_0^{2\pi}P(re^{i\theta})\,d\theta
=\sum_{k=0}^da_kr^k\frac1{2\pi}\int_0^{2\pi}e^{ik\theta}\,d\theta=a_0=P(0).
```



(b) Appliquer (a) au polynôme $Q(X)=P(z+X)$ :


```math
P(z)=\frac1{2\pi}\int_0^{2\pi}P(z+re^{i\theta})\,d\theta.
```


La valeur au centre est la moyenne sur le cercle.

3. La continuité de $|P|$ sur le cercle compact $\mathbb U$ assure l'existence de $M=\max_{\mathbb U}|P|$.


```math
a_k=\frac1{2\pi}\int_0^{2\pi}P(e^{i\theta})e^{-ik\theta}\,d\theta,
```


donc $|a_k|\leq M$ pour chaque $k$.

## 58

1. $f(0)=0$ implique $g(x)=f(x)/x\to f'(0)$. Poser $g(0)=f'(0)$.

2. Par Leibniz, pour $x\ne0$,


```math
g^{(n)}(x)=\frac{(-1)^nn!}{x^{n+1}}
\sum_{k=0}^n\frac{(-x)^k}{k!}f^{(k)}(x).
```


Taylor de $f$ entre $x$ et $0$, avec $f(0)=0$, donne


```math
g^{(n)}(x)=\frac1{x^{n+1}}\int_0^xt^nf^{(n+1)}(t)\,dt
=\int_0^1u^nf^{(n+1)}(xu)\,du.
```



3. Par parties,


```math
g^{(n)}(x)=\frac{f^{(n+1)}(x)}{n+1}
-\frac1{(n+1)x^{n+1}}\int_0^xt^{n+1}f^{(n+2)}(t)\,dt.
```


Le second terme est $O(|x|)$ au voisinage de $0$, donc


```math
\lim_{x\to0}g^{(n)}(x)=\frac{f^{(n+1)}(0)}{n+1}.
```



4. Par prolongement des dérivées, successivement à chaque ordre,


```math
g\in C^\infty(\mathbb R),\qquad
g^{(n)}(0)=\frac{f^{(n+1)}(0)}{n+1}.
```



## 59

Sans zéro de $f'$, sa continuité impose $f'>0$ partout ou $f'<0$ partout.
Dans le premier cas, $f(t)<f(1)$ pour $t<1$, donc $\int_0^1f<f(1)$.
Dans le second, $\int_0^1f>f(1)$.
Les deux cas contredisent l'hypothèse : $\exists c\in[0,1]$, $f'(c)=0$.

## 60

Supposons que $f$ ne change de signe que $m<n$ fois. Choisir des zéros $c_1<\cdots<c_m$ séparant les changements de signe, et


```math
Q(X)=\prod_{j=1}^m(X-c_j).
```


Quitte à remplacer $Q$ par $-Q$, $Qf\geq0$ sur $[a,b]$ et $Qf$ n'est pas identiquement nulle. Ainsi $\int_a^bQf>0$.
Or $\deg Q=m\leq n-1$, donc la linéarité et les hypothèses donnent $\int_a^bQf=0$.
Contradiction. S'il y a une infinité de changements, la conclusion est immédiate.

## 61

Soit $M=\|f\|_\infty$. Pour $n>2M$, tous les facteurs sont positifs. Uniformément pour $|u|\leq M/n$,


```math
\ln(1+u)=u+O(u^2).
```


Donc


```math
\ln\prod_{k=1}^n\left(1+\frac1nf(k/n)\right)
=\frac1n\sum_{k=1}^nf(k/n)+O(n^{-1})
\longrightarrow\int_0^1f.
```


La limite vaut $\displaystyle\exp\left(\int_0^1f\right)$.

## 62

$P$ ne peut être constant : pour $P=c$, prendre $f(t)=(t-c)^2$.
Par approximation continue des indicatrices d'intervalles,


```math
|P^{-1}(J)\cap[0,1]|=|J|\qquad(J\subset[0,1]\text{ intervalle}),
```


où $|\cdot|$ désigne la longueur. Les préimages des extrémités sont finies, puisque $P$ n'est pas constant ; elles ne contribuent pas aux intégrales.

L'image de $[0,1]$ est tout $[0,1]$ : sinon un intervalle $J$ de longueur positive dans son complément aurait une préimage vide.

Si $P'(t_0)=0$ pour un $t_0\in[0,1]$, prendre un intervalle $I_\delta\subset[0,1]$ de longueur $\delta$, adjacent à $t_0$. Alors


```math
|P(I_\delta)|\leq\delta\sup_{t\in I_\delta}|P'(t)|=o(\delta).
```


Mais $I_\delta\subset P^{-1}(P(I_\delta))$ et la conservation de longueur imposeraient $\delta\leq|P(I_\delta)|$, contradiction.

Ainsi $P'$ ne s'annule pas, donc $P$ est strictement monotone.
S'il est croissant, $P(0)=0$, $P(1)=1$ et


```math
P^{-1}([0,y])=[0,P^{-1}(y)],\qquad P^{-1}(y)=y.
```


Donc $P(X)=X$. S'il est décroissant,


```math
P^{-1}([0,y])=[P^{-1}(y),1],\qquad 1-P^{-1}(y)=y,
```


donc $P(X)=1-X$. Ces deux polynômes conviennent par changement de variable.

## 63

Posons $h(x)=3x^2-2x^3$. Pour $0<u<1$, l'équation $h(x)=u$ a trois racines


```math
a(u)\in(-1/2,0),\qquad b(u)\in(0,1),\qquad c(u)\in(1,3/2).
```


Elles sont dérivables, avec $a',c'<0$ et $b'>0$. Les relations entre racines donnent


```math
a(u)+b(u)+c(u)=\frac32,\qquad a'+b'+c'=0.
```


En changeant de variable sur les trois intervalles de monotonie,


```math
\int_{-1/2}^{3/2}f(h(x))\,dx
=\int_0^1f(u)\bigl(-a'(u)+b'(u)-c'(u)\bigr)\,du
=2\int_0^1f(u)b'(u)\,du.
```


La dernière intégrale vaut $\int_0^1f(h(x))\,dx$. Les changements de variable se font d'abord hors des extrémités, puis par passage à la limite ; $f$ est bornée et les trois branches parcourent des intervalles de longueur finie.
