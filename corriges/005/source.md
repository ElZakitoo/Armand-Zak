# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td05-complexes.pdf)

## Autocorrection A

Pour $b\ne0$, $a/b=a\overline b/|b|^2$ et $|a/b|=|a|/|b|$.



```math
\begin{array}{c|c|c}&\text{forme algébrique}&\text{module}\\\hline
(i)&-i&1\\
(ii)&i&1\\
(iii)&(-1+i)/2&1/\sqrt2\\
(iv)&-11/5+19i/10&13\sqrt5/10\\
(v)&i&1\\
(vi)&(-8+6i)/25&2/5\\
(vii)&-3&3\\
(viii)&(1+i\sqrt3)/2&1\\
(ix)&-16+24i&8\sqrt{13}
\end{array}
```



Pour (iv), $(2+3i)^2=-5+12i$ et $(-5+12i)(4+2i)/20=(-44+38i)/20$.

Pour (vi), $(1+i)/(2-i)=(1+3i)/5$, puis $(1+3i)^2=-8+6i$.

Pour (ix), $(5-i)^2=24-10i=-2i(3+2i)^2$, donc



```math
\frac{(5-i)^6}{(3+2i)^5}=(-2i)^3(3+2i)=8i(3+2i)=-16+24i.
```



## Autocorrection B

Poser $z=x+iy$, $x,y\in\mathbb R$.

### (i)



```math
3z-(3-i)\overline z=y+i(x+6y)=1-2i\iff y=1,\ x=-8.
```





```math
\boxed{z=-8+i}.
```



### (ii)



```math
2z+6\overline z=8x-4iy=3+2i\iff x=3/8,\ y=-1/2.
```





```math
\boxed{z=3/8-i/2}.
```



### (iii)



```math
(3+4i)z-5\overline z=(-2x-4y)+i(4x+8y).
```



L'égalité à $2i$ imposerait à la fois $x+2y=0$ et $x+2y=1/2$. Il n'y a aucune solution.

## Exercice 1



```math
i^n=\begin{cases}1,&n\equiv0\pmod4,\\i,&n\equiv1\pmod4,\\-1,&n\equiv2\pmod4,\\-i,&n\equiv3\pmod4.\end{cases}
```





```math
\sum_{k=0}^ni^k=\frac{1-i^{n+1}}{1-i}=\begin{cases}1,&n\equiv0\pmod4,\\1+i,&n\equiv1\pmod4,\\i,&n\equiv2\pmod4,\\0,&n\equiv3\pmod4.\end{cases}
```





```math
\boxed{\prod_{k=1}^ni^k=i^{n(n+1)/2}}.
```



Pour $n=0$, le produit vide vaut $1$.

## Exercice 2

Pour $z=x+iy$,



```math
(z-2)(\overline z+i)=(x-2+iy)(x+i(1-y)),\qquad\operatorname{Im}\bigl((z-2)(\overline z+i)\bigr)=x+2y-2.
```





```math
\boxed{\{z:(z-2)(\overline z+i)\in\mathbb R\}=\{x+iy:x+2y=2\}}.
```



## Exercice 3

Si $\overline z=az+b$ pour tout $z$, les valeurs $z=0$ et $z=1$ imposent $b=0$ et $a=1$. La valeur $z=i$ donnerait alors $-i=i$, contradiction. L'assertion est fausse.

## Exercice 4

Si $\operatorname{Im}\alpha\ne0$, l'égalité $x+\alpha y=0$ donne $y\operatorname{Im}\alpha=0$, donc $y=0$, puis $x=0$.

Si $\alpha\in\mathbb R$, le couple $(x,y)=(-\alpha,1)$ est non nul et vérifie l'égalité. Ainsi la condition est $\boxed{\alpha\notin\mathbb R}$.

## Exercice 5

### 1

Les carrés entiers sont congrus à $0$ ou $1$ modulo $4$ ; leur somme n'est jamais congrue à $3$. Donc $3\notin S$.

### 2



```math
a^2+b^2=|a+ib|^2,\qquad(a^2+b^2)(c^2+d^2)=|(a+ib)(c+id)|^2.
```





```math
\boxed{(a^2+b^2)(c^2+d^2)=(ac-bd)^2+(ad+bc)^2\in S}.
```



### 3

Modulo $8$, un carré vaut $0,1$ ou $4$. Une somme de trois tels résidus ne vaut jamais $7$ : avec zéro, un, deux ou trois résidus $4$, les sommes possibles sont respectivement $0,1,2,3$ ; $4,5,6$ ; $0,1$ ; $4$. Donc $15\notin S'$.

Mais $3=1^2+1^2+1^2$ et $5=2^2+1^2+0^2$ appartiennent à $S'$, alors que $3\cdot5=15\notin S'$. L'ensemble $S'$ n'est pas stable par produit.

## Exercice 6

Avec $j^2+j+1=0$,



```math
|a+bj|^2=a^2-ab+b^2,
```





```math
(a+bj)(c+dj)=(ac-bd)+(ad+bc-bd)j.
```



La multiplicativité du module donne



```math
(a^2-ab+b^2)(c^2-cd+d^2)=A^2-AB+B^2,
```



où $A=ac-bd\in\mathbb Z$ et $B=ad+bc-bd\in\mathbb Z$. L'ensemble est stable par produit.

## Autocorrection C

Pour $(x+iy)^2=a+ib$, les conditions sont $x^2-y^2=a$, $2xy=b$, $x^2+y^2=\sqrt{a^2+b^2}$.



```math
\begin{array}{c|c}
(i)&\displaystyle\pm\frac{1+i}{\sqrt2}\\
(ii)&\pm(2-i)\\
(iii)&\pm(3-i)\\
(iv)&\pm(5-i)\\
(v)&\displaystyle\pm\left(\sqrt{\frac{\sqrt5+1}{2}}+i\sqrt{\frac{\sqrt5-1}{2}}\right)
\end{array}
```



Les carrés des expressions proposées redonnent respectivement $i$, $3-4i$, $8-6i$, $24-10i$ et $1+2i$.

## Autocorrection D

### (i)



```math
z^2+z+1=0\iff\boxed{z=\frac{-1\pm i\sqrt3}{2}}.
```



### (ii)



```math
z^2-2iz+2-4i=(z-1-3i)(z+1+i).
```





```math
\boxed{z\in\{1+3i,-1-i\}}.
```



### (iii)



```math
z^2-2iz-1+2i=(z-1)(z+1-2i),\qquad\boxed{z\in\{1,-1+2i\}}.
```



### (iv)



```math
4z^2-16z+11-12i=0\iff(z-2)^2=\frac{5+12i}{4}=\left(\frac{3+2i}{2}\right)^2.
```





```math
\boxed{z\in\{7/2+i,1/2-i\}}.
```



