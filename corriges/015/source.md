# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td15-suites.pdf)

## Autocorrection A

(i) $u_n=7(-2)^{n-1}$ pour $n\ge1$.

(ii) $u_n=3\,2^{1-n}$ pour $n\ge1$.

(iii) $u_n=10+3n$.

(iv) Le point fixe de $x\mapsto x/3+4$ est $6$. Ainsi $u_n-6=(u_0-6)3^{-n}$, donc $u_n=6-5\,3^{-n}$.

(v) $u_{n+1}+1/3=(u_n+1/3)/4$, donc $u_n=(4^{-n}-1)/3$.

(vi) La différence $u_{n+1}-u_n$ est constante et vaut $-1$; $u_n=2-n$.

(vii) L’équation caractéristique $2r^2+r-1=0$ a pour racines $1/2$ et $-1$. Les conditions initiales donnent $u_n=\frac43(\frac12)^n-\frac13(-1)^n$.

(viii) Les racines de $r^2-r-3=0$ sont $r_\pm=(1\pm\sqrt{13})/2$. En posant $u_n=Ar_+^n+Br_-^n$, les conditions initiales donnent $A=(3+\sqrt{13})/(2\sqrt{13})$, $B=(\sqrt{13}-3)/(2\sqrt{13})$.

(ix) $u_1=-2$ et $u_{n+1}=-u_n^2/2$; donc $u_n=-2$ pour tout $n\ge1$.

(x) $u_n=\sum_{k=1}^n k=n(n+1)/2$.

(xi) En posant $v_n=1/u_n$, on obtient $v_{n+1}=v_n+1$ et $v_1=1$; donc $u_n=1/n$.

(xii) Poser $v_n=2u_n$. Alors $v_0=2$ et $v_{n+1}=v_n^2$, donc $v_n=2^{2^n}$ et $u_n=2^{2^n-1}$.

## Exercice 1

(i) Pour $p=0$, $u_n=1$. Pour $p\ge1$, $u_n=0$ si $n<p$ et, dès que $n\ge p$, $u_{n+1}/u_n=(n+1)/(n+1-p)\ge1$. La suite est croissante.

(ii) Pour $n\ge1$,


```math
u_{n+1}-u_n=\frac1{(n+1)^2}+\frac1{n+1}-\frac1n=-\frac1{n(n+1)^2}<0.
```


La suite est strictement décroissante.

(iii) $u_{n+1}/u_n=(n+1)/2$. Elle décroît jusqu’à $n=1$, vérifie $u_1=u_2=1/2$, puis croît strictement dès $n\ge2$.

(iv) $u_{n+1}-u_n=n\ln\!\left(\frac n{n+1}\right)<0$; la suite est strictement décroissante.

(v) $u_{n+1}/u_n=2(n+1)/(2n+3)<1$; la suite est strictement décroissante et positive.

(vi) Si $u_n>0$, alors $u_{n+1}>0$ et


```math
u_{n+1}-u_n=-\frac{u_n(u_n+1)}{1+4u_n}<0.
```


Elle décroît vers une limite $\ell\ge0$. L’équation $\ell=3\ell^2/(1+4\ell)$ impose $\ell=0$.

## Exercice 2+

1. Une suite réelle non bornée est non bornée supérieurement ou inférieurement. Dans le premier cas, choisir $p$ tel que $u_p>u_0+C$ et prendre $q=0$; dans le second, choisir $p$ tel que $u_p<u_0-C$. Alors $|u_p-u_q|>C$.

2. Supposons qu’aucune paire ne vérifie les deux inégalités. Comme $(u_n)$ est non bornée, on peut choisir $p_0,p_1$ tels que $|u_{p_1}-u_{p_0}|>2C$. Pour tout $q$, soit $|u_q-u_{p_0}|>C$, auquel cas l’hypothèse impose $|v_q-v_{p_0}|\le C$, soit $|u_q-u_{p_0}|\le C$, auquel cas $|u_q-u_{p_1}|>C$ et $|v_q-v_{p_1}|\le C$. Ainsi $(v_q)$ est bornée, contradiction.

3. Pour $n\ge0$, définissons $(u_{3n},v_{3n},w_{3n})=(n,0,0)$, $(u_{3n+1},v_{3n+1},w_{3n+1})=(0,n,0)$ et $(u_{3n+2},v_{3n+2},w_{3n+2})=(0,0,n)$. Les trois suites sont non bornées. Entre deux indices quelconques, au moins une coordonnée est nulle aux deux points, donc la différence correspondante vaut $0$. La conclusion simultanée est donc fausse.

## Autocorrection B

(i) $|\cos n/(n+1)|\le1/(n+1)\to0$.

(ii) $|n+(-1)^n|/(n^2+1)\le(n+1)/(n^2+1)\to0$.

(iii) Pour $n\geq1$, $\dfrac{n+(-1)^n}{2+(-1)^n}\geq\dfrac{n-1}{3}\to+\infty$.

(iv) $|e^n+n^2|/(n^4+1)\sim e^n/n^4\to+\infty$.

(v) $(\ln n+1)/(n+4)\to0$.

(vi) $\frac{3^n+(-2)^n}{3^n-(-2)^n}=\frac{1+(-2/3)^n}{1-(-2/3)^n}\to1$.

(vii) $\sqrt{n+1}-\sqrt{n-1}=2/(\sqrt{n+1}+\sqrt{n-1})\to0$.

(viii) $\sqrt{n^2+n}-\sqrt{n^2-n}=2n/(\sqrt{n^2+n}+\sqrt{n^2-n})\to1$.

(ix) $0\leq\lfloor\sqrt n\rfloor/n\leq1/\sqrt n\to0$.

