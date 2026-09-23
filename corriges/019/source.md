# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td19-asymptotique.pdf)

## Autocorrection A



```math
\text{(i)}\quad u_n\sim\frac1{2n},\qquad\text{(ii)}\quad u_n\sim\frac1{3n},\qquad\text{(iii)}\quad u_n\sim-\frac1n.
```





```math
\text{(iv)}\quad(1+o(n^{-1}))(n^{-3}+o(n^{-10}))=n^{-3}+o(n^{-4}).
```





```math
\text{(v)}\quad u_n=o((\ln n)^{-1}),\qquad\text{(vi)}\quad u_n=o(n),\qquad\text{(vii)}\quad u_n=O(n).
```





```math
\text{(viii)}\quad u_n=(1+o(1))v_n\iff u_n\sim v_n.
```



## Autocorrection B



```math
\boxed{(v)\Longrightarrow(viii)\Longrightarrow[(i)\Longleftrightarrow(ii)\Longleftrightarrow(iv)\Longleftrightarrow(vii)]\Longrightarrow[(ix)\Longleftrightarrow(x)]\Longrightarrow(vi)\Longrightarrow(iii).}
```



Les réciproques des cinq flèches simples sont fausses, respectivement pour



```math
u_n=1+\frac1n,\qquad1+\frac1{\sqrt n},\qquad2,\qquad\sqrt n,\qquad n.
```



Les équivalences utilisent $e^{r_n}\to1\iff r_n\to0$ et $u_n-1=O(1)\iff u_n=O(1)$.

## Autocorrection C

$1\le v_n/u_n\le w_n/u_n\to1$, donc $v_n\sim u_n$.

## Autocorrection D



```math
u_n=n+1,\quad v_n=n:\qquad u_n\sim v_n,\qquad u_n-v_n=1\not\to0.
```





```math
u_n=\frac1n,\quad v_n=\frac1{n^2}:\qquad u_n-v_n\to0,\qquad\frac{u_n}{v_n}=n\not\to1.
```



Aucune implication.

## Exercice 1

À partir d'un rang, $u_n,v_n>0$. Posons $w_n=\sqrt{u_nv_n}$. Alors $u_n/w_n=\sqrt{u_n/v_n}\to0$ et $w_n/v_n=\sqrt{u_n/v_n}\to0$.

## Exercice 2

Prenons $u_n=n$ et $v_n=n$ si $n$ est pair, $v_n=n^2$ si $n$ est impair. Alors $u_n=O(v_n)$, mais $v_n\ne O(u_n)$ et $u_n\ne o(v_n)$.

## Exercice 3

Prendre $f(x)=e^{\sqrt{\max(x,0)}}$ sur $\mathbb R$. Pour $\alpha>0$,



```math
\ln\frac{x^\alpha}{f(x)}=\alpha\ln x-\sqrt x\to-\infty,\qquad\ln\frac{f(x)}{e^{\alpha x}}=\sqrt x-\alpha x\to-\infty.
```



## Exercice 4

Oui : $f(0)=0$, $f(x)=1/\ln(e/x)$ pour $0<x\le1$. Pour tout $\alpha>0$, $x^\alpha\ln(e/x)\to0$, donc $x^\alpha=o(f(x))$.

## Exercice 5

(i) Faux : $u_n=n$, $v_n=n+1$.
(ii) Vrai : $e^{u_n}/e^{v_n}\to1$ équivaut à $e^{u_n-v_n}\to1$, donc $u_n-v_n\to0$.
(iii) Faux : $u_n=1+1/n$, $v_n=1+2/n$.
(iv) Vrai : $u_n/v_n\to1$ et $u_n\to+\infty$ donnent $\ln u_n=\ln v_n+o(1)$, avec $\ln v_n\to+\infty$.

## Exercice 6

La notation $a_n\ll b_n$ signifie $a_n=o(b_n)$.

### (i)



```math
\boxed{\frac1{n^2}\ll\frac{\ln n}{n^2}\ll\frac1{n\ln n}\ll\frac1n\ll\frac{\ln n}{n}\ll\frac1{\ln n}.}
```



### (ii)



```math
\boxed{\sqrt n\ln n\ll\frac n{\ln n}\ll n\ll n\ln n\ll\frac{n^2}{\ln n}\ll n^2.}
```



Chaque quotient de deux termes consécutifs tend vers $0$, par $\ln^q n=o(n^\alpha)$ pour $q,\alpha>0$.

## Exercice 7

Pour $n\ge2$,



```math
0\le\sum_{k=0}^{n-1}k!\le(n-1)!+(n-1)(n-2)!=2(n-1)!.
```





```math
1\le\frac{\sum_{k=0}^nk!}{n!}\le1+\frac2n\longrightarrow1,\qquad\boxed{\sum_{k=0}^nk!\sim n!}.
```



## Exercice 8

La décroissance donne



```math
u_n+u_{n+1}\le2u_n\le u_{n-1}+u_n.
```



Les deux membres extrêmes sont équivalents à $1/n$, donc



```math
\boxed{u_n\sim\frac1{2n}.}
```



## Exercice 9

### 1



```math
2(\sqrt{n+1}-\sqrt n)=\frac2{\sqrt{n+1}+\sqrt n},\qquad2\sqrt n\le\sqrt{n+1}+\sqrt n\le2\sqrt{n+1}.
```



Inverser les inégalités donne l'encadrement demandé.

### 2

En sommant les deux bornes, avec décalage d'indice pour la seconde,



```math
2(\sqrt{n+1}-1)\le S_n\le1+2(\sqrt n-1).
```





```math
\boxed{S_n\to+\infty,\qquad S_n\sim2\sqrt n.}
```



## Exercice 10

Pour tout $m\in\mathbb N$,