### (v)

Poser $u=z^2$. Alors



```math
u^2-(5-14i)u-24-10i=(u+2i)(u-5+12i).
```



Comme $-2i=(1-i)^2$ et $5-12i=(3-2i)^2$,



```math
\boxed{z\in\{\pm(1-i),\ \pm(3-2i)\}}.
```



### (vi)



```math
mz^4+(m-i)z^2-i=(z^2+1)(mz^2-i).
```



Pour $m\ne0$,



```math
\boxed{z\in\left\{i,-i,\ \pm\frac{1+i\operatorname{sgn}(m)}{\sqrt{2|m|}}\right\}}.
```



## Autocorrection E

Les nombres $x,y$ sont les deux racines de $T^2-sT+p$, où $s=x+y$ et $p=xy$ ; les deux ordres sont admis.



```math
\begin{array}{c|c}
(i)&(x,y)=(1+i,1-i)\text{ ou }(1-i,1+i)\\
(ii)&(x,y)=(-1,1+3i)\text{ ou }(1+3i,-1)\\
(iii)&(x,y)=(5i,3-i)\text{ ou }(3-i,5i)
\end{array}
```



Pour (iv), le discriminant vaut $\Delta=(1+i)^2-8=-8+2i$. Poser



```math
d=\sqrt{\sqrt{17}-4}+i\sqrt{\sqrt{17}+4},\qquad d^2=-8+2i.
```



Les solutions sont



```math
\boxed{(x,y)=\left(\frac{1+i+d}{2},\frac{1+i-d}{2}\right)\quad\text{ou le couple inversé}}.
```



## Exercice 7

Pour une racine réelle $t$, les parties réelle et imaginaire donnent



```math
t^3+3t^2-3t-m=0,\qquad t^2-1=0.
```



Ainsi $t=1$ impose $m=1$, et $t=-1$ impose $m=5$. Réciproquement, ces deux couples satisfont l'équation.



```math
\boxed{m\in\{1,5\}}.
```



## Exercice 8

Pour $z=x+iy$, $y\ne0$, l'équation donne



```math
2xy+py=0\Longrightarrow p=-2x,
```





```math
x^2-y^2+px+q=0\Longrightarrow q=x^2+y^2.
```





```math
\boxed{p=-2\operatorname{Re}z,\qquad q=|z|^2},\qquad X^2+pX+q=(X-z)(X-\overline z).
```



## Exercice 9

Noter $u,v$ les deux racines. Alors $u+v=p$, $uv=q^2\ne0$, et $|u/v|=1$. Donc



```math
\frac{p^2}{q^2}=\frac{(u+v)^2}{uv}=2+\frac uv+\frac vu=2+2\operatorname{Re}\left(\frac uv\right)\in[0,4].
```



Un nombre complexe dont le carré est réel positif ou nul est réel : si $w=a+ib$, $w^2\ge0$ impose $ab=0$ et $a^2-b^2\ge0$, donc $b=0$. Ainsi $\boxed{p/q\in\mathbb R}$.

## Autocorrection F



```math
\begin{array}{c|c}
(i)&2\sqrt2\,e^{-i\pi/4}\\
(ii)&e^{i\pi/2}\\
(iii)&e^{i\pi/3}\\
(v)&e^{\cos\theta}e^{i\sin\theta}
\end{array}
```



Pour (iv) et (vi),



```math
e^{i\theta}+e^{2i\theta}=2\cos(\theta/2)e^{3i\theta/2},\qquad1+\cos\theta+i\sin\theta=2\cos(\theta/2)e^{i\theta/2}.
```



Si $c=\cos(\theta/2)>0$, ces expressions sont déjà sous forme exponentielle de module $2c$. Si $c<0$, les modules sont $-2c$ et il faut ajouter $\pi$ aux arguments affichés. Si $c=0$, les deux nombres sont nuls.

## Autocorrection G



```math
1-i=\sqrt2e^{-i\pi/4},\quad\sqrt3+i=2e^{i\pi/6},\quad-1-i\sqrt3=2e^{-2i\pi/3}.
```





```math
\frac{(1-i)^{10}(\sqrt3+i)^5}{(-1-i\sqrt3)^{10}}=\frac{2^5\cdot2^5}{2^{10}}e^{i(-5\pi/2+5\pi/6+20\pi/3)}=e^{5i\pi}=\boxed{-1}.
```



## Autocorrection H



```math
z^n=2^ne^{in\pi/6}.
```





```math
\boxed{z^n\in\mathbb R\iff n\equiv0\pmod6},
```





```math
\boxed{z^n\in\mathbb R_-\iff n\equiv6\pmod{12}},\qquad\boxed{z^n\in i\mathbb R_+\iff n\equiv3\pmod{12}}.
```



Les valeurs $z^n$ ne sont jamais nulles.

## Exercice 10

### (i)

L'expression imprimée ne comporte pas de $i$ :



```math
\boxed{\left(\frac{1+\sqrt3}{2}\right)^{66}=\exp\left(66\ln\frac{1+\sqrt3}{2}\right)}.
```



Avec $i\sqrt3/2$ à la place de $\sqrt3/2$, la valeur serait $e^{66i\pi/3}=1$.

### (ii)



```math
(1+i)^{18}=2^9e^{9i\pi/2}=\boxed{512i}.
```



### (iii)



```math
\left(\frac{1+i\sqrt3}{1-i}\right)^{20}=(\sqrt2e^{7i\pi/12})^{20}=2^{10}e^{5i\pi/3}=\boxed{512-512i\sqrt3}.
```



### (iv)



```math
\frac{(1+i)^4}{(1-i)^3}=1-i,\qquad\frac{(1-i)^4}{(1+i)^3}=1+i.
```



La somme vaut $\boxed2$.

### (v)–(vi)



```math
\boxed{(1+j)^n=e^{in\pi/3}},\qquad\boxed{(1+i\sqrt3)^n+(1-i\sqrt3)^n=2^{n+1}\cos(n\pi/3)}.
```



## Exercice 11

Les nombres $(2+i\sqrt5)^7$ et $(2-i\sqrt5)^7$ sont conjugués ; leur somme vaut $2\operatorname{Re}((2+i\sqrt5)^7)\in\mathbb R$.

De même,



```math
\frac{19+7i}{9-i}=2+i,\qquad\frac{20+5i}{7+6i}=2-i,
```





```math
\left(\frac{19+7i}{9-i}\right)^n+\left(\frac{20+5i}{7+6i}\right)^n=2\operatorname{Re}((2+i)^n)\in\mathbb R.
```



## Exercice 12

Le quotient est défini si et seulement si $e^{i(\theta_1+\theta_2)}\ne-1$, soit $\theta_1+\theta_2\notin\pi+2\pi\mathbb Z$. Dans ce cas,