(x) $n!/n^n\le1$ et, pour $k\le\lfloor n/2\rfloor$, le facteur $k/n\le1/2$; donc $n!/n^n\le2^{-\lfloor n/2\rfloor}\to0$.

## Autocorrection C

1. Deux suites convergentes ont une somme convergente. Si une seule converge, leur somme diverge, sinon soustraire la suite convergente donnerait la convergence de l'autre. Deux suites divergentes peuvent avoir une somme convergente ($n+(-n)=0$) ou divergente ($n+n=2n$).

2. Deux suites convergentes ont un produit convergent. Si $u_n\to\ell\ne0$ et $(v_n)$ diverge, leur produit diverge : une limite du produit donnerait celle de $v_n=(u_nv_n)/u_n$. Si $u_n\to0$, les deux cas sont possibles : $u_n=1/n$, avec $v_n=n$ donne un produit constant; avec $v_n=n^2$, un produit divergent. Enfin, deux suites divergentes peuvent avoir un produit convergent ($u_n=v_n=(-1)^n$, produit $1$) ou divergent ($u_n=v_n=n$, produit $n^2$).

## Autocorrection D

On a $\min(u_n,v_n)=\frac12(u_n+v_n-|u_n-v_n|)$ et $\max(u_n,v_n)=\frac12(u_n+v_n+|u_n-v_n|)$. La continuité des opérations et la convergence de $u_n,v_n$ prouvent les deux convergences.

## Exercice 3

Pour $n$ fixé, la limite en $m$ de $\cos(2\pi n!x)^{2m}$ vaut $1$ si $n!x\in\tfrac12\mathbb Z$, et $0$ sinon. Si $x=a/b\in\mathbb Q$, alors $n!x\in\mathbb Z$ dès que $n\ge b$, donc la limite extérieure vaut $1$. Si $x\notin\mathbb Q$, aucun $n!x$ n’est demi-entier; la limite intérieure vaut toujours $0$, donc la limite extérieure vaut $0$.

## Exercice 4

Si $u_n\to\ell$, alors $\lfloor u_n\rfloor$ est stationnaire égal à $\lfloor\ell\rfloor$ lorsque $\ell\notin\mathbb Z$. Si $\ell\in\mathbb Z$, chaque terme entier-partie vaut éventuellement $\ell-1$ ou $\ell$ (et vaut $\ell$ si les termes sont finalement au-dessus de $\ell$); la suite entière-partie peut ne pas converger, par exemple $u_{2n}=\ell-1/(n+1)$, $u_{2n+1}=\ell+1/(n+1)$.

## Exercice 5

On cherche $u_n\to1$, $v_n\to+\infty$ et $u_n^{v_n}\to\ell$. Pour $\ell>0$, prendre $v_n=n$ et $u_n=\ell^{1/n}$ (pour $\ell=1$, on peut prendre $u_n=1$). Pour $\ell=0$, prendre $v_n=n$ et $u_n=1-1/\sqrt n$ à partir de $n\ge2$; alors $n\ln u_n\sim-\sqrt n\to-\infty$. Pour $\ell=+\infty$, prendre $v_n=n$, $u_n=1+1/\sqrt n$; alors $n\ln u_n\sim\sqrt n\to+\infty$.

## Exercice 6

Posons $v_n=1/\sqrt{u_n}$ dès que $u_n>0$, et $v_n=0$ sinon. À partir d’un rang, $u_n>0$ et $u_nv_n=\sqrt{u_n}\to+\infty$, tandis que $v_n\to0$; définir arbitrairement les premiers termes.

## Exercice 7

1. $S_{n+1}-S_n=1/(n+1)^2>0$.
2. Si $n\ge2$, $1/n^2\le1/(n(n-1))=1/(n-1)-1/n$.
3. Par sommation, $S_n\le1+\sum_{k=2}^n(1/(k-1)-1/k)=2-1/n$. Croissante et majorée, $(S_n)$ converge.

## Exercice 8

1. $S_n=\sum_{k=0}^n3^{-k}=\frac32(1-3^{-(n+1)})\to\frac32$.
2. En décalant l’indice, $T_{n+1}=\frac13\sum_{j=0}^n(j+1)3^{-j}=(T_n+S_n)/3$.
3. La formule de somme géométrique dérivée donne $T_n=\frac34-(\frac n2+\frac34)3^{-n}$, donc $T_n\to3/4$.

## Exercice 9

Les deux termes extrêmes de $A_n=\sum_{k=0}^n\binom nk^{-1}$ valent $1$. Les deux termes voisins valent $1/n$. Pour $2\le k\le n-2$, $\binom nk\ge\binom n2$, d’où


```math
0\le A_n-2\le\frac2n+\frac{n-3}{\binom n2}\longrightarrow0.
```


Donc $A_n\to2$.

## Exercice 10

Poser $a_n=(1!+\cdots+n!)/n!$. Pour $n\geq2$, les $n-2$ premiers termes sont au plus $(n-2)!$ chacun, donc


```math
1\leq a_n\leq1+\frac1n+\frac{n-2}{n(n-1)}\longrightarrow1.
```


Pour $p=0$, la limite vaut $1$. Pour $p\geq1$,


```math
\frac{1!+\cdots+n!}{(n+p)!}=\frac{a_n}{(n+1)\cdots(n+p)}\longrightarrow0.
```



## Exercice 11

1. 

```math
\frac{n^2}{n^2+n}\leq\sum_{k=1}^n\frac n{n^2+k}\leq\frac{n^2}{n^2+1}.
```


Les deux bornes tendent vers $1$.

2. Pour $x\in\mathbb R$ fixé, $kx-1<\lfloor kx\rfloor\leq kx$. Ainsi