```math
\frac{|f(x)|}{|x|^m}\le\frac{e^{-1/x^2}}{|x|^m}\longrightarrow0.
```



Donc $f$ est continue en $0$ et $f'(0)=\lim_{x\to0}f(x)/x=0$. Pour $x\ne0$,



```math
f'(x)=\frac2{x^3}\left[e^{-1/x^2}\cos(e^{1/x^2})+\sin(e^{1/x^2})\right].
```



Avec $x_k=(\ln(\pi/2+2k\pi))^{-1/2}\to0$,



```math
f'(x_k)=\frac2{x_k^3}\longrightarrow+\infty.
```



Ainsi $\boxed{f\in C^0(\mathbb R)\setminus C^1(\mathbb R)}$ ; elle est dérivable partout et $C^\infty$ sur $\mathbb R^*$. Elle n'est pas deux fois dérivable en $0$ puisque $f'(x_k)/x_k\to+\infty$.

## Autocorrection E

Les produits, quotients et compositions utilisent



```math
e^x=1+x+\frac{x^2}2+\frac{x^3}6+o(x^3),\qquad(1+x)^\alpha=1+\alpha x+\frac{\alpha(\alpha-1)}2x^2+\frac{\alpha(\alpha-1)(\alpha-2)}6x^3+o(x^3).
```



Pour (vi) et (x), développer d'abord l'exposant :



```math
\frac{\ln(1+x)}x=1-\frac x2+\frac{x^2}3+O(x^3),\qquad\frac{\ln(\cos x)}x=-\frac x2-\frac{x^3}{12}+o(x^3).
```



Pour (ix), $e^{-x}=1-x+x^2/2-x^3/6+O(x^4)$ et $(1+2x)^{-1}=1-2x+4x^2-8x^3+O(x^4)$. On obtient :

(i) $e^x\sqrt[3]{1+x}=1+\frac43x+\frac{13}{18}x^2+\frac{23}{81}x^3+o(x^3)$.
(ii) $\sin x\ln(1+x)=x^2-\frac12x^3+o(x^3)$.
(iii) $\sqrt{1+\sin x}=1+\frac x2-\frac{x^2}{8}-\frac{x^3}{48}+o(x^3)$.
(iv) $(e^x-1)\sin x=x^2+\frac{x^3}{2}+o(x^3)$.
(v) $x/(e^x-1)=1-x/2+x^2/12+o(x^2)$.
(vi) $e^{\cos x}-(1+x)^{1/x}=\frac e2x-\frac{23e}{24}x^2+o(x^2)$.
(vii) $(\sin x)^4=x^4-\frac23x^6+\frac15x^8+o(x^8)$.
(viii) $\tan x=x+x^3/3+2x^5/15+o(x^6)$.
(ix) $xe^{-x}/(2x+1)=x-3x^2+\frac{13}{2}x^3-\frac{79}{6}x^4+o(x^4)$.
(x) $(\cos x)^{1/x}=1-x/2+x^2/8-5x^3/48+o(x^3)$.
(xi) avec $h=x-2$, $x^4=16+32h+24h^2+8h^3+h^4+o(h^{100})$.
(xii) $\sqrt x=1+(x-1)/2-(x-1)^2/8+o((x-1)^2)$.
(xiii) $1/(1+x)=1/2-(x-1)/4+(x-1)^2/8+o((x-1)^2)$.
(xiv) $e^x=e+e(x-1)+e(x-1)^2/2+e(x-1)^3/6+o((x-1)^3)$.
(xv) avec $h=x-\pi/3$, $\sin x\cos3x=-\sqrt3/2-h/2+5\sqrt3h^2/2+o(h^2)$.
(xvi) avec $h=x-\pi/4$, $\sqrt{\tan x}=1+h+\frac12h^2+\frac56h^3+o(h^3)$.
(xvii) avec $h=x-1$, $x\ln x/(x^2-1)=1/2-h^2/12+h^3/12+o(h^3)$.

## Exercice 11

### 1

Écrire $\tan x=a_1x+a_3x^3+a_5x^5+a_7x^7+o(x^8)$ et multiplier par



```math
\cos x=1-\frac{x^2}2+\frac{x^4}{24}-\frac{x^6}{720}+O(x^8).
```



L'identification avec $\sin x=x-x^3/6+x^5/120-x^7/5040+o(x^8)$ donne



```math
a_1=1,\quad a_3-\frac12=-\frac16,\quad a_5-\frac{a_3}2+\frac1{24}=\frac1{120},
```





```math
a_7-\frac{a_5}2+\frac{a_3}{24}-\frac1{720}=-\frac1{5040}.
```





```math
\boxed{\tan x=x+\frac{x^3}3+\frac{2x^5}{15}+\frac{17x^7}{315}+o(x^8).}
```



### 2

Poser $P_0(T)=T$, $P_{k+1}(T)=(1+T^2)P_k'(T)$. Alors $\tan^{(k)}x=P_k(\tan x)$. Les valeurs en $0$ sont



```math
\tan'(0)=1,\quad\tan^{(3)}(0)=2,\quad\tan^{(5)}(0)=16,\quad\tan^{(7)}(0)=272,
```



et les dérivées paires sont nulles. Taylor-Young redonne le même développement. La relation $\tan'=1+\tan^2$ et l'imparité simplifient le calcul des dérivées.

### 3

Pour $T_n(x)=\sum_{k=0}^na_kx^k$, la relation différentielle donne



```math
a_0=0,\qquad a_{m+1}=\frac{\mathbf1_{m=0}+\sum_{k=0}^ma_ka_{m-k}}{m+1}\quad(0\le m<n).
```



Calculer successivement $a_1,\ldots,a_n$ avec cette formule, puis retourner $T_n$. Les coefficients pairs sont nuls ; les coefficients impairs commencent par $1,1/3,2/15,17/315,62/2835$.