```math
\boxed{\frac{z_1+z_2}{1+z_1z_2}=\frac{2e^{i(\theta_1+\theta_2)/2}\cos((\theta_1-\theta_2)/2)}{2e^{i(\theta_1+\theta_2)/2}\cos((\theta_1+\theta_2)/2)}=\frac{\cos((\theta_1-\theta_2)/2)}{\cos((\theta_1+\theta_2)/2)}}.
```



## Exercice 13

### 1

Pour $|z|=1$, $\overline z=1/z$. Ainsi



```math
\overline{\left(i\frac{1+z}{1-z}\right)}=-i\frac{1+1/z}{1-1/z}=i\frac{1+z}{1-z}.
```



Le nombre est réel lorsque $z\ne1$.

### 2

Appliquer 1 à $-z$, puis poser



```math
a=i\frac{1-z}{1+z}\in\mathbb R.
```



On a $ia=(z-1)/(z+1)$, donc



```math
\boxed{z=\frac{1+ia}{1-ia}}.
```



Le dénominateur $1-ia$ ne s'annule pas pour $a\in\mathbb R$.

## Exercice 14

Pour $z=x+iy\ne0$,



```math
\operatorname{Im}\left(z+\frac1z\right)=y\left(1-\frac1{|z|^2}\right).
```



Cette quantité s'annule si et seulement si $y=0$ ou $|z|=1$, donc



```math
\boxed{\left\{z\ne0:z+\frac1z\in\mathbb R\right\}=\mathbb R^*\cup\mathbb U}.
```



## Exercice 15

Pour $\zeta=e^{2i\pi/n}\ne1$, la somme $S=1+\zeta+\cdots+\zeta^{n-1}$ vérifie $\zeta S=S$, par permutation des termes. Ainsi $S=0$ et sa partie réelle donne



```math
\boxed{\sum_{k=0}^{n-1}\cos(2\pi k/n)=0}.
```



## Exercice 16

Par l'inégalité triangulaire inversée,



```math
\left|\sum_{k=1}^n\frac{e^{i\theta_k}}{2^k}\right|\ge\frac12-\sum_{k=2}^n\frac1{2^k}=\boxed{2^{-n}>0}.
```



## Autocorrection I

Si $\theta\in2\pi\mathbb Z$,



```math
\sum_{k=0}^n\cos(\varphi+k\theta)=(n+1)\cos\varphi,\qquad\sum_{k=0}^n\sin(\varphi+k\theta)=(n+1)\sin\varphi.
```



Sinon,



```math
\sum_{k=0}^ne^{i(\varphi+k\theta)}=e^{i\varphi}\frac{1-e^{i(n+1)\theta}}{1-e^{i\theta}}=\frac{\sin((n+1)\theta/2)}{\sin(\theta/2)}e^{i(\varphi+n\theta/2)}.
```



Donc



```math
\boxed{\sum_{k=0}^n\cos(\varphi+k\theta)=\frac{\sin((n+1)\theta/2)}{\sin(\theta/2)}\cos(\varphi+n\theta/2)},
```





```math
\boxed{\sum_{k=0}^n\sin(\varphi+k\theta)=\frac{\sin((n+1)\theta/2)}{\sin(\theta/2)}\sin(\varphi+n\theta/2)}.
```



## Exercice 17

Utiliser $\cos^2t=(1+\cos2t)/2$ et $\sin^2t=(1-\cos2t)/2$. Si $\theta\notin\pi\mathbb Z$,



```math
\boxed{\sum_{k=0}^n\cos^2(k\theta)=\frac{n+1}{2}+\frac{\sin((n+1)\theta)\cos(n\theta)}{2\sin\theta}},
```





```math
\boxed{\sum_{k=0}^n\sin^2(k\theta)=\frac{n+1}{2}-\frac{\sin((n+1)\theta)\cos(n\theta)}{2\sin\theta}}.
```



Si $\theta\in\pi\mathbb Z$, les sommes valent respectivement $n+1$ et $0$.

## Exercice 18

Le binôme donne



```math
\sum_{k=0}^n\binom nk e^{ik\theta}=(1+e^{i\theta})^n=2^n\cos^n(\theta/2)e^{in\theta/2}.
```





```math
\boxed{\sum_{k=0}^n\binom nk\cos(k\theta)=2^n\cos^n(\theta/2)\cos(n\theta/2)},
```





```math
\boxed{\sum_{k=0}^n\binom nk\sin(k\theta)=2^n\cos^n(\theta/2)\sin(n\theta/2)}.
```



## Exercice 19

### 1

Pour $x\notin\pi\mathbb Z$, la somme géométrique donne



```math
\boxed{\sum_{k=0}^{n-1}\cos(2kx)=\frac{\sin(nx)\cos((n-1)x)}{\sin x}},
```





```math
\boxed{\sum_{k=0}^{n-1}\cos((2k+1)x)=\frac{\sin(nx)\cos(nx)}{\sin x}=\frac{\sin(2nx)}{2\sin x}}.
```



Pour $x=m\pi$, les sommes valent respectivement $n$ et $n(-1)^m$.

### 2



```math
\cos\frac\pi7+\cos\frac{3\pi}7+\cos\frac{5\pi}7=\frac{\sin(6\pi/7)}{2\sin(\pi/7)}=\frac12.
```



Donc



```math
\boxed{\cos^2\frac\pi{14}+\cos^2\frac{3\pi}{14}+\cos^2\frac{5\pi}{14}=\frac32+\frac14=\frac74}.
```



## Exercice 20

L'hypothèse $2^nx/\pi\notin\mathbb Z$ assure $\sin(2^kx)\ne0$ pour $0\le k\le n$. Or



```math
\cot t-\cot(2t)=\frac{\cos t\sin(2t)-\cos(2t)\sin t}{\sin t\sin(2t)}=\frac1{\sin(2t)}.
```



Par télescopage,



```math
\boxed{\sum_{k=1}^n\frac1{\sin(2^kx)}=\cot x-\cot(2^nx)}.
```



## Exercice 21



```math
S_0+S_1+S_2=2^n,
```





```math
S_0+jS_1+j^2S_2=(1+j)^n=e^{in\pi/3},
```





```math
S_0+j^2S_1+jS_2=(1+j^2)^n=e^{-in\pi/3}.
```



Pour $r\in\{0,1,2\}$, multiplier les deux dernières égalités par $j^{-r}$ et $j^{-2r}$, puis les ajouter à la première. Les autres classes s'annulent puisque $1+j+j^2=0$ :



```math
\boxed{S_r=\frac13\left(2^n+2\cos\left(\frac{n\pi}{3}-\frac{2r\pi}{3}\right)\right)}.
```



## Exercice 22

Les termes d'indice impair dans le développement de $(1+i)^{4n}$ donnent sa partie imaginaire :