```math
\frac{x(n+1)}{2n}-\frac1n<\frac1{n^2}\sum_{k=1}^n\lfloor kx\rfloor\leq\frac{x(n+1)}{2n},
```


d'où la limite $x/2$.

3. C'est $a_n$ de l'exercice 10; la limite vaut $1$.

## Exercice 12

$0\le1-u_n\le1-u_nv_n\to0$ et $0\le1-v_n\le1-u_nv_n$. Ainsi $u_n\to1$ et $v_n\to1$.

## Exercice 13+

1. 

```math
u_{n+1}-u_n=\frac1{(n+1)!}>0,\qquad v_{n+1}-v_n=-\frac1{n(n+1)(n+1)!}<0.
```


De plus $v_n-u_n=1/(n\,n!)\to0$. Les suites sont adjacentes.

2. Si $e=a/b$ avec $a,b\in\mathbb N^*$, prendre $n\geq\max(b,2)$. Les nombres $n!e$ et $n!u_n$ sont entiers, mais


```math
0<n!(e-u_n)\leq n!(v_n-u_n)=\frac1n<1,
```


contradiction.

## Exercice 14

1. $u_n=\sum_{k=n+1}^{2n}1/k$ et $v_n=u_n+1/n$. De plus


```math
u_{n+1}-u_n=\frac1{2n+1}-\frac1{2n+2}>0,
```




```math
v_{n+1}-v_n=\frac1{2n+1}-\frac1{2n+2}-\frac1{n(n+1)}<0.
```


Enfin $v_n-u_n=1/n\to0$: les suites sont adjacentes.
2. Posons $u_n=\sum_{k=1}^n k^{-1/2}-2\sqrt n$ et $v_n=\sum_{k=1}^n k^{-1/2}-2\sqrt{n+1}$. Alors $u_n-v_n=2(\sqrt{n+1}-\sqrt n)>0$ tend vers $0$. On a


```math
u_{n+1}-u_n=\frac1{\sqrt{n+1}}-\frac2{\sqrt{n+1}+\sqrt n}<0,
```




```math
v_{n+1}-v_n=\frac1{\sqrt{n+1}}-\frac2{\sqrt{n+2}+\sqrt{n+1}}>0.
```


Elles sont adjacentes.

## Exercice 15

La décroissance vers $0$ donne $u_n\geq0$. Poser $S_n=\sum_{k=0}^n(-1)^ku_k$. Alors


```math
S_{2n+2}-S_{2n}=u_{2n+2}-u_{2n+1}\leq0,
```




```math
S_{2n+3}-S_{2n+1}=u_{2n+2}-u_{2n+3}\geq0.
```


Les sommes paires décroissent, les impaires croissent, et


```math
0\leq S_{2n+1}\leq S_{2n}\leq u_0,\qquad S_{2n}-S_{2n+1}=u_{2n+1}\to0.
```


Ces sous-suites sont adjacentes; $(S_n)$ converge vers leur limite commune.

## Exercice 16+

1. Si $u_n\to+\infty$, pour tout $A>0$, choisissons $N$ tel que $u_k\ge2A$ pour $k\ge N$. Alors $C_n\ge n^{-1}\sum_{k<N}u_k+2A(n-N+1)/n$, donc $C_n\to+\infty$. La réciproque est fausse: $u_{2n}=0$, $u_{2n+1}=2n+1$ donne $C_n\to+\infty$ sans que $u_n\to+\infty$.
2. Une suite monotone non convergente tend vers $+\infty$ ou $-\infty$, et ses moyennes ont alors la même limite infinie. Ainsi, si les moyennes convergent dans $\mathbb R$, la suite monotone converge dans $\mathbb R$.
3. Si $|u_n|\le M$, alors $|C_n|\le M$. La réciproque est fausse: $u_n=(-1)^n n$ a des moyennes bornées, mais est non bornée.
4. Si $(u_n)$ croît, $C_n\le u_n\le u_{n+1}$, donc $C_{n+1}-C_n=(u_{n+1}-C_n)/(n+1)\ge0$. La réciproque est fausse : $u_1=0$, $u_2=1$ et $u_n=1/2$ pour tout $n\geq3$ donnent $C_1=0$ et $C_n=1/2$ pour tout $n\geq2$.

## Exercice 17

Soit $\varepsilon>0$ et $N$ tel que $|u_k|\le\varepsilon$ dès que $k\ge N$. Alors


```math
\left|\frac1{n^2}\sum_{k=1}^nku_k\right|\le\frac1{n^2}\sum_{k<N}k|u_k|+\frac{\varepsilon}{n^2}\sum_{k=N}^nk.
```


Le premier terme tend vers $0$ et le second est majoré par $\varepsilon(1+1/n)/2$. La limite est nulle.

## Exercice 18

1. Les rapports étant positifs, leur limite $\ell$ est positive ou nulle. Si $\ell>0$, pour tout $0<\varepsilon<\ell$, à partir d’un rang $N$, $\ell-\varepsilon\le u_{k+1}/u_k\le\ell+\varepsilon$. En multipliant de $N$ à $n-1$ puis en prenant les racines $n$-ièmes, on obtient $\ell-\varepsilon\le\liminf\sqrt[n]{u_n}\le\limsup\sqrt[n]{u_n}\le\ell+\varepsilon$. Si $\ell=0$, on majore de même les rapports par tout $\varepsilon>0$. Dans les deux cas, $\sqrt[n]{u_n}\to\ell$.
2. Pour $a_n=n^n/n!$,


```math
\frac{a_{n+1}}{a_n}=\left(1+\frac1n\right)^n\longrightarrow e.
```