## Exercice 12

### 1



```math
\frac{\ln(1+x)}x=1-\frac x2+\frac{x^2}3-\frac{x^3}4+o(x^3).
```



Appliquer $e^u=1+u+u^2/2+u^3/6+o(u^3)$ au terme après $1$ :



```math
\boxed{(1+x)^{1/x}=e\left(1-\frac x2+\frac{11x^2}{24}-\frac{7x^3}{16}+o(x^3)\right).}
```



### 2



```math
1+\sqrt{1+x}=2\left(1+\frac x4-\frac{x^2}{16}+\frac{x^3}{32}+o(x^3)\right).
```



Appliquer $(1+u)^{1/2}=1+u/2-u^2/8+u^3/16+o(u^3)$ :



```math
\boxed{\sqrt{1+\sqrt{1+x}}=\sqrt2\left(1+\frac x8-\frac{5x^2}{128}+\frac{21x^3}{1024}\right)+o(x^3).}
```



## Exercice 13



```math
u(x)=\frac{\sqrt3+x}{1+\sqrt3x},\qquad u'(x)=\frac{-2}{(1+\sqrt3x)^2}.
```





```math
f'(x)=\frac{u'(x)}{1+u(x)^2}=\frac{-2}{(1+\sqrt3x)^2+(\sqrt3+x)^2}=-\frac1{2(1+\sqrt3x+x^2)}.
```





```math
f'(x)=-\frac12+\frac{\sqrt3}{2}x-x^2+\frac{\sqrt3}{2}x^3+o(x^3).
```



Comme $f(0)=\pi/3$, l'intégration donne



```math
\boxed{f(x)=\frac\pi3-\frac x2+\frac{\sqrt3}{4}x^2-\frac{x^3}3+\frac{\sqrt3}{8}x^4+o(x^4).}
```



## Exercice 14

### 1(a)–(b)



```math
f'(x)=e^{x^2}(1+2x^2)>0,\qquad\lim_{x\to\pm\infty}f(x)=\pm\infty.
```



Ainsi $f$ est bijective. Puisque $f'$ ne s'annule pas, $g=f^{-1}$ est $C^\infty$. L'imparité de $f$ entraîne celle de $g$, donc



```math
g(x)=ax+bx^3+cx^5+o(x^5).
```



### 1(c)



```math
f(x)=x+x^3+\frac{x^5}2+o(x^5),
```





```math
g(f(x))=ax+(a+b)x^3+\left(\frac a2+3b+c\right)x^5+o(x^5)=x.
```





```math
a=1,\quad b=-1,\quad c=\frac52,\qquad\boxed{g(x)=x-x^3+\frac52x^5+o(x^5).}
```



### 2

Pour $h(x)=2x+\sin x$, $h'(x)=2+\cos x\ge1$ et ses limites sont $\pm\infty$. Son inverse est $C^\infty$ et impaire. Écrire $h^{-1}(x)=ax+bx^3+o(x^3)$, puis



```math
h^{-1}(h(x))=3ax+\left(-\frac a6+27b\right)x^3+o(x^3)=x.
```





```math
\boxed{h^{-1}(x)=\frac x3+\frac{x^3}{486}+o(x^3).}
```



## Exercice 15

Comme $\sum_{k=0}^{11}x^k/k!=e^x-x^{12}/12!+O(x^{13})$,


```math
\ln\left(\sum_{k=0}^{11}\frac{x^k}{k!}\right)=x-\frac{x^{12}}{12!}+o(x^{12}).
```



## Exercice 16

Non. $f(x)=1+x^2+|x|^{5/2}$ est paire et $f(x)=1+x^2+o(x^2)$, mais $|x|^{5/2}$ n'est pas $o(x^3)$.

## Exercice 17

Pour $x>0$, $\arctan x=\pi/2-\arctan(1/x)$. En intégrant le développement géométrique de $(1+t^2)^{-1}$,



```math
\boxed{\arctan x=\frac\pi2+\sum_{\substack{k\ge0\\2k+1\le n}}\frac{(-1)^{k+1}}{(2k+1)x^{2k+1}}+o(x^{-n}).}
```



Pour $n=0$, la somme est vide. Tous les termes d'ordre $x^{-n}$ sont conservés lorsqu'ils existent.

## Exercice 18

### 1



```math
a\sin x+b\cos x=b+ax-\frac b2x^2-\frac a6x^3+O(x^4).
```



L'égalité à $x+O(x^5)$ impose $b=0$, $a=1$, puis $-a/6=0$, contradiction.

### 2



```math
\frac{x+ax^3}{1+bx^2}=x+(a-b)x^3+b(b-a)x^5+b^2(a-b)x^7+O(x^9).
```





```math
f_{a,b}(x)=\left(b-a-\frac16\right)x^3+\left(\frac1{120}+b(a-b)\right)x^5+\left(-\frac1{5040}+b^2(b-a)\right)x^7+O(x^9).
```



Le coefficient cubique s'annule si et seulement si $a=b-1/6$. Sous cette condition, le coefficient d'ordre $5$ vaut $1/120-b/6$ ; il s'annule si et seulement si $b=1/20$. Ainsi



```math
\boxed{a=-\frac7{60},\qquad b=\frac1{20}},\qquad f_{-7/60,1/20}(x)=\frac{11}{50400}x^7+O(x^9).
```



Toute autre fonction de la famille a un premier terme non nul de degré $3$ ou $5$ : la fonction trouvée est négligeable devant elle.

### 3



```math
\frac1{\ln(1+x)}=\frac1x+\frac12-\frac x{12}+\frac{x^2}{24}+O(x^3),\qquad\frac1{e^x-1}=\frac1x-\frac12+\frac x{12}+O(x^3).
```