```math
\sum_{p=0}^{2n-1}(-1)^p\binom{4n}{2p+1}=\operatorname{Im}(1+i)^{4n}=\operatorname{Im}(2^{2n}e^{in\pi})=\boxed0.
```



Pour $n=0$, la somme est vide et vaut aussi $0$.

## Exercice 23

Pour $n\ge1$ et $|z|\ne1$,



```math
\left|\frac{1-z^n}{1-z}\right|=\left|\sum_{k=0}^{n-1}z^k\right|\le\sum_{k=0}^{n-1}|z|^k=\boxed{\frac{1-|z|^n}{1-|z|}}.
```



Pour $n=0$, les deux membres sont nuls.

## Exercice 24

Poser $u=a+b$ et $v=a-b$. Les deux inégalités triangulaires donnent



```math
|a|+|b|=\frac{|u+v|+|u-v|}{2}\le|u|+|v|=|a+b|+|a-b|.
```



L'égalité impose simultanément l'égalité triangulaire pour $(u,v)$ et pour $(u,-v)$. Si $u,v\ne0$, la première impose qu'ils aient le même argument, et la seconde qu'ils aient des arguments opposés, contradiction. Ainsi $u=0$ ou $v=0$.



```math
\boxed{\text{Égalité}\iff a=b\ \text{ou}\ a=-b}.
```



## Exercice 25



```math
1=(1+a)-(a+b)+(b+c)-c.
```



L'inégalité triangulaire donne $\boxed{1\le|1+a|+|a+b|+|b+c|+|c|}$.

## Exercice 26

Avec $x=|\operatorname{Re}z|$, $y=|\operatorname{Im}z|$,



```math
x^2+y^2\le(x+y)^2\le2(x^2+y^2),
```



la deuxième inégalité équivalant à $(x-y)^2\ge0$. En prenant les racines carrées,



```math
\boxed{\frac{x+y}{\sqrt2}\le|z|\le x+y}.
```



## Exercice 27



```math
|e^z|=e^{\operatorname{Re}z}\le e^{|z|}.
```



L'égalité équivaut à $\operatorname{Re}z=|z|$, donc à $\boxed{z\in\mathbb R_+}$.

## Exercice 28



```math
|a+b|^2+|a-b|^2=2|a|^2+2|b|^2\le4.
```



Les deux carrés ne peuvent donc pas être strictement supérieurs à $2$. Ainsi $|a+b|\le\sqrt2$ ou $|a-b|\le\sqrt2$.

## Exercice 29

Si $|1+z|<1$ avec $|z|=1$, alors



```math
2+2\operatorname{Re}z<1\Longrightarrow\operatorname{Re}z<-1/2.
```



Or $1+z^2=z(\overline z+z)$, donc $|1+z^2|=2|\operatorname{Re}z|>1$. Cela prouve l'alternative demandée.

## Exercice 30



```math
|z|^2=|z^2|\le|z^2-1|+1\le9\Longrightarrow|z|\le3.
```



Donc $\boxed{|z-2|\le|z|+2\le5}$.

## Exercice 31

Poser $a=e^{ix}$, $b=e^{iy}$ et $c=e^{iz}$. Comme $a+b+c=0$ et $\overline a=1/a$, etc.,



```math
ab+bc+ca=abc(\overline a+\overline b+\overline c)=0.
```



Donc $a^2+b^2+c^2=(a+b+c)^2-2(ab+bc+ca)=0$, soit l'égalité demandée.

## Exercice 32



```math
ab+bc+ca=abc(\overline a+\overline b+\overline c)=abc\,\overline{a+b+c}.
```



Comme $|abc|=1$, $\boxed{|ab+bc+ca|=|a+b+c|}$.

## Exercice 33

Le dénominateur est non nul puisque $|\overline a b|<1$. Un développement donne



```math
|1-\overline a b|^2-|a-b|^2=(1-|a|^2)(1-|b|^2)>0.
```



Donc $\boxed{\left|\frac{a-b}{1-\overline a b}\right|<1}$.

## Exercice 34



```math
(1+|a|^2)(1+|b|^2)-|a+b|^2=1+|a|^2|b|^2-2\operatorname{Re}(a\overline b)=|1-a\overline b|^2\ge0.
```



Ainsi $\boxed{|a+b|^2\le(1+|a|^2)(1+|b|^2)}$.

## Exercice 35

Écrire $z=e^{i\theta}$ avec $0<|\theta|\le\pi$. Si $|\theta|\ge2\pi/3$, prendre $n=1$. Sinon, prendre $n=\lceil2\pi/(3|\theta|)\rceil$. Dans les deux cas,



```math
\frac{2\pi}{3}\le n|\theta|\le\frac{4\pi}{3}.
```



Par conséquent,



```math
|z^n-1|^2=2-2\cos(n\theta)\ge3,\qquad\boxed{|z^n-1|\ge\sqrt3}.
```



## Exercice 36

### 1