La question 1 donne $n/\sqrt[n]{n!}=\sqrt[n]{a_n}\to e$.
Pour $b_n=\binom{2n}n$,


```math
\frac{b_{n+1}}{b_n}=\frac{(2n+2)(2n+1)}{(n+1)^2}\longrightarrow4,
```


donc $\binom{2n}n^{1/n}\to4$.

## Exercice 19+

Soient $a=\lim u_n$ et $b=\lim v_n$. Les suites sont bornées. Fixons $\varepsilon>0$ et choisissons $N$ tel que $|u_k-a|<\varepsilon$ et $|v_k-b|<\varepsilon$ pour $k\ge N$. Sauf au plus $2N$ termes de bord, les facteurs $u_k,v_{n+1-k}$ sont tous deux à distance $<\varepsilon$ de leurs limites; ainsi $|u_kv_{n+1-k}-ab|\le\varepsilon(|a|+|b|)+\varepsilon^2$. La contribution des termes de bord à la moyenne tend vers $0$ par bornitude. Donc $w_n\to ab$.

## Exercice 20

Une suite convergente d’entiers naturels est de Cauchy. Pour un rang $N$ assez grand, $p,q\ge N$ entraîne $|u_p-u_q|<1$. Comme cette différence est entière, elle est nulle; la suite est stationnaire.

## Exercice 21

1. Si $\ell<1$, choisissons $r$ tel que $\ell<r<1$. À partir d’un rang, $u_{n+1}\le r u_n$, donc $u_n\le u_Nr^{n-N}\to0$.
2. Si $\ell>1$, choisissons $r$ tel que $1<r<\ell$. Alors $u_{n+1}\ge r u_n$ à partir d’un rang, donc $u_n\to+\infty$.
3. Pour $\ell=1$, $u_n=1$ converge, tandis que $u_n=n+1$ diverge vers $+\infty$; les deux ont un quotient de termes successifs tendant vers $1$.

## Exercice 22

Posons $w_n=u_{n+1}+u_n/2$. L’hypothèse donne $w_{n+1}\le w_n$; comme $w_n\ge0$, $w_n$ converge. Posons $\varepsilon_n=w_n-w_{n+1}\ge0$. Alors $\sum_n\varepsilon_n<+\infty$. Pour $d_n=u_{n+1}-u_n$, on a $d_{n+1}=-d_n/2-\varepsilon_n$. Ainsi


```math
|d_{n+1}|\le\frac12|d_n|+\varepsilon_n.
```


En sommant cette inégalité de $n=0$ à $N$, on obtient $\sum_{n=1}^{N+1}|d_n|\le |d_0|+2\sum_{n=0}^N\varepsilon_n$, donc $\sum|d_n|<+\infty$. La suite $(u_n)$ est de Cauchy et converge.

## Exercice 23+

1. Comme $u_n\to+\infty$, il existe $N$ tel que $u_n>u_0$ pour $n\ge N$. Le minimum de $E$ est donc le minimum de l’ensemble fini $\{u_0,\ldots,u_{N-1}\}$.
2. Si $u_n\to\ell$ et tous les termes valent $\ell$, le maximum et le minimum sont atteints. Sinon il existe $j$ tel que $u_j\ne\ell$. Si $u_j>\ell$, le terme $u_j$ dépasse finalement tous les termes de la queue; le maximum est donc atteint parmi un nombre fini de termes. Si $u_j<\ell$, de même le minimum est atteint parmi un nombre fini de termes.

## Exercice 24+

Pour tout $A\in\mathbb N$, il n’y a que $A+1$ entiers naturels $\le A$. Comme les $u_n$ sont deux à deux distincts, au plus $A+1$ indices vérifient $u_n\le A$. Ainsi $u_n\to+\infty$.

## Exercice 25+

1. Écrivons $m=qn+r$, $0\le r<n$. Par sous-additivité, $u_m\le q u_n+u_r$ (avec $u_0=0$ si $r=0$). Pour $r<n$, les valeurs $u_r$ sont bornées par une constante $K_n$. Ainsi


```math
\frac{u_m}{m}\le\frac{q u_n+K_n}{qn+r}\longrightarrow\frac{u_n}{n}
```


quand $m\to\infty$. On obtient finalement $u_m/m\le u_n/n+\delta$ dès $m$ assez grand.
2. Soit $L=\inf_{k\ge1}u_k/k$. On a $u_n/n\ge L$. D’après 1, pour tout $k$ et $\delta>0$, $u_m/m\le u_k/k+\delta$ dès $m$ assez grand. Donc $\limsup u_m/m\le u_k/k+\delta$. En prenant l’infimum en $k$ puis $\delta\downarrow0$, $\limsup u_m/m\le L$, et la limite vaut $L$.

## Autocorrection E

Si une suite est périodique de période $p$ et non constante, elle prend deux valeurs distinctes infiniment souvent. Deux sous-suites constantes distinctes empêchent la convergence.

## Exercice 26

Soit $u_n\to\ell$ et $(-1)^nu_n\to m$. Les sous-suites paires tendent à la fois vers $\ell$ et $m$, donc $m=\ell$; les sous-suites impaires tendent à la fois vers $\ell$ et $-m$, donc $\ell=-m$. Ainsi $\ell=m=0$.

## Exercice 27

Posons $a=\lim u_{2n}$ et $b=\lim u_{2n+1}$. La sous-suite $u_{6n}$ est paire et vaut aussi $u_{3(2n)}$, et $u_{6n+3}$ est impaire et vaut aussi $u_{3(2n+1)}$. Comme $(u_{3n})$ converge, ces deux sous-suites ont la même limite; donc $a=b$. Les parties paire et impaire de $(u_n)$ tendent à la même limite, donc $u_n$ converge.