```math
\frac1x+\frac a{\ln(1+x)}+\frac b{e^x-1}=\frac{1+a+b}{x}+\frac{a-b}{2}+\frac{b-a}{12}x+\frac a{24}x^2+O(x^3).
```



Annuler les deux premiers termes impose $a=b=-1/2$, ce qui annule aussi le coefficient de $x$. Le résultat est alors $-x^2/48+O(x^3)$. Aucun équivalent $Cx$, avec $C\ne0$, n'est possible ; un équivalent à la fonction nulle n'est pas défini.

## Exercice 19

Pour tout $\varepsilon>0$, $|u_k|\le\varepsilon/k$ dès que $k$ est assez grand. Ainsi


```math
\left|\sum_{k=n+1}^{2n}u_k\right|\le\varepsilon\sum_{k=n+1}^{2n}\frac1k\le\varepsilon,
```


et la somme tend vers $0$.

## Exercice 20

Uniformément pour $1\le k\le n$, $\sin(k/n^2)=k/n^2+O(k^3/n^6)$. Donc la somme vaut $(n+1)/(2n)+O(n^{-2})=1/2+1/(2n)+o(1/n)$.

## Autocorrection F

### (i)



```math
\ln(1+x)-\sin x=-\frac{x^2}2+O(x^3),\qquad\tan x-x=\frac{x^3}3+O(x^5).
```



Le quotient est équivalent à $-3/(2x)$ : limite $-\infty$ en $0^+$, $+\infty$ en $0^-$.

### (ii)



```math
\ln(2x^2-1)=4(x-1)+o(x-1),\qquad\tan(x-1)\sim x-1.
```



Limite : $\boxed4$.

### (iii)



```math
\frac1{\sin^3x}=\frac1{x^3}\left(1+\frac{x^2}2+O(x^4)\right),\qquad\frac1{x^3}-\frac1{\sin^3x}\sim-\frac1{2x}.
```



Limites : $-\infty$ en $0^+$ et $+\infty$ en $0^-$.

### (iv)



```math
x-\arctan x\sim\frac{x^3}3,\qquad\sin^3x\sim x^3\implies\boxed{\lim=\frac13}.
```



### (v)



```math
\ln|x|\ln(\cos x)=-\frac{x^2\ln|x|}{2}+O(x^4\ln|x|)\longrightarrow0.
```





```math
\boxed{(\cos x)^{\ln|x|}\longrightarrow1.}
```



### (vi)



```math
x^3+7x^2-8=17(x-1)+O((x-1)^2),\quad x^4+x^3-2=7(x-1)+O((x-1)^2).
```



Limite : $\boxed{17/7}$.

## Autocorrection G

### (i)–(vi)



```math
\text{(i)}\quad x-1<\lfloor x\rfloor\le x\implies\boxed{\lfloor x\rfloor\sim x}.
```





```math
\text{(ii)}\quad\boxed{-\frac2x\text{ en }0,\qquad\frac x2\text{ en }+\infty}.
```





```math
\text{(iii)}\quad\ln(1+x^2)-\sin(x^2)+2\cos^2x=2\ln x+O(1)\sim\boxed{2\ln x}.
```





```math
\text{(iv)}\quad\frac{\ln x}{\sqrt{x-1}}\sim\boxed{\sqrt{x-1}}\qquad(x\to1^+).
```





```math
\text{(v)}\quad\frac1x-\frac1{1+x}+\frac1{2+x}=\frac1x-\frac1{(1+x)(2+x)}\sim\boxed{\frac1x}
```



en $0$ et en $+\infty$.



```math
\text{(vi)}\quad e^x\to0,\quad e^{e^x}\to1,\quad e^{e^{e^x}}\to e,\qquad\boxed{1+e^{e^{e^x}}-\arctan x\sim1+e+\frac\pi2}\quad(x\to-\infty).
```



### (vii)–(xii)



```math
\text{(vii)}\quad\sqrt{\sqrt{x+2}-\sqrt{x+1}}=\frac1{\sqrt{\sqrt{x+2}+\sqrt{x+1}}}\sim\boxed{\frac1{\sqrt2\,x^{1/4}}}.
```





```math
\text{(viii)}\quad\frac{\sin x}{\sqrt x}\sim\boxed{-\frac{x-\pi}{\sqrt\pi}}.
```





```math
\text{(ix)}\quad\frac{(\sqrt x)^3+2}{(\sqrt[3]x)^2+3}\sim\frac{x^{3/2}}{x^{2/3}}=\boxed{x^{5/6}}.
```





```math
\text{(x)}\quad\sqrt{x^2+1}-\sqrt{x^2-1}=\frac2{\sqrt{x^2+1}+\sqrt{x^2-1}}\sim\boxed{\frac1x}.
```





```math
\text{(xi)}\quad\frac{\ln(x+1)}{\ln x}-1=\frac{\ln(1+1/x)}{\ln x}\sim\boxed{\frac1{x\ln x}}.
```





```math
\text{(xii)}\quad\sqrt{\ln(x+1)}-\sqrt{\ln(x-1)}=\frac{\ln((x+1)/(x-1))}{\sqrt{\ln(x+1)}+\sqrt{\ln(x-1)}}\sim\boxed{\frac1{x\sqrt{\ln x}}}.
```



### (xiii)–(xviii)



```math
\text{(xiii)}\quad x\ln(x+1)-(x+1)\ln x=x\ln(1+1/x)-\ln x\sim\boxed{-\ln x}.
```





```math
\text{(xiv)}\quad\sqrt{1+x^2}-\sqrt{1-x^2}=\frac{2x^2}{\sqrt{1+x^2}+\sqrt{1-x^2}}\sim\boxed{x^2}.
```