Poser $M=\max_k|z_k|$. Construire des réels $t_k\in[-1,1]$ tels que $\sum_kt_kz_k=0$ et au plus deux des $t_k$ appartiennent à $]-1,1[$.

Partir de $t_k=0$. S'il reste au moins trois indices avec $|t_k|<1$, les vecteurs correspondants dans $\mathbb R^2\simeq\mathbb C$ sont liés sur $\mathbb R$ : il existe une famille réelle non nulle $(h_k)$ portée par ces indices et telle que $\sum_kh_kz_k=0$. Faire varier $t_k$ en $t_k+sh_k$ jusqu'au premier contact avec une borne $-1$ ou $1$. Les contraintes restent satisfaites, et le nombre de coefficients strictement intérieurs diminue. Après un nombre fini d'étapes, il en reste au plus deux.

Noter $a,b$ ces deux coefficients et $u,v$ les vecteurs associés ; ajouter au besoin un coefficient nul et un vecteur nul s'il en reste moins de deux. Pour $\sigma,\tau\in\{-1,1\}$, poser



```math
p_\sigma=\frac{1+\sigma a}{2},\qquad q_\tau=\frac{1+\tau b}{2}.
```



Ces nombres sont positifs ou nuls, et les poids $p_\sigma q_\tau$ ont pour somme $1$. Comme $\sum_\sigma p_\sigma\sigma=a$ et $\sum_\tau q_\tau\tau=b$,



```math
\sum_{\sigma,\tau}p_\sigma q_\tau\left|(\sigma-a)u+(\tau-b)v\right|^2=(1-a^2)|u|^2+(1-b^2)|v|^2\le2M^2.
```



Un des quatre carrés est donc au plus $2M^2$. Remplacer $a,b$ par les signes correspondants, et conserver les autres coefficients, déjà dans $\{-1,1\}$. Puisque la somme initiale était nulle, la nouvelle somme est précisément $(\sigma-a)u+(\tau-b)v$. Ainsi



```math
\boxed{\left|\sum_{k=1}^n\epsilon_kz_k\right|\le\sqrt2\,M}.
```



### 2

Pour $\theta\in[0,2\pi]$, poser $F(\theta)=\sum_k|\operatorname{Re}(e^{-i\theta}z_k)|$. Si $z_k=r_ke^{i\alpha_k}$,



```math
\frac1{2\pi}\int_0^{2\pi}F(\theta)\,d\theta=\frac1{2\pi}\sum_kr_k\int_0^{2\pi}|\cos(\alpha_k-\theta)|\,d\theta=\frac2\pi\sum_k|z_k|.
```



Il existe donc $\theta$ tel que $F(\theta)\ge(2/\pi)\sum_k|z_k|$. Choisir $\epsilon_k$ selon le signe de $\operatorname{Re}(e^{-i\theta}z_k)$, avec un signe arbitraire si cette partie réelle est nulle. Alors



```math
\left|\sum_k\epsilon_kz_k\right|\ge\operatorname{Re}\left(e^{-i\theta}\sum_k\epsilon_kz_k\right)=F(\theta)\ge\boxed{\frac2\pi\sum_k|z_k|}.
```



## Exercice 37



```math
|z+z'|^2=|z|^2+|z'|^2+2\operatorname{Re}(z\overline{z'}),\qquad |z-z'|^2=|z|^2+|z'|^2-2\operatorname{Re}(z\overline{z'}).
```





```math
\boxed{|z+z'|^2+|z-z'|^2=2(|z|^2+|z'|^2).}
```



Dans un parallélogramme de côtés représentés par $z,z'$, la somme des carrés des diagonales est la somme des carrés des quatre côtés.

## Exercice 38

### 1



```math
\boxed{r(z)=2-i+e^{i\pi/4}(z-2+i)},\qquad \boxed{h(z)=-2z+9+6i}.
```



Pour la dernière transformation,



```math
r_1(z)=iz+1-i,\qquad s(z)=6+2i-z,
```





```math
\boxed{(r_1\circ s)(z)=-iz-1+5i=(2+3i)-i(z-2-3i).}
```



C'est la rotation de centre $2+3i$ et d'angle $-\pi/2$.

### 2



```math
e^{i\pi/3}z+1=c+e^{i\pi/3}(z-c),\qquad c=\frac1{1-e^{i\pi/3}}=\frac{1+i\sqrt3}{2}.
```



Rotation de centre $c$, d'angle $\pi/3$.



```math
z+4-2i: \quad\text{translation de vecteur d'affixe }4-2i.
```





```math
3z+i=-\frac i2+3\left(z+\frac i2\right):\quad\text{homothétie de centre }-\frac i2\text{ et de rapport }3.
```



## Exercice 39

### (i)



```math
z=x+iy:\quad z+\overline z=|z|\iff 2x=\sqrt{x^2+y^2}\iff x\ge0,\ y^2=3x^2.
```





```math
\boxed{\{te^{i\pi/3}:t\ge0\}\cup\{te^{-i\pi/3}:t\ge0\}.}
```



### (ii)



```math
|1+z|^2+|1-z|^2=2+2|z|^2\le2\implies z=0.
```



Réciproquement, $z=0$ convient : $\boxed{\{0\}}$.

### (iii)

Pour $z=re^{i\theta}\ne0$,



```math
z\perp\frac1z\iff\operatorname{Re}\left(z\overline{\frac1z}\right)=0\iff\cos(2\theta)=0.
```





```math
\boxed{\{x+iy\ne0:y=x\text{ ou }y=-x\}.}
```



### (iv)



```math
|z|=|z+i|=1\iff x^2+y^2=x^2+(y+1)^2=1\iff y=-\frac12,\ x=\pm\frac{\sqrt3}{2}.
```



Les trois sommets sont alors distincts et non alignés. Ainsi



```math
\boxed{z\in\left\{\frac{\sqrt3-i}{2},\frac{-\sqrt3-i}{2}\right\}.}
```



## Exercice 40



```math
\mathbb Q(j)=\{a+bj:a,b\in\mathbb Q\}=\mathbb Q+i\sqrt3\,\mathbb Q.
```



C'est un corps : pour $u=a+bj\ne0$,



```math
u^{-1}=\frac{a+bj^2}{a^2-ab+b^2}\in\mathbb Q(j).
```



Deux côtés consécutifs d'un carré non dégénéré ont pour affixes $u\ne0$ et $\pm iu$. Si ses sommets appartiennent à $\mathbb Z[j]$, alors $u,\pm iu\in\mathbb Z[j]$, donc $i\in\mathbb Q(j)$. Or



```math
i=r+i\sqrt3\,s,\quad r,s\in\mathbb Q\implies r=0,\ s=\frac1{\sqrt3}\notin\mathbb Q.
```



Contradiction.

## Exercice 41

Les racines cubiques sont $w,jw,j^2w$, où $w^3=z\ne0$. Dans le parallélogramme, le sommet opposé à $z$ est l'une de ces racines ; la noter $w$. L'égalité des milieux des diagonales donne



```math
z+w=jw+j^2w=-w\iff z=-2w.
```





```math
w^3=-2w\iff w^2=-2\iff w=\pm i\sqrt2.
```



Réciproquement, pour ces deux valeurs, les milieux coïncident ; les quatre sommets sont distincts et non alignés. Ainsi



```math
\boxed{z=\pm2i\sqrt2.}
```



## Exercice 42

### 1(a)

Une similitude directe s'écrit $s(u)=\alpha+\beta u$, avec $\beta\ne0$. Elle conserve les angles orientés et multiplie les longueurs par $|\beta|$. L'image de $(1,j,j^2)$ est donc équilatérale directe.

Réciproquement, pour un triangle équilatéral direct $(a,b,c)$, poser



```math
\beta=\frac{b-a}{j-1}\ne0,\qquad\alpha=a-\beta.
```



Alors $s(1)=a$, $s(j)=b$. L'unique troisième sommet donnant un triangle équilatéral direct sur le côté orienté $(a,b)$ est $s(j^2)$ ; donc $s(j^2)=c$.

### 1(b)



```math
a=\alpha+\beta,\quad b=\alpha+\beta j,\quad c=\alpha+\beta j^2
```





```math
\implies a+jb+j^2c=\alpha(1+j+j^2)+\beta(1+j^2+j^4)=0.
```



Réciproquement, avec $a\ne b$, les nombres $\alpha,\beta$ précédents donnent un unique $c$ satisfaisant cette relation, à savoir $\alpha+\beta j^2$.



```math
\boxed{(a,b,c)\text{ équilatéral direct}\iff a+jb+j^2c=0\quad(a\ne b).}
```



Sans l'hypothèse de non-dégénérescence, la relation admet aussi $a=b=c$.

### 2

Dans l'orientation de la figure, les sommets extérieurs vérifient



```math
a'=-j^2b-jc,\qquad b'=-j^2c-ja,\qquad c'=-j^2a-jb.
```



Les centres de gravité sont donc



```math
a''=\frac{(1-j^2)b+(1-j)c}{3},\quad b''=\frac{(1-j^2)c+(1-j)a}{3},\quad c''=\frac{(1-j^2)a+(1-j)b}{3}.
```



En regroupant les coefficients de $a,b,c$ et en utilisant $1+j+j^2=0$,



```math
a''+jb''+j^2c''=0,\qquad a''+j^2b''+jc''=-(a+j^2b+jc).
```



Si $a''=b''=c''$, la seconde égalité imposerait $a+j^2b+jc=0$, donc un triangle initial équilatéral indirect, contrairement à son orientation. Le triangle $(a'',b'',c'')$ est donc équilatéral direct. L'autre orientation se traite en conjuguant toutes les affixes.

## Exercice 43

Poser $t=b/a\in\mathbb U$. Alors $c/a=-1-t$ et $|1+t|=1$. Ainsi



```math
1=|1+t|^2=2+2\operatorname{Re}t\implies\operatorname{Re}t=-\frac12\implies t\in\{j,j^2\}.
```



L'autre rapport vaut l'autre racine. Donc $\{a,b,c\}=\{a,aj,aj^2\}$ : le triangle est équilatéral.

## Autocorrection J

Avec $u=e^{ix}$,



```math
\cos x=\frac{u+u^{-1}}2,\qquad\sin x=\frac{u-u^{-1}}{2i}.
```



Développer, puis regrouper $u^k+u^{-k}=2\cos(kx)$ et $u^k-u^{-k}=2i\sin(kx)$ :



```math
\begin{aligned}
\text{(i)}\quad&\cos^3x=\frac{3\cos x+\cos3x}{4},\\
\text{(ii)}\quad&\sin^3x=\frac{3\sin x-\sin3x}{4},\\
\text{(iii)}\quad&\cos^4x=\frac{3+4\cos2x+\cos4x}{8},\\
\text{(iv)}\quad&\sin^4x=\frac{3-4\cos2x+\cos4x}{8},\\
\text{(v)}\quad&\cos^5x=\frac{10\cos x+5\cos3x+\cos5x}{16},\\
\text{(vi)}\quad&\sin^5x=\frac{10\sin x-5\sin3x+\sin5x}{16},\\
\text{(vii)}\quad&\sin x\cos^2x=\frac{\sin x+\sin3x}{4},\\
\text{(viii)}\quad&\sin^3x\cos^2x=\frac{2\sin x+\sin3x-\sin5x}{16},\\
\text{(ix)}\quad&\sin^3x\cos^3x=\frac{3\sin2x-\sin6x}{32},\\
\text{(x)}\quad&\sin^6x\cos x=\frac{5\cos x-9\cos3x+5\cos5x-\cos7x}{64},\\
\text{(xi)}\quad&\sin^2(2x)\cos3x=\frac{2\cos3x-\cos x-\cos7x}{4},\\
\text{(xii)}\quad&\cos^3x\sin3x=\frac{3\sin2x+3\sin4x+\sin6x}{8}.
\end{aligned}
```



## Autocorrection K

Poser $c=\cos x$, $s=\sin x$. Les parties réelle et imaginaire du développement de $(c+is)^n$ donnent



```math
\begin{aligned}
\text{(i)}\quad&\cos3x=c^3-3cs^2,\\
\text{(ii)}\quad&\sin3x=3c^2s-s^3,\\
\text{(iii)}\quad&\cos4x=c^4-6c^2s^2+s^4,\\
\text{(iv)}\quad&\sin4x=4c^3s-4cs^3,\\
\text{(v)}\quad&\cos5x=c^5-10c^3s^2+5cs^4,\\
\text{(vi)}\quad&\sin5x=5c^4s-10c^2s^3+s^5.
\end{aligned}
```



## Exercice 44

### Racines carrées



```math
(a+ib)^2=\frac{1+i}{\sqrt2}\iff a^2-b^2=\frac1{\sqrt2},\quad 2ab=\frac1{\sqrt2},\quad a^2+b^2=1.
```





```math
a=\pm\frac{\sqrt{2+\sqrt2}}2,\qquad b=\pm\frac{\sqrt{2-\sqrt2}}2,
```



avec des signes identiques. Puisque $e^{i\pi/8}$ est dans le premier quadrant,



```math
\boxed{\cos\frac\pi8=\frac{\sqrt{2+\sqrt2}}2,\qquad\sin\frac\pi8=\frac{\sqrt{2-\sqrt2}}2.}
```



### Angle double



```math
\cos\frac\pi4=2\cos^2\frac\pi8-1\implies\cos^2\frac\pi8=\frac{2+\sqrt2}{4},\qquad\sin^2\frac\pi8=\frac{2-\sqrt2}{4}.
```



Les deux valeurs étant positives, on retrouve les mêmes racines.

## Exercice 45

### Demi-angle



```math
\cos^2\frac\pi{12}=\frac{1+\cos(\pi/6)}2=\frac{2+\sqrt3}{4},\qquad\sin^2\frac\pi{12}=\frac{2-\sqrt3}{4}.
```





```math
\boxed{\cos\frac\pi{12}=\frac{\sqrt6+\sqrt2}{4},\qquad\sin\frac\pi{12}=\frac{\sqrt6-\sqrt2}{4}.}
```



### Différence d'angles



```math
\cos\left(\frac\pi3-\frac\pi4\right)=\frac12\frac{\sqrt2}{2}+\frac{\sqrt3}{2}\frac{\sqrt2}{2}=\frac{\sqrt6+\sqrt2}{4},
```





```math
\sin\left(\frac\pi3-\frac\pi4\right)=\frac{\sqrt3}{2}\frac{\sqrt2}{2}-\frac12\frac{\sqrt2}{2}=\frac{\sqrt6-\sqrt2}{4}.
```



## Exercice 46

Poser $u_n=2\cos(\pi/2^n)$. Alors $u_1=0$, et



```math
u_{n+1}^2=4\cos^2\frac\pi{2^{n+1}}=2+2\cos\frac\pi{2^n}=2+u_n.
```



Comme $u_{n+1}>0$,



```math
u_{n+1}=\sqrt{2+u_n},\qquad u_2=\sqrt2.
```



Par récurrence, pour $n\ge2$,



```math
\boxed{2\cos\frac\pi{2^n}=\sqrt{2+\sqrt{2+\cdots+\sqrt2}}}\qquad(n-1\text{ radicaux}).
```



Pour $n=1$, la valeur initiale est $0$.

## Exercice 47



```math
\begin{aligned}
(a+bj+cj^2)(a+bj^2+cj)
&=a^2+b^2+c^2+(ab+ac+bc)(j+j^2)\\
&=\boxed{a^2+b^2+c^2-ab-ac-bc}.
\end{aligned}
```





```math
\begin{aligned}
(a+b+c)(a+bj+cj^2)(a+bj^2+cj)
&=(a+b+c)(a^2+b^2+c^2-ab-ac-bc)\\
&=\boxed{a^3+b^3+c^3-3abc}.
\end{aligned}
```



## Exercice 48



```math
\prod_{\omega\in\mathbb U_n}\omega=\prod_{k=0}^{n-1}e^{2i\pi k/n}=\exp\left(\frac{2i\pi}{n}\frac{n(n-1)}2\right)=\boxed{(-1)^{n-1}}.
```



## Exercice 49

### 1



```math
\omega^n=1\implies(\omega^2)^n=1\implies\boxed{Q\subseteq\mathbb U_n}.
```



### 2

Si $n$ est impair, pour $\eta\in\mathbb U_n$, poser $\omega=\eta^{(n+1)/2}\in\mathbb U_n$. Alors $\omega^2=\eta^{n+1}=\eta$, donc $Q=\mathbb U_n$.

Si $n=2m$, alors



```math
Q=\{e^{2i\pi k/m}:0\le k<2m\}=\mathbb U_m\subsetneq\mathbb U_n.
```





```math
\boxed{Q=\mathbb U_n\iff n\text{ impair}.}
```



## Exercice 50

### 1

Avec $\zeta=e^{2i\pi/5}$,



```math
1+\zeta+\zeta^2+\zeta^3+\zeta^4=0\implies\boxed{1+2\cos\frac{2\pi}5+2\cos\frac{4\pi}5=0}.
```



### 2

Poser $c=\cos(2\pi/5)>0$. Alors



```math
1+2c+2(2c^2-1)=0\iff4c^2+2c-1=0.
```





```math
c=\frac{-1\pm\sqrt5}{4},\qquad\boxed{c=\frac{\sqrt5-1}{4}}.
```



### 3



```math
\sin\frac{2\pi}5=\sqrt{1-c^2}=\boxed{\frac{\sqrt{10+2\sqrt5}}4}.
```





```math
\boxed{\cos\frac\pi{10}=\frac{\sqrt{10+2\sqrt5}}4,\qquad\sin\frac\pi{10}=\frac{\sqrt5-1}{4}.}
```





```math
\cos\frac\pi5=\sqrt{\frac{1+c}{2}}=\frac{1+\sqrt5}{4},\qquad\sin\frac\pi5=\sqrt{\frac{1-c}{2}}=\frac{\sqrt{10-2\sqrt5}}4.
```



## Exercice 51

Pour $\theta=2\pi/7$, la somme des sept racines de l'unité donne



```math
1+2\cos\theta+2\cos2\theta+2\cos3\theta=0.
```



Poser $c=\cos\theta$ :



```math
1+2c+2(2c^2-1)+2(4c^3-3c)=0\implies\boxed{8c^3+4c^2-4c-1=0}.
```



## Exercice 52

Poser $\zeta=\zeta_7$. Alors



```math
A+B=\sum_{k=1}^6\zeta^k=\boxed{-1},
```





```math
AB=(\zeta+\zeta^2+\zeta^4)(\zeta^3+\zeta^5+\zeta^6)=3+\sum_{k=1}^6\zeta^k=\boxed2.
```



Ainsi $A,B$ sont les racines de $T^2+T+2$, soit $(-1\pm i\sqrt7)/2$. De plus



```math
\operatorname{Im}A=\sin\frac{2\pi}7+\sin\frac{3\pi}7-\sin\frac\pi7>0,
```



car $0<\pi/7<2\pi/7<\pi/2$. Par conséquent



```math
\boxed{A=\frac{-1+i\sqrt7}{2},\qquad B=\frac{-1-i\sqrt7}{2}.}
```



## Exercice 53

### 1

Poser $a=\omega+\omega^{-1}$, $b=\omega^2+\omega^{-2}$, $c=\omega^3+\omega^{-3}$. Comme $\omega\ne1$ et $\omega^7=1$,



```math
a+b+c=\sum_{k=1}^6\omega^k=-1.
```





```math
ab=a+c,\qquad ac=b+c,\qquad bc=a+b\implies ab+ac+bc=-2.
```





```math
abc=2+\omega^2+\omega^{-2}+\omega^4+\omega^{-4}+\omega^6+\omega^{-6}=2+\sum_{k=1}^6\omega^k=1.
```



En particulier, les dénominateurs suivants sont non nuls, et



```math
\frac{\omega}{1+\omega^2}+\frac{\omega^2}{1+\omega^4}+\frac{\omega^3}{1+\omega^6}=\frac1a+\frac1b+\frac1c=\frac{ab+ac+bc}{abc}=\boxed{-2}.
```



### 2

Pour $\omega=e^{2i\pi/7}$, $\omega^k+\omega^{-k}=2\cos(2k\pi/7)$. Donc



```math
\boxed{\frac1{\cos(2\pi/7)}+\frac1{\cos(4\pi/7)}+\frac1{\cos(6\pi/7)}=-4.}
```



## Autocorrection L

### (i)



```math
\frac{1+i}{\sqrt3-i}=2^{-1/2}e^{5i\pi/12}.
```





```math
\boxed{z=2^{-1/16}e^{i(5\pi/96+k\pi/4)},\qquad k\in\{0,\ldots,7\}.}
```



### (ii)



```math
\boxed{z=e^{i(\pi/(2n)+2k\pi/n)},\qquad k\in\{0,\ldots,n-1\}.}
```



### (iii)



```math
(2+i)^2=3+4i,\qquad(2+i)^4=-7+24i.
```





```math
\boxed{z\in(2+i)\mathbb U_4=\{2+i,-1+2i,-2-i,1-2i\}.}
```



### (iv)



```math
z^8-3z^4+2=(z^4-1)(z^4-2)\implies\boxed{z\in\mathbb U_4\cup2^{1/4}\mathbb U_4}.
```



## Exercice 54



```math
1+\overline z=|z|\implies\operatorname{Im}z=0.
```



Pour $z=x\in\mathbb R$, si $x\ge0$, l'équation donne $1=0$ ; si $x<0$, elle donne $1+x=-x$. Ainsi



```math
\boxed{z=-\frac12.}
```



## Exercice 55

Dans toutes les familles ci-dessous, $k\in\mathbb Z$.

### (i)



```math
|e^z|=e^{\operatorname{Re}z}>0\implies\boxed{\varnothing}.
```



### (ii)



```math
e^z=i\iff\boxed{z=i\left(\frac\pi2+2k\pi\right)}.
```



### (iii)



```math
1+i=\sqrt2e^{i\pi/4}\implies\boxed{z=\frac{\ln2}{2}+i\left(\frac\pi4+2k\pi\right)}.
```



### (iv)

Poser $w=e^z\ne0$ :



```math
w+w^{-1}=1\iff w^2-w+1=0\iff w=e^{\pm i\pi/3}.
```





```math
\boxed{z=i\left(\pm\frac\pi3+2k\pi\right).}
```



### (v)



```math
w+2w^{-1}=i\iff w^2-iw+2=(w-2i)(w+i)=0.
```





```math
\boxed{z=\ln2+i\left(\frac\pi2+2k\pi\right)\quad\text{ou}\quad z=i\left(-\frac\pi2+2k\pi\right).}
```



## Exercice 56

Le dénominateur $\overline z-i$ s'annule pour $z=-i$. Pour tout autre $z$,



```math
\left|\frac{z+i}{\overline z-i}\right|=\frac{|z+i|}{|\overline z-i|}=\frac{|z+i|}{|z+i|}=1.
```





```math
\boxed{\mathbb C\setminus\{-i\}}.
```



## Exercice 57

$z=0$ convient. Pour $z=re^{i\theta}$, $r>0$,



```math
\operatorname{Re}(z^3)=\operatorname{Im}(z^3)\iff\cos3\theta=\sin3\theta\iff3\theta\equiv\frac\pi4\pmod\pi.
```





```math
\boxed{\bigcup_{k=0}^2\left\{te^{i(\pi/12+k\pi/3)}:t\in\mathbb R\right\}.}
```



## Exercice 58



```math
|z|=\left|\frac1z\right|\iff|z|=1.
```





```math
|1-z|^2=1+|z|^2-2\operatorname{Re}z=1\iff\operatorname{Re}z=\frac12.
```





```math
\boxed{z=\frac{1\pm i\sqrt3}{2}.}
```



## Exercice 59

L'équation imprimée est $z^n=\overline z$.

Si $n=1$,



```math
z=\overline z\iff\boxed{z\in\mathbb R}.
```



Si $n\ge2$, $z=0$ convient. Pour $z=re^{i\theta}\ne0$,



```math
r^ne^{in\theta}=re^{-i\theta}\iff r^{n-1}=1,\quad e^{i(n+1)\theta}=1.
```





```math
\boxed{z\in\{0\}\cup\mathbb U_{n+1}\qquad(n\ge2).}
```



## Exercice 60

### (i)

Pour $z=re^{it}\ne0$,



```math
\overline z^{\,7}=\frac1{z^2}\iff r^7e^{-7it}=r^{-2}e^{-2it}\iff r^9=1,\quad e^{-5it}=1.
```





```math
\boxed{z\in\mathbb U_5.}
```



### (ii)



```math
e^{2i\theta}-2i\sin\theta\,e^{i\theta}=e^{i\theta}(e^{i\theta}-2i\sin\theta)=1.
```



Donc le discriminant vaut $4$, et



```math
\boxed{z=e^{i\theta}\pm1.}
```



### (iii)



```math
z^{2n}-2\cos(n\theta)z^n+1=(z^n-e^{in\theta})(z^n-e^{-in\theta}).
```





```math
\boxed{z\in e^{i\theta}\mathbb U_n\cup e^{-i\theta}\mathbb U_n.}
```



Les deux ensembles coïncident si et seulement si $n\theta\in\pi\mathbb Z$ ; sinon ils sont disjoints.

### (iv)



```math
16\sqrt2+16i\sqrt2=32e^{i\pi/4}\implies\boxed{z=2e^{i(\pi/20+2k\pi/5)},\quad k=0,\ldots,4}.
```



### (v)



```math
z^7-4z^5-z^2+4=(z^2-4)(z^5-1)\implies\boxed{z\in\{-2,2\}\cup\mathbb U_5}.
```



### (vi)



```math
z^8+2z^7-2z-4=(z+2)(z^7-2)\implies\boxed{z\in\{-2\}\cup2^{1/7}\mathbb U_7}.
```



## Exercice 61



```math
|a+ib|^3=|2+11i|=5\sqrt5\implies a^2+b^2=5.
```



Parmi les couples entiers possibles, $(a,b)=(2,1)$ donne



```math
(2+i)^3=(3+4i)(2+i)=2+11i.
```





```math
z^3=(2+i)^3\iff\left(\frac z{2+i}\right)^3=1\iff\boxed{z\in(2+i)\mathbb U_3}.
```



## Exercice 62

$z=i$ n'est pas solution. Pour $z\ne i$,



```math
(z+i)^n=(z-i)^n\iff w=\frac{z+i}{z-i}\in\mathbb U_n.
```



La valeur $w=1$ est impossible. Pour $w=e^{2ik\pi/n}\ne1$,



```math
z=i\frac{w+1}{w-1}=i\frac{2e^{ik\pi/n}\cos(k\pi/n)}{2ie^{ik\pi/n}\sin(k\pi/n)}=\cot\frac{k\pi}{n}.
```





```math
\boxed{z\in\left\{\cot\frac{k\pi}{n}:1\le k\le n-1\right\}.}
```



Pour $n=1$, l'ensemble est vide.

## Exercice 63

Poser



```math
w=\frac{1+iz}{1-iz},\qquad z\ne-i.
```



Cette transformation est une bijection de $\mathbb C\setminus\{-i\}$ sur $\mathbb C\setminus\{-1\}$, d'inverse



```math
z=i\frac{1-w}{1+w}.
```



En écrivant $z=x+iy$,



```math
|1+iz|^2-|1-iz|^2=-4y\implies\boxed{z\in\mathbb R\iff|w|=1}.
```



Si $|A|=1$, chaque racine de $w^n=A$ a pour module $1$ ; toutes celles différentes de $-1$ donnent des solutions réelles.

Si $|A|\ne1$, les racines de $w^n=A$ ont toutes un module différent de $1$ ; elles sont donc différentes de $-1$, et donnent des solutions non réelles. Il en existe au moins une, y compris pour $A=0$.



```math
\boxed{\text{Toutes les solutions sont réelles}\iff |A|=1\qquad(n\ge1).}
```



Pour $A=e^{i\alpha}$, elles s'écrivent



```math
\boxed{z=\tan\frac{\alpha+2k\pi}{2n},\qquad0\le k<n,\quad\frac{\alpha+2k\pi}{n}\not\equiv\pi\pmod{2\pi}.}
```



Il y en a $n$, sauf si $A=(-1)^n$, auquel cas il y en a $n-1$. Pour $n=1$, $A=-1$, il n'y a aucune solution.