## Exercice 28

1. Si $u_{\varphi(n)}$ converge vers $\ell$ et $(u_n)$ est croissante, alors pour tout $n$ suffisamment grand, choisir $\varphi(k)\ge n$ donne $u_n\le u_{\varphi(k)}$; l’encadrement par les termes de la sous-suite montre $u_n\to\ell$.
2. Une sous-suite majorée fournit une borne supérieure à tous les termes antérieurs; par croissance, toute la suite est majorée. Une suite croissante majorée converge.

## Exercice 29+

1. Pour $m$ entre $kn$ et $k(n+1)$, $|u_m-u_{kn}|\le k\max_{j\ge kn}|u_{j+1}-u_j|\to0$. Comme $u_{kn}$ converge, $u_m$ converge vers la même limite.
2. Non. $u_n=\sin(2\pi\sqrt n)$ vérifie $u_{n^2}=0$ et $u_{n+1}-u_n\to0$ (théorème des accroissements finis appliqué à $x\mapsto\sin(2\pi\sqrt x)$), mais $(u_n)$ ne converge pas: on peut choisir des entiers proches de $(j+1/4)^2$ et $(j+3/4)^2$ pour obtenir des sous-suites tendant vers $1$ et $-1$.

## Exercice 30+

Soient $a<b$ deux valeurs d’adhérence et $c\in(a,b)$. Choisissons $n_j<m_j$ tels que $u_{n_j}\to a$ et $u_{m_j}\to b$. Entre ces indices, soit $k_j$ le premier indice pour lequel $u_{k_j}\ge c$. Alors $u_{k_j-1}<c\le u_{k_j}$ et $|u_{k_j}-u_{k_j-1}|\to0$; donc $u_{k_j}\to c$. Toute valeur entre deux valeurs d’adhérence est une valeur d’adhérence.

## Exercice 31+

Si $|q_n|$ ne tendait pas vers l’infini, une sous-suite aurait $q_n=q$ fixé non nul (un dénominateur nul est impossible), et alors $p_n/q$ convergerait vers l’irrationnel $\ell$. Les entiers $p_n$ devraient être stationnaires le long d’une sous-suite, ce qui rendrait cette limite rationnelle. Contradiction. Ainsi $|q_n|\to\infty$. Comme $p_n/q_n\to\ell\notin\mathbb Q$, en particulier $\ell\ne0$; donc $|p_n|=|q_n||p_n/q_n|\to\infty$.

## Exercice 32++

Par Cesàro appliqué aux différences, $u_n/n\to0$. Choisir $N$ tel que $|u_{j+1}-u_j|<1$ et $u_j<j/2$ pour $j\geq N$, puis un entier $K>N$ supérieur à $u_0,\ldots,u_N$.

Pour chaque entier $m\geq K$, poser $\varphi(m)=\min\{j:u_j\geq m\}$. Cet indice existe, et $\varphi(m)>m\geq N$. Par minimalité,


```math
u_{\varphi(m)-1}<m\leq u_{\varphi(m)}<m+1.
```


Il en résulte $\varphi(m+1)>\varphi(m)$ et


```math
0\leq u_{\varphi(m)}-m\leq|u_{\varphi(m)}-u_{\varphi(m)-1}|\longrightarrow0.
```


Définir $\varphi(m)=m$ pour $m<K$ complète cette extraction sans changer la limite.

## Exercice 33

1. Si $E$ est infini, énumérons ses éléments $n_0<n_1<\cdots$. Par définition de $E$, $u_{n_{j+1}}<u_{n_j}$; on obtient une sous-suite strictement décroissante.
2. Si $E$ est fini, choisissons $n_0$ au-delà de $E$. Comme $n_0\notin E$, il existe $n_1>n_0$ tel que $u_{n_1}\ge u_{n_0}$. Puis, puisque $n_1\notin E$, choisissons $n_2>n_1$ avec $u_{n_2}\ge u_{n_1}$, et poursuivons. Cela donne une sous-suite croissante.
3. Une suite bornée possède, d’après 1 ou 2, une sous-suite monotone; cette sous-suite est bornée, donc convergente.

## Exercice 34+

Oui : prendre $k=1$ dans l'hypothèse donne directement la convergence de $(u_n)$. L'indice imprimé est $kn$.

## Exercice 35+

1. $e^{a_n}+e^{b_n}\to2$ implique que les deux suites sont majorées. Comme $a_n+b_n\to0$, elles sont aussi minorées. Pour toute valeur d’adhérence $a$ de $(a_n)$, une sous-suite donne $b_n\to-a$ et $e^a+e^{-a}=2$. Or $e^a+e^{-a}\ge2$, avec égalité seulement pour $a=0$. Ainsi toutes les valeurs d’adhérence de $(a_n)$ sont nulles; $a_n\to0$, puis $b_n\to0$.
2. Oui. Les trois suites sont bornées: chacune est majorée par la convergence de la somme des exponentielles; la somme linéaire tendant vers zéro fournit leurs minorations. Pour toute sous-suite convergente du triplet, sa limite $(a,b,c)$ vérifie $a+b+c=0$ et $e^a+e^b+e^c=3$. L’inégalité de convexité stricte donne


```math
\frac{e^a+e^b+e^c}{3}\ge e^{(a+b+c)/3}=1,
```


avec égalité seulement si $a=b=c$. Il s’ensuit $a=b=c=0$. Tout point d’adhérence étant $(0,0,0)$, les trois suites convergent vers $0$.

## Exercice 36+