```math
\text{(xv)}\quad\tan x-\sin x=\frac{x^3}2+o(x^3)\sim\boxed{\frac{x^3}2}.
```





```math
\text{(xvi)}\quad\ln(1+\sin x)\sim\sin x\sim\boxed x.
```





```math
\text{(xvii)}\quad\ln(\ln(1+x))=\ln x+\ln\frac{\ln(1+x)}x=\ln x+o(1)\sim\boxed{\ln x}\quad(x\to0^+).
```





```math
\text{(xviii)}\quad t=\frac\pi2-x\to0^+,\qquad\ln(\cos x)=\ln(\sin t)=\ln t+o(1)\sim\boxed{\ln\left(\frac\pi2-x\right)}.
```



## Autocorrection H



```math
\begin{array}{c|c}
(i)&3n/2\\
(ii)&1/(3n)\\
(iii)&1/n^2\\
(iv)&1/n\\
(v)&\pi/n^2\\
(vi)&n^2/\pi\\
(vii)&1/n\\
(viii)&2ne^{-(n+1)}\\
(ix)&2\ln n/n\\
(x)&n^{1/3}\\
(xi)&-n/2\\
(xii)&n!/3^n\\
(xiii)&-2/n^2\\
(xiv)&1/\sqrt n\\
(xv)&-\ln n
\end{array}
```



Pour (iii)–(vii), utiliser $\ln(1+t)\sim t$, $\sin t\sim t$, $\tan t\sim t$ et



```math
\ln(n+2)-\ln(n+1)=\ln\left(1+\frac1{n+1}\right).
```



Pour (xii), $n!\ge\lfloor n/2\rfloor^{\lfloor n/2\rfloor}$ donne $e^n=o(n!)$, tandis que $2^n=o(3^n)$.



```math
\text{(xiii)}\quad\frac1{n+1}-\frac1{n-1}=-\frac2{n^2-1},\qquad
\text{(xiv)}\quad\sqrt{n+1}-\sqrt{n-1}=\frac2{\sqrt{n+1}+\sqrt{n-1}}.
```



Pour (xv), $\sqrt{\ln(n+1)}=o(\ln n)$ et $\ln(n-1)\sim\ln n$.

## Exercice 21

### 1

Pour $x\to0^+$, poser $A=\sin x\ln x$ et $B=x\ln(\sin x)$. Alors $A,B\to0$, et



```math
A-B=(\sin x-x)\ln x-x\ln\frac{\sin x}{x}=-\frac{x^3\ln x}{6}+\frac{x^3}6+o(x^3).
```





```math
e^A-e^B=e^B(e^{A-B}-1)\sim A-B\sim\boxed{-\frac{x^3\ln x}{6}}.
```



### 2

Composer les développements de $\sin$ et $\sinh$ à l'ordre $7$ donne



```math
\sinh(\sin x)=x-\frac{x^5}{15}+\frac{x^7}{90}+o(x^7),
```





```math
\sin(\sinh x)=x-\frac{x^5}{15}-\frac{x^7}{90}+o(x^7).
```





```math
\boxed{\sinh(\sin x)-\sin(\sinh x)\sim\frac{x^7}{45}.}
```



## Exercice 22

L'imparité et Taylor-Young donnent



```math
f(x)=x+ax^3+bx^5+o(x^6),\qquad g(x)=x+Ax^3+Bx^5+o(x^6).
```





```math
f(g(x))=x+(a+A)x^3+(b+B+3aA)x^5+o(x^6),
```





```math
g(f(x))=x+(A+a)x^3+(B+b+3Aa)x^5+o(x^6).
```



Ainsi $f\circ g-g\circ f=o(x^6)$ et la limite vaut $\boxed0$.

## Exercice 23



```math
\frac{m(m-1)}2<n\le\frac{m(m+1)}2\iff u_n=m.
```





```math
\boxed{u_n=\left\lceil\frac{\sqrt{8n+1}-1}{2}\right\rceil}.
```