Soient $m=\liminf u_n$ et $M=\limsup u_n$. L’égalité $u_n+u_{2n}/2\to1$ entraîne, en utilisant $m\le\liminf u_{2n}\le\limsup u_{2n}\le M$,


```math
M\le1-\frac m2,\qquad m\ge1-\frac M2.
```


Donc $M-m\le(M-m)/2$, d’où $M=m$. La suite converge vers $\ell$ et $\ell+\ell/2=1$, donc $\ell=2/3$.

## Exercice 37+++

1. Poser $y_n=x_n(1-x_{n+1})\in(0,1)$. Si $\liminf y_n>1/4$, choisir $c>1/4$ tel que $y_n\geq c$ à partir d'un rang. Alors


```math
x_n\geq c,\qquad x_{n+1}\leq1-\frac c{x_n}<x_n,
```


la dernière inégalité venant de $x_n(1-x_n)\leq1/4<c$. La suite finirait par décroître vers $L\geq c$, avec $L(1-L)\geq c>1/4$, impossible. Ainsi $\liminf y_n\leq1/4$. La suite $(y_n)$ étant bornée, son infimum limite est une valeur d'adhérence.

2. L'hypothèse donne $\liminf y_n\geq1/4$. Fixer $c\in(0,1/4)$ et $N$ tel que $y_n\geq c$ pour $n\geq N$. Poser


```math
r_\pm=\frac{1\pm\sqrt{1-4c}}2,\qquad F_c(t)=1-\frac ct.
```


On a $x_n>c$ et $x_{n+1}\leq F_c(x_n)$ sur cette queue.

Si $x_j<r_-$ pour un $j\geq N$, alors $F_c(x_j)<x_j$, et cette inégalité se propage : $(x_n)_{n\geq j}$ décroît, reste $>c$ et converge vers $L<r_-$. Mais $L\leq F_c(L)$ impose $L(1-L)\geq c$, donc $L\in[r_-,r_+]$, contradiction. Ainsi $x_n\geq r_-$ pour $n\geq N$.

Pour $M=\limsup x_n>0$, la croissance et la continuité de $F_c$ donnent $M\leq F_c(M)$, donc $M\leq r_+$. Par conséquent


```math
r_-\leq\liminf x_n\leq\limsup x_n\leq r_+.
```


Faire tendre $c$ vers $1/4$ : $x_n\to1/2$.

## Exercice 38

1. Par définition de $\ell=\limsup u_n$, la queue supérieure $\sup_{k\ge n}u_k$ tend vers $\ell$. Elle est donc inférieure à $\ell+\varepsilon$ pour tout $n$ assez grand, ce qui prouve (a). Elle est supérieure à $\ell-\varepsilon$ pour tout $n$; chaque queue contient donc un terme au moins $\ell-\varepsilon$, ce qui prouve (b).
2. L’ensemble $\{n:u_n\ge\ell\}$ peut être fini ou infini. Par exemple $u_n=\ell-1/(n+1)$ donne l’ensemble vide, tandis que $u_n=\ell$ donne tous les indices.

## Exercice 39

1. La conjecture des nombres premiers jumeaux affirme qu’il existe une infinité de premiers consécutifs distants de $2$; comme tous les écarts sont des entiers pairs positifs, elle équivaut à $\liminf(p_{n+1}-p_n)=2$.
2. $\limsup(p_{n+1}-p_n)=+\infty$. Pour chaque $m$, le nombre $N=(m+1)!+2$ et les $m$ entiers consécutifs $N,N+1,\ldots,N+m-1$ sont composés; il existe donc des écarts entre nombres premiers consécutifs arbitrairement grands.

## Exercice 40

1. Si $u_n\to\ell$, pour $\varepsilon>0$ on a $|u_p-u_q|\le|u_p-\ell|+|u_q-\ell|<\varepsilon$ dès que $p,q$ sont assez grands.
2. (a) En prenant $\varepsilon=1$, la propriété de Cauchy borne la queue à distance $1$ d’un terme fixé; avec le préfixe fini, la suite est bornée.
(b) Posons $a=\liminf u_n$ et $b=\limsup u_n$. Pour tout $\varepsilon>0$, il existe $N$ tel que $|u_p-u_q|\le\varepsilon$ pour $p,q\ge N$. Les infimums et supremums des queues vérifient donc $\sup_{p\ge N}u_p-\inf_{q\ge N}u_q\le\varepsilon$. En passant aux limites, $b-a\le\varepsilon$, donc $a=b$.
(c) Si $a=b=\ell$, la suite bornée a liminf et limsup égaux à $\ell$, ce qui équivaut à $u_n\to\ell$.

## Exercice 41+

Pour chaque $x\in\mathbb R$ et chaque $j\geq1$, l'intervalle $]x-1/j,x+1/j[$ contient une infinité de rationnels. Une infinité d'indices y sont donc envoyés par $\varphi$. Choisir successivement $n_j>n_{j-1}$ tel que $|\varphi(n_j)-x|<1/j$. Alors $\varphi(n_j)\to x$. L'ensemble des valeurs d'adhérence réelles est $\mathbb R$.

## Exercice 42+

Soit $x\ge0$ et $\varepsilon>0$. Choisissons $N$ tel que $u_n<\varepsilon$ pour $n\ge N$. En parcourant les termes à partir de $N$, ajoutons $u_n$ à une somme partielle tant que cela ne dépasse pas $x$. Les sommes restent $\le x$; elles finissent par dépasser $x-\varepsilon$, car la série diverge et chaque terme ajouté est inférieur à $\varepsilon$. Cette somme est une somme sur un ensemble fini d’indices, à distance au plus $\varepsilon$ de $x$. L’ensemble des sommes finies est dense dans $\mathbb R_+$.

## Exercice 43+

Fixer $x\in\mathbb R$ et $\varepsilon>0$. Choisir $N$ tel que $|v_{m+1}-v_m|<\varepsilon$ pour $m\geq N$, puis $n$ tel que $u_n-x>\max(v_0,\ldots,v_{N+1})$. Soit $m$ le premier indice tel que $v_m\geq u_n-x$. Alors $m>N+1$ et


```math
v_{m-1}<u_n-x\leq v_m,\qquad0\leq x-(u_n-v_m)<v_m-v_{m-1}<\varepsilon.
```


Les différences sont donc denses dans $\mathbb R$.

## Exercice 44

Écrivons $z_n=a_n+ib_n$. La relation donne $a_{n+1}=2a_n$ et $b_{n+1}=4b_n$. Ainsi $z_n=2^n\operatorname{Re}(z_0)+i4^n\operatorname{Im}(z_0)$.

## Exercice 45

L'égalité imprimée $z_n=\frac14z_n+\frac34\overline{z_n}$ équivaut à $z_n=\overline{z_n}$ : tous les termes sont réels. Elle n'impose aucune convergence ($z_n=0$ converge, $z_n=n$ diverge).

Avec la récurrence $z_{n+1}=\frac14z_n+\frac34\overline{z_n}$, écrire $z_n=a_n+ib_n$ donne $a_{n+1}=a_n$ et $b_{n+1}=-b_n/2$, donc


```math
z_n=\operatorname{Re}z_0+i(-1/2)^n\operatorname{Im}z_0\longrightarrow\operatorname{Re}z_0.
```



## Exercice 46

Pour $\theta=\pi$, $\sin(n\theta)=0$ converge et $\cos(n\theta)=(-1)^n$ diverge : l'énoncé est faux pour $\theta\in\pi\mathbb Z\setminus2\pi\mathbb Z$.

Si $\theta\notin\pi\mathbb Z$, les formules d'addition donnent


```math
v_n=\frac{\cos\theta\,u_n-u_{n+1}}{\sin\theta},\qquad u_n=\frac{v_{n+1}-\cos\theta\,v_n}{\sin\theta}.
```


La convergence de l'une des suites entraîne donc celle de l'autre. Si elles convergeaient, $e^{in\theta}=u_n+iv_n$ aurait une limite $z$ de module $1$. Passer à la limite dans $e^{i(n+1)\theta}=e^{i\theta}e^{in\theta}$ donnerait $z=e^{i\theta}z$, donc $e^{i\theta}=1$, contradiction. Elles divergent toutes deux dans ce cas.

## Exercice 47+

Par récurrence sur $n$, l’identité remarquable donne


```math
\prod_{k=0}^n(1+z^{2^k})=\frac{1-z^{2^{n+1}}}{1-z}.
```


Comme $|z|<1$, le numérateur tend vers $1$ et le dénominateur est non nul; la limite vaut $1/(1-z)$.

## Autocorrection F

On a $u_{n+1}-u_n=e^{-u_n}>0$, donc $(u_n)$ croît. Si elle était majorée, elle convergerait vers un réel $L$, et la relation donnerait $e^{-L}=0$, impossible. Donc $u_n\to+\infty$.

## Autocorrection G

La relation se factorise $u_{n+1}=u_n(1+u_n)$. Or $u_0=-1/2$, $u_1=-1/4$, $u_2=-3/16$; pour $-1/2<u_n<0$, $u_n<u_{n+1}<0$. La suite croît et est majorée par $0$; sa limite $L$ vérifie $L=L+L^2$, donc $L=0$.

## Exercice 48

Ici $u_0=1/2$ et $u_{n+1}=(u_n^2+u_n)/2$. Si $0<u_n<1$, alors $0<u_{n+1}<u_n$. La suite décroît vers $L\ge0$; la relation donne $L=(L^2+L)/2$, donc $L=0$.

## Exercice 49

1. $f(x)=\frac12(x+a/x)$ et $f'(x)=\frac12(1-a/x^2)$. Elle décroît sur $]0,\sqrt a]$, croît sur $[\sqrt a,+\infty[$ et atteint $\sqrt a$. Pour $x\ge\sqrt a$, $f(x)\le x$ équivaut à $a/x\le x$.
2. $u_1=f(u_0)\ge\sqrt a$ par $x+a/x\ge2\sqrt a$. Puis, si $u_n\ge\sqrt a$, $u_{n+1}=f(u_n)\ge\sqrt a$ et $u_{n+1}\le u_n$.
3. $(u_n)_{n\ge1}$ décroît et est minorée par $\sqrt a$, donc converge vers $L\ge\sqrt a$. Le passage à la limite donne $L=(L+a/L)/2$, donc $L=\sqrt a$.

## Exercice 50

La récurrence est $u_{n+1}=e\ln(u_n)$; elle exige $u_n>0$. La fonction $f(x)=e\ln x-x$ vérifie $f' (x)=e/x-1$ et atteint son maximum $0$ en $x=e$; ainsi $e\ln x\le x$, avec égalité seulement en $e$.
1. Si $u_0\ge e$, alors $u_{n+1}\ge e$ et $u_{n+1}\le u_n$. La suite converge vers $L\ge e$ vérifiant $L=e\ln L$; l’égalité n’est possible que pour $L=e$. Donc $u_n\to e$.
2. Si $u_0\le0$, la suite n’est pas définie. Si $0<u_0<e$, tant que tous les termes restent positifs, ils décroissent strictement. S’ils restaient positifs pour tout $n$, ils convergeraient vers un $L\ge0$; $L=0$ entraînerait $e\ln u_n\to-\infty$, incompatible avec $u_{n+1}>0$. Ainsi $L>0$, et $L=e\ln L$ imposerait $L=e$, impossible puisque $u_n\le u_0<e$. Le processus finit donc par atteindre un terme non positif, après quoi la suite réelle n’est plus définie.