Puisque la différence entre un réel et son plafond appartient à $[0,1[$,



```math
u_n=\sqrt{2n}+O(1)\sim\boxed{\sqrt{2n}}.
```



## Exercice 24

Pour $n\ge1$, la définition imprimée est $u_n=n^n\sqrt n/(e^nn!)$.

### 1



```math
v_n=\left(n+\frac12\right)\ln\left(1+\frac1n\right)-1.
```





```math
\ln\left(1+\frac1n\right)=\frac1n-\frac1{2n^2}+\frac1{3n^3}-\frac1{4n^4}+O(n^{-5}),
```





```math
\boxed{v_n=\frac1{12n^2}-\frac1{12n^3}+O(n^{-4})\sim\frac1{12n^2}.}
```



### 2

Ainsi $v_n>0$ pour $n$ assez grand et $|v_n|\le C/n^2$. La série $\sum v_n$ converge absolument, donc



```math
\ln u_n=\ln u_1+\sum_{k=1}^{n-1}v_k\longrightarrow L\in\mathbb R,\qquad u_n\longrightarrow\lambda=e^L>0.
```



Comme $\ln u_{n+1}-\ln u_n=v_n>0$ finalement, $u$ est finalement croissante.



```math
\boxed{n!=\frac1{u_n}\sqrt n\left(\frac ne\right)^n\sim\frac1\lambda\sqrt n\left(\frac ne\right)^n.}
```



La remarque imprimée inverse la constante : avec cette définition de $u_n$, la constante de Stirling est $\lambda^{-1}=\sqrt{2\pi}$.

## Exercice 25

### 1



```math
\boxed{P(X)=X^3-(a+b+c)X^2+(ab+ac+bc)X-abc.}
```



### 2

Pour $n\ge5$, poser $d_n=(2n+1)/3>3$. Alors



```math
P_n(0)=-1<0,\quad P_n(1)=n-1>0,\quad P_n(3)=11-3n<0,
```





```math
P_n(d_n)=-\frac{(n-1)(4n^2-8n-23)}{27}<0,\qquad\lim_{x\to+\infty}P_n(x)=+\infty.
```



Le théorème des valeurs intermédiaires donne une racine dans chacun des intervalles $(0,1)$, $(1,3)$ et $(d_n,+\infty)$. Le degré étant $3$, ce sont les trois racines, distinctes :



```math
0<a_n<1<b_n<3<d_n<c_n.
```



### 3

L'équation $P_n(a_n)=0$ s'écrit



```math
na_n(2-a_n)=1-a_n(a_n-1)^2.
```



Comme $0<a_n<1$, elle entraîne $na_n\le1$, donc $a_n\to0$. Le membre droit tend vers $1$ ; ainsi



```math
\boxed{a_n\sim\frac1{2n}.}
```



De même,



```math
nb_n(2-b_n)=1-b_n(b_n-1)^2=O(1).
```



Puisque $1<b_n<3$, on obtient $2-b_n=O(1/n)$, donc $\boxed{b_n\sim2}$. Enfin



```math
c_n=n+2-a_n-b_n=n+O(1)\sim\boxed n.
```



## Exercice 26

1. $f_n'(x)=5x^4+n>0$, $f_n(0)=-1$, $f_n(1/n)=n^{-5}>0$ : racine unique $u_n\in(0,1/n)$.
2. $nu_n=1-u_n^5\to1$, donc $u_n\sim1/n$.
3. $1/n-u_n=u_n^5/n$ par l'équation, donc $1/n-u_n\sim n^{-6}$.

## Exercice 27

### 1



```math
h(x)=x+\ln x,\quad h'(x)=1+\frac1x>0,\quad h(0^+)=-\infty,\quad h(+\infty)=+\infty.
```



Ainsi $h(u_n)=n$ a une unique solution positive.

### 2

$h(1)=1$ donne $u_n\ge1$, puis $u_n=n-\ln u_n\le n$. Donc



```math
n-\ln n\le u_n\le n\implies\boxed{u_n\sim n}.
```



### 3



```math
u_n=n-\ln u_n=n-\ln n-\ln\frac{u_n}{n}=\boxed{n-\ln n+o(1)}.
```



## Exercice 28

### 1

Si $0<u_n<1/3$, alors $0<u_{n+1}=u_n(1-3u_n)<u_n<1/3$. Par récurrence, $u$ est positive et décroissante. Sa limite satisfait $\ell=\ell-3\ell^2$, donc $\ell=0$.

### 2(a)

Pour $\lambda\alpha\ne0$,



```math
v_{n+1}-v_n=\lambda n^\alpha\left[\left(1+\frac1n\right)^\alpha-1\right]\sim\lambda\alpha n^{\alpha-1},\qquad-3v_n^2=-3\lambda^2n^{2\alpha}.
```



Si $\lambda=0$ ou $\alpha=0$, la première différence est identiquement nulle.

### 2(b)–(c)

Les solutions non nulles de $y'+3y^2=0$ vérifient



```math
\left(\frac1y\right)'=3\implies y(t)=\frac1{3t+C}.
```



La solution nulle convient aussi. L'équilibrage $\alpha-1=2\alpha$, $\lambda\alpha=-3\lambda^2$ donne $\alpha=-1$, $\lambda=1/3$ : conjecture $u_n\sim1/(3n)$.

### 3(a)–(b)

Avec $dt/t$, comme imprimé, l'intégrale vaut $-\ln(1-3u_n)\to0$ ; la limite $3$ exige $dt/t^2$.



```math
\int_{u_{n+1}}^{u_n}\frac{dt}{t^2}=\frac1{u_{n+1}}-\frac1{u_n}=\frac3{1-3u_n}\longrightarrow3.
```



Par Cesàro,



```math
\frac1n\int_{u_n}^{u_0}\frac{dt}{t^2}=\frac1n\sum_{k=0}^{n-1}\frac3{1-3u_k}\longrightarrow3.
```





```math
\frac1{u_n}-\frac1{u_0}\sim3n\implies\boxed{u_n\sim\frac1{3n}.}
```



### 4(a)–(b)



```math
w_n=\frac1{3u_n}\to+\infty,\qquad w_{n+1}-w_n=\frac1{1-1/w_n}\longrightarrow1.
```



Cesàro donne $w_n\sim n$. Ensuite



```math
[w_{n+1}-(n+1)]-[w_n-n]=\frac1{w_n-1}\sim\frac1n.
```



### 4(c)–(d)

Pour tout $\varepsilon>0$ et $n\ge N$ assez grand,



```math
\frac{1-\varepsilon}{n}\le\frac1{w_n-1}\le\frac{1+\varepsilon}{n}.
```



Sommer de $N$ à $n-1$, puis utiliser $\sum_{k=N}^{n-1}1/k\sim\ln n$ : $w_n-n\sim\ln n$. Donc



```math
u_n=\frac1{3n}\left(1+\frac{\ln n}{n}+o\left(\frac{\ln n}{n}\right)\right)^{-1},
```





```math
\boxed{u_n=\frac1{3n}-\frac{\ln n}{3n^2}+o\left(\frac{\ln n}{n^2}\right).}
```



## Exercice 29

### 1

Pour $t>0$, $0<\arctan t<t$. Donc $u_n>0$, $u$ décroît et converge. Sa limite vérifie $\ell=\arctan\ell$, donc $\ell=0$.

### 2



```math
u_{n+1}=u_n-\frac{u_n^3}3+o(u_n^3),\qquad u_{n+1}-u_n\sim-\frac{u_n^3}3.
```





```math
\frac1{u_{n+1}^2}-\frac1{u_n^2}=\frac1{u_n^2}\left[\left(1-\frac{u_n^2}3+o(u_n^2)\right)^{-2}-1\right]\longrightarrow\frac23.
```



Par Cesàro, $1/u_n^2\sim2n/3$, donc



```math
\boxed{u_n\sim\sqrt{\frac3{2n}}.}
```



## Exercice 30

$u_n>0$ et $u_{n+1}>u_n$. Une limite finie $\ell>0$ imposerait $\ell=\ell+1/\ell$, impossible. Ainsi $u_n\to+\infty$ et



```math
u_{n+1}^2-u_n^2=2+\frac1{u_n^2}\longrightarrow2.
```



Cesàro donne $u_n^2/n\to2$, donc $\boxed{u_n\sim\sqrt{2n}}$.

## Exercice 31

$x_n>1$ et $x$ croît. Une limite finie $\ell>1$ contredirait $x_{n+1}-x_n=1/\ln x_n$ ; donc $x_n\to+\infty$.



```math
\frac{x_{n+1}}{x_n}=1+\frac1{x_n\ln x_n}\longrightarrow1,\qquad\frac{\ln x_{n+1}}{\ln x_n}\longrightarrow1.
```



Par monotonie de $\ln$,



```math
1=(x_{n+1}-x_n)\ln x_n\le\int_{x_n}^{x_{n+1}}\ln t\,dt\le\frac{\ln x_{n+1}}{\ln x_n}\longrightarrow1.
```



Cesàro donne



```math
\int_{x_0}^{x_n}\ln t\,dt=x_n\ln x_n-x_n+O(1)\sim n.
```



Ainsi $x_n\ln x_n\sim n$. En prenant les logarithmes,



```math
\ln x_n+\ln\ln x_n=\ln n+o(1)\implies\ln x_n\sim\ln n.
```





```math
\boxed{x_n\sim\frac n{\ln n}.}
```



## Exercice 32

$x$ est strictement croissante. Une limite finie $\ell$ imposerait $0=e^{-\ell}$, donc $x_n\to+\infty$. Poser $y_n=e^{x_n}\to+\infty$ :



```math
y_{n+1}-y_n=y_n(e^{1/y_n}-1)=1+\frac1{2y_n}+O(y_n^{-2})\longrightarrow1.
```



Cesàro donne $y_n\sim n$. Ainsi $y_{n+1}-y_n=1+O(1/n)$ et, par sommation, $y_n=n+O(\ln n)$. En réinjectant,



```math
\frac1{y_n}=\frac1n+O\left(\frac{\ln n}{n^2}\right),
```





```math
y_{n+1}-y_n=1+\frac1{2n}+O\left(\frac{\ln n}{n^2}\right).
```



La série des derniers termes converge absolument, donc $y_n=n+\frac12\ln n+O(1)$. Finalement,



```math
\boxed{x_n=\ln n+\frac{\ln n}{2n}+O\left(\frac1n\right)=\ln n+\frac{\ln n}{2n}+o\left(\frac{\ln n}{n}\right).}
```



## Exercice 33

1. La récurrence est $u_{n+1}=\sqrt{u_n+n^2}$. Par récurrence, $u_n=O(n)$ : si $u_n\le2n$, alors $u_{n+1}\le\sqrt{n^2+2n}\le n+1$. Ainsi $u_{n+1}=n+O(1)$.
2. $u_{n+1}=n+u_n/(2n)+O(1/n)=n+1/2+o(1)$, car $u_n=n+O(1)$. Donc $u_n=n-1/2+o(1)$.
3. Le développement $u_{n+1}=n+u_n/(2n)-u_n^2/(8n^3)+O(n^{-2})$, avec $u_n=n-1/2+o(1)$, donne $u_{n+1}=n+1/2-3/(8n)+o(1/n)$, donc $u_n=n-1/2-3/(8n)+o(1/n)$.

## Exercice 34

### 1



```math
e^x-e^{-x}=2x\left(1+\frac{x^2}6+O(x^4)\right),
```





```math
\boxed{f(x)=\frac x2\left(1-\frac{x^2}6+O(x^4)\right)=\frac x2-\frac{x^3}{12}+o(x^3).}
```



### 2

Le quotient est lisse hors de $0$ ; le développement donne $f(x)\to0=f(0)$ et $f(x)/x\to1/2$. Ainsi $f$ est dérivable sur $\mathbb R$, avec $\boxed{f'(0)=1/2}$.

### 3



```math
f(x)-\frac x2\sim-\frac{x^3}{12}.
```



Au voisinage de $0$, la courbe est au-dessus de sa tangente $y=x/2$ pour $x<0$, et au-dessous pour $x>0$.

## Exercice 35

### 1

Pour $x>0$,



```math
f(x)=\exp\left(\left(1+\frac1x\right)\ln x\right)\longrightarrow0=f(0),
```





```math
\frac{f(x)-f(0)}x=x^{1/x}\longrightarrow0.
```



Donc $f$ est continue et dérivable à droite en $0$, avec $f'(0)=0$. Sur $\mathbb R_+^*$,



```math
f'(x)=f(x)\left(\frac1x+\frac{1-\ln x}{x^2}\right)=x^{1/x}\left(1+\frac{1-\ln x}{x}\right).
```



Comme $(\ln x)/x$ tend vers $-\infty$ plus vite que toute constante multiple de $|\ln x|$, l'exponentielle $x^{1/x}$ domine les facteurs polynomiaux en $1/x$ et $|\ln x|$. Ainsi $f'(x)\to0$ ; en particulier $f\in C^1(\mathbb R_+)$.

### 2

Poser $h=x-1$. Alors



```math
\ln f(1+h)=\left(1+\frac1{1+h}\right)\ln(1+h)=2h-2h^2+\frac{13}6h^3+o(h^3).
```



En exponentiant,



```math
\boxed{f(1+h)=1+2h-\frac12h^3+o(h^3).}
```



La tangente en $1$ est $y=2x-1$. La différence vaut $-(x-1)^3/2+o((x-1)^3)$ : courbe au-dessus à gauche, au-dessous à droite, près de $1$.

## Exercice 36



```math
\arcsin x=x\left(1+\frac{x^2}6+\frac{3x^4}{40}+o(x^4)\right),
```





```math
\frac1{\arcsin x}=\frac1x\left(1-\frac{x^2}6-\frac{17x^4}{360}+o(x^4)\right).
```





```math
\boxed{f(x)=\frac x6+\frac{17x^3}{360}+o(x^3).}
```



Le prolongement continu vaut $f(0)=0$ ; il est dérivable en $0$, avec $f'(0)=1/6$. Sa tangente est $y=x/6$. Comme $f(x)-x/6\sim17x^3/360$, la courbe est au-dessus pour $x>0$, au-dessous pour $x<0$, près de $0$.

## Exercice 37

En $+\infty$,



```math
e^{1/x}=1+\frac1x+\frac1{2x^2}+\frac1{6x^3}+o(x^{-3}),
```





```math
f(x)=x+2+\frac3{2x}+O(x^{-2}).
```



Asymptote : $\boxed{y=x+2}$. Pour tout $x>0$,



```math
e^{1/x}>1+\frac1x\implies f(x)>(x+1)\left(1+\frac1x\right)=x+2+\frac1x>x+2.
```



La courbe est au-dessus. En $0^+$, $f(x)\to+\infty$ : asymptote verticale $\boxed{x=0}$, avec la courbe dans le demi-plan $x>0$.

## Exercice 38

1. $u_n=(1+1/n)^n\to e$.
2. $\ln(u_{n+1}/u_n)=(n+1)\ln(1+1/(n+1))-n\ln(1+1/n)=1/(2n^2)+o(1/n^2)>0$ finalement.

## Exercice 39

### 1

Pour $|x|\to\infty$,



```math
\sqrt{x^4+x^3+1}=x^2\sqrt{1+\frac1x+\frac1{x^4}}.
```



Appliquer $\sqrt{1+t}=1+t/2-t^2/8+t^3/16+O(t^4)$ :



```math
\boxed{\sqrt{x^4+x^3+1}=x^2+\frac x2-\frac18+\frac1{16x}+O(x^{-2}).}
```



### 2

Le même développement vaut en $+\infty$ et en $-\infty$. Pour $x\in\mathbb Z$,



```math
\operatorname{dist}\left(x^2+\frac x2-\frac18,\mathbb Z\right)=\begin{cases}1/8,&x\text{ pair},\\3/8,&x\text{ impair}.
\end{cases}
```



Or



```math
\sqrt{x^4+x^3+1}-\left(x^2+\frac x2-\frac18\right)\longrightarrow0\qquad(|x|\to\infty).
```



Pour $|x|$ assez grand, cette différence a une valeur absolue inférieure à $1/16$, donc la racine carrée n'est pas entière. Les solutions entières ont donc $x$ borné ; pour chaque $x$, il y a au plus deux valeurs de $y$. Ainsi $\boxed{E\text{ est fini}}$.

## Exercice 40

$\sin^n x=x^n+O(x^{n+2})$; ainsi $f^{(k)}(0)=0$ pour $0\le k<n$ et $f^{(n)}(0)=n!$.

## Exercice 41

### 1



```math
f(x)=\frac{e^{(n+1)x}-1}{e^x-1}=\sum_{k=0}^ne^{kx}\qquad(x\ne0).
```



Le prolongement continu vaut $\boxed{f(0)=n+1}$.

### 2

Poser $N=n+1$. Alors



```math
\frac{e^{Nx}-1}{x}=N+\frac{N^2}2x+\frac{N^3}6x^2+\frac{N^4}{24}x^3+o(x^3),
```





```math
\frac{x}{e^x-1}=1-\frac x2+\frac{x^2}{12}+o(x^3).
```



Le produit donne



```math
\boxed{f(x)=n+1+\frac{n(n+1)}2x+\frac{n(n+1)(2n+1)}{12}x^2+\frac{n^2(n+1)^2}{24}x^3+o(x^3).}
```



### 3

La somme de la question1 donne également



```math
f(x)=\sum_{k=0}^n\left(1+kx+\frac{k^2x^2}2+\frac{k^3x^3}6\right)+o(x^3).
```



Identifier les coefficients cubiques :



```math
\frac16\sum_{k=1}^nk^3=\frac{n^2(n+1)^2}{24}\implies\boxed{\sum_{k=1}^nk^3=\left(\frac{n(n+1)}2\right)^2.}
```



## Exercice 42

D'une part,



```math
(e^x-1)^n=(x+O(x^2))^n=x^n+o(x^n).
```



D'autre part, par le binôme et Taylor,



```math
(e^x-1)^n=\sum_{k=0}^n(-1)^{n-k}\binom nk e^{kx}=\sum_{p=0}^n\frac{x^p}{p!}\left(\sum_{k=0}^n(-1)^{n-k}\binom nk k^p\right)+o(x^n).
```



L'unicité des coefficients du développement limité donne



```math
\boxed{\sum_{k=0}^n(-1)^{n-k}\binom nk k^p=\begin{cases}0,&0\le p<n,\\n!,&p=n.\end{cases}}
```



Pour $p=0$, le terme $k^0$ vaut $1$, y compris pour $k=0$, conformément au terme constant de $e^{kx}$.