## Exercice 51

1. Il faut et il suffit que $u_0\in[-2,2]$: si $u_0<-2$, alors $u_1>2$ et $u_2$ n’est pas défini; si $-2\le u_0\le2$, alors $u_1\in[0,2]$ et tous les termes suivants restent dans $[0,\sqrt2]\subset[0,2]$.
2. À partir de $n=2$, $u_n\in[0,\sqrt2]$. Sur cet intervalle, $|f'(x)|=1/(2\sqrt{2-x})\le1/(2\sqrt{2-\sqrt2})<1$. Comme $f(1)=1$, le théorème des accroissements finis donne $|u_{n+1}-1|\le q|u_n-1|$ pour $n\ge2$, avec $q<1$. Donc $u_n\to1$.

## Exercice 52

$u_0=1$ et $u_{n+1}=1+2/u_n$. Les termes restent dans $[1,3]$. L’application $f(x)=1+2/x$ est décroissante, et


```math
f(f(x))-x=\frac{(2-x)(x+1)}{x+2}.
```


Les termes pairs croissent et restent dans $[1,3]$; les termes impairs décroissent et restent dans $[1,3]$. Leurs limites sont des points fixes de $f\circ f$, donc des solutions de $(2-x)(x+1)=0$. Dans $[1,3]$, seule $x=2$ convient; les deux sous-suites et donc $(u_n)$ tendent vers $2$.

## Exercice 53

Posons $x_n=a_{2n}$. Alors $a_{2n+1}=x_n/2$ et $x_{n+1}=1+x_n/2$. La récurrence affine donne $x_n=2-2^{-n}(2-x_0)\to2$; donc $a_{2n+1}\to1$. Les valeurs d’adhérence sont $1$ et $2$.

## Exercice 54

Pour $u_n\geq v_n>0$, l'inégalité arithmético-géométrique donne


```math
v_n\leq\sqrt{u_nv_n}=v_{n+1}\leq u_{n+1}=\frac{u_n+v_n}2\leq u_n.
```


Cette propriété, vraie au rang $0$, se propage. Les suites sont donc bien définies; $(u_n)$ décroît, $(v_n)$ croît, et toutes deux restent dans $[b,a]$. Si leurs limites sont $U,V$, la relation $u_{n+1}=(u_n+v_n)/2$ donne $U=(U+V)/2$, donc $U=V$. Elles sont adjacentes.

## Exercice 55

Pour $u_n\ge v_n>0$, $u_{n+1}=(u_n+v_n)/2$ et $v_{n+1}=2u_nv_n/(u_n+v_n)$ sont positifs et


```math
v_{n+1}\le u_{n+1},\qquad u_{n+1}-v_{n+1}=\frac{(u_n-v_n)^2}{2(u_n+v_n)}\ge0.
```


Ainsi $u_n$ décroît, $v_n$ croît; elles sont encadrées par $1$ et $x$, donc convergent. La relation $u_{n+1}=(u_n+v_n)/2$ impose l'égalité de leurs limites, notée $L>0$. La quantité $u_nv_n$ est constante, puisque $u_{n+1}v_{n+1}=u_nv_n=x$; alors $L^2=x$, et $L=\sqrt x$.

## Exercice 56

1. $F_n(x)=x+x^2+\cdots+x^n$ est continue strictement croissante sur $\mathbb R_+$, avec $F_n(0)=0$ et $F_n(1)=n\ge1$; l’équation $F_n(x)=1$ a une unique solution $x_n\in(0,1]$.
2. $F_n(1/2)=1-2^{-n}<1$, donc $x_n>1/2$; et $F_n(1)=n\ge1$, donc $x_n\le1$.
3. $F_{n+1}(x_n)=1+x_n^{n+1}>1=F_{n+1}(x_{n+1})$, donc $x_{n+1}<x_n$.
4. La suite décroissante est minorée par $1/2$, donc tend vers $L\ge1/2$. Pour tout entier fixé $p$ et tout $n\geq p$, $1\ge x_n+x_n^2+\cdots+x_n^p$, d’où $1\ge L+L^2+\cdots+L^p$. Pour $L>1/2$, cette somme dépasse $1$ pour $p$ assez grand, contradiction. Donc $L=1/2$.

## Exercice 57

1. $f_n(x)=x^5+nx-1$ est continue strictement croissante, $f_n(0)=-1$ et $f_n(1/n)=n^{-5}>0$; elle a un unique zéro $u_n\in(0,1/n)$.
2. $f_{n+1}(u_n)=u_n^5+(n+1)u_n-1=f_n(u_n)+u_n=u_n>0$. Comme $f_{n+1}$ croît et s’annule en $u_{n+1}$, $u_{n+1}<u_n$.
3. La suite décroît et est minorée par $0$, donc tend vers $L\ge0$. Or $u_n<1/n$, donc $L=0$.

## Exercice 58

1. $f(x)=x+\ln x$ est continue strictement croissante sur $]0,+\infty[$ et tend vers $-\infty$ en $0^+$, vers $+\infty$ en $+\infty$; chaque équation $f(x)=n$ a une unique solution $u_n>0$.
2. Comme $f$ croît, $n+1>n$ entraîne $u_{n+1}>u_n$. Si $(u_n)$ était majorée, elle convergerait vers un $L>0$, mais $u_n+\ln u_n=n$ est non borné. Ainsi $u_n\to+\infty$.
