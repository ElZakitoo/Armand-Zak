# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td10-groupes.pdf)

## Autocorrection A



```math
1\in M^\times,\qquad a,b\in M^\times\Rightarrow(ab)(b^{-1}a^{-1})=(b^{-1}a^{-1})(ab)=1.
```




```math
a^{-1}\in M^\times,\qquad(a^{-1})^{-1}=a.
```


L'associativité est celle de $M$.

## Exercice 1

### 1

$e$ neutre de $*$, $u$ neutre de $\otimes$.


```math
e=(e\otimes u)*(u\otimes e)=(e*u)\otimes(u*e)=u\otimes u=u.
```



### 2



```math
a*b=(a\otimes e)*(e\otimes b)=(a*e)\otimes(e*b)=a\otimes b.
```



### 3



```math
a*b=(e\otimes a)*(b\otimes e)=(e*b)\otimes(a*e)=b\otimes a=b*a.
```




```math
(a*b)*c=(a\otimes b)*(e\otimes c)=(a*e)\otimes(b*c)=a*(b*c).
```



## Exercice 2



```math
a,b\in A,\quad y,z\in E,
```




```math
(a*b)*(y*z)=a*(b*(y*z))=a*((b*y)*z)=(a*(b*y))*z=((a*b)*y)*z.
```




```math
a*b\in A,\qquad a,b,c\in A\Rightarrow a*(b*c)=(a*b)*c.
```



## Exercice 3

L'assertion est fausse pour un magma quelconque.


```math
E=\{0,1\},\qquad x*y=x.
```




```math
\sigma(x*y)=\sigma(x)=\sigma(x)*\sigma(y)\qquad(\forall\sigma\in\mathfrak S(E)),
```




```math
|E|=2\notin\{0,1,3\}.
```


La même loi convient sur tout ensemble, notamment de cardinal $0$, $1$ ou $3$.

## Exercice 4



```math
xy=1,\quad yz=1\Rightarrow x=x(yz)=(xy)z=z\Rightarrow yx=yz=1.
```




```math
\forall x,\quad\exists y,\quad xy=yx=1.
```



## Exercice 5

### 1



```math
x\circ y=yx,\qquad(x\circ y)\circ z=z(yx)=(zy)x=x\circ(y\circ z).
```




```math
1\circ x=x\circ1=x.
```



### 2



```math
M=\{1,a,b\},\quad1x=x1=x,\quad ax=a,\quad bx=b\quad(x\in M).
```




```math
x\ne1\Rightarrow(xy)z=xz=x=x(yz);\qquad x=1\Rightarrow(xy)z=y z=x(yz).
```




```math
\#\{z:\forall x,\ zx=z\}=2,\qquad\#\{z:\forall x,\ xz=z\}=0.
```


Un isomorphisme avec le monoïde opposé échangerait ces deux ensembles : impossible.

### 3



```math
x\circ x^{-1}=x^{-1}x=1=x^{-1}\circ x.
```




```math
\varphi(x)=x^{-1},\qquad\varphi(xy)=y^{-1}x^{-1}=\varphi(x)\circ\varphi(y),\qquad\varphi^2=\operatorname{id}.
```



## Autocorrection B

### (i)



```math
\ell(uv)=\ell(u)+\ell(v),\quad\ell(u)>0\Rightarrow uv\ne\varnothing.
```


Pas un groupe.

### (ii)



```math
0M=0\ne I_2.
```


Pas un groupe.

### (iii)



```math
\det(AB)=\det A\det B,\qquad\begin{pmatrix}a&b\\c&d\end{pmatrix}^{-1}=\begin{pmatrix}d&-b\\-c&a\end{pmatrix}\quad(ad-bc=1).
```




```math
U=\begin{pmatrix}1&1\\0&1\end{pmatrix},\quad V=\begin{pmatrix}1&0\\1&1\end{pmatrix},\quad UV=\begin{pmatrix}2&1\\1&1\end{pmatrix}\ne\begin{pmatrix}1&1\\1&2\end{pmatrix}=VU.
```


Groupe non abélien.

### (iv)



```math
U(x)U(y)=U(x+y),\qquad U(0)=I_2,\quad U(x)^{-1}=U(-x).
```


Groupe abélien, isomorphe à $(\mathbb R,+)$.

### (v)



```math
e\in\mathbb R,\quad x=e-1\Rightarrow\max(e,x)=e\ne x.
```


Aucun neutre.

### (vi)



```math
z^n=w^m=1\Rightarrow(zw)^{nm}=1,\quad(z^{-1})^n=1.
```


Sous-groupe du groupe abélien $\mathbb C^\times$.

## Exercice 6



```math
z=xy\Rightarrow z^2=xyxy=y^4\Rightarrow zy^4=y^4z.
```




```math
y^5=1\Rightarrow(y^4)^4=y^{16}=y\Rightarrow zy=yz.
```




```math
x=zy^{-1}\Rightarrow xy=yx,\qquad x^2y=xyx=y^3\Rightarrow\boxed{x^2=y^2.}
```



## Exercice 7



```math
g^2=1\Rightarrow g^{-1}=g,\qquad xy=(xy)^{-1}=y^{-1}x^{-1}=yx.
```



## Exercice 8



```math
\mathbf1_{A\triangle B}=\mathbf1_A+\mathbf1_B\pmod2.
```




```math
\mathbf1_{(A\triangle B)\triangle C}=\mathbf1_A+\mathbf1_B+\mathbf1_C=\mathbf1_{A\triangle(B\triangle C)}.
```




```math
A\triangle\varnothing=A,\quad A\triangle A=\varnothing,\quad A\triangle B=B\triangle A.
```



## Autocorrection C



```math
H=\bigcup_{n\ge0}H_n,\quad1\in H_0\subset H.
```




```math
x\in H_p,\ y\in H_q\Rightarrow x,y\in H_{\max(p,q)}\Rightarrow xy^{-1}\in H.
```



## Autocorrection D

### 1(a)



```math
1\in C_G(g),\qquad gx=xg,\ gy=yg\Rightarrow gxy^{-1}=xgy^{-1}=xy^{-1}g.
```



### 1(b)



```math
h\in C_G(g)\iff gh=hg\iff\varphi(g)\varphi(h)=\varphi(h)\varphi(g).
```




```math
\varphi\text{ bijective}\Rightarrow\varphi(C_G(g))=C_G(\varphi(g)).
```



### 2(a)



```math
Z(G)=\bigcap_{g\in G}C_G(g)\le G.
```



### 2(b)



```math
\varphi(Z(G))=\bigcap_{g\in G}\varphi(C_G(g))=\bigcap_{g\in G}C_G(\varphi(g))=Z(G).
```



## Exercice 9

### 1



```math
0\in\operatorname{Pér}(f),\quad S,T\in\operatorname{Pér}(f)\Rightarrow f(x+S-T)=f(x-T)=f(x).
```



### 2



```math
f=\mathbf1_G,\quad T\in G\Rightarrow(x+T\in G\iff x\in G)\Rightarrow T\in\operatorname{Pér}(f).
```




```math
T\in\operatorname{Pér}(f)\Rightarrow f(T)=f(0)=1\Rightarrow T\in G.
```



## Exercice 10

### 1



```math
H_1\subseteq H_2\Rightarrow H_1\cup H_2=H_2\le G.
```




```math
a\in H_1\setminus H_2,\ b\in H_2\setminus H_1:\quad ab\in H_1\Rightarrow b\in H_1,\quad ab\in H_2\Rightarrow a\in H_2.
```




```math
ab\notin H_1\cup H_2\Rightarrow H_1\cup H_2\text{ non stable}.
```



### 2

Si $H_1,H_2$ étaient tous deux stricts et $G=H_1\cup H_2$, ils ne peuvent être
inclus l'un dans l'autre, car alors leur union serait le plus grand, encore strict.
Prenons donc $a\in H_1\setminus H_2$ et $b\in H_2\setminus H_1$. Alors $ab$ n'appartient ni à $H_1$
(sinon $b=a^{-1}(ab)\in H_1$) ni à $H_2$ (sinon $a=(ab)b^{-1}\in H_2$), contradiction.
Ainsi $G=H_1$ ou $G=H_2$.

### 3



```math
\mathbb F_2^2=\{0,(1,0)\}\cup\{0,(0,1)\}\cup\{0,(1,1)\}.
```



## Exercice 11



```math
g\text{ d'ordre infini}\Rightarrow\langle g\rangle\supsetneq\langle g^2\rangle\supsetneq\langle g^4\rangle\supsetneq\cdots,
```


impossible. Tous les sous-groupes cycliques sont finis.


```math
\{\langle g\rangle:g\in G\}=\{C_1,\ldots,C_r\}\Rightarrow G=\bigcup_{i=1}^rC_i\text{ fini}.
```



## Exercice 12

### 1



```math
f(a)?f(b)=f(a*b),\qquad(f(a)?f(b))?f(c)=f((a*b)*c)=f(a*(b*c))=f(a)?(f(b)?f(c)).
```




```math
e_E=f(e_G),\qquad f(a)^{-1}=f(a^{-1}).
```



### 2



```math
|E|=n\ge1\Rightarrow E\simeq\mathbb Z/n\mathbb Z\text{ par transport de structure}.
```




```math
E=\varnothing\Rightarrow\text{aucun neutre}.
```



### 3



```math
f(t)=\frac{e^{2t}-1}{e^{2t}+1},\qquad f^{-1}(x)=\frac12\ln\frac{1+x}{1-x}.
```




```math
f:\mathbb R\xrightarrow{\sim}(-1,1),\qquad f(s+t)=\frac{f(s)+f(t)}{1+f(s)f(t)}.
```




```math
e=0,\qquad x^{-1}=-x.
```



## Exercice 13

### 1



```math
(xy)^2=x^2y^2\iff xyxy=xxyy\iff yx=xy.
```



### 2



```math
s(x)=x^2,\quad\ker s=\{x:x^2=1\},\qquad\operatorname{ord}(x)\mid2,|G|\Rightarrow x=1.
```




```math
s\text{ injective},\ G\text{ fini}\Rightarrow s\text{ surjective}.
```



### 3



```math
m=|G|\text{ impair},\quad y^m=1,\qquad x=y^{(m+1)/2}\Rightarrow x^2=y^{m+1}=y.
```



## Exercice 14



```math
\varphi(x_1,x_2)\varphi(y_1,y_2)=x_1x_2y_1y_2=x_1y_1x_2y_2=\varphi(x_1y_1,x_2y_2).
```




```math
x_1x_2=1\Rightarrow x_1=x_2^{-1}\in H_1\cap H_2=\{1\}\Rightarrow\ker\varphi=\{(1,1)\}.
```




```math
\operatorname{Im}\varphi\le G,\qquad H_1\cup H_2\subset\operatorname{Im}\varphi\Rightarrow\operatorname{Im}\varphi=G.
```



## Exercice 15



```math
(-1)^2=1,\quad-1\ne1;\qquad2x=0\Rightarrow x=0\text{ dans }\mathbb R.
```


Les éléments d'ordre $2$ sont préservés par isomorphisme.

## Exercice 16



```math
\Phi(z)=\left(\frac z{|z|},\ln|z|\right),\qquad\Phi^{-1}(u,t)=ue^t.
```




```math
\Phi(zw)=\left(\frac z{|z|}\frac w{|w|},\ln|z|+\ln|w|\right)=\Phi(z)\Phi(w).
```



## Exercice 17

### 1



```math
n\ge1,\quad\varphi:\mathbb Z/n\mathbb Z\to\mathbb Z\Rightarrow n\varphi(\overline1)=\varphi(\overline0)=0\Rightarrow\varphi=0.
```



### 2



```math
q\in\mathbb Q,\quad k\ge1:\quad\varphi(q)=k\varphi(q/k)\in k\mathbb Z.
```




```math
\bigcap_{k\ge1}k\mathbb Z=\{0\}\Rightarrow\varphi=0.
```



## Exercice 18



```math
m=|F|,\qquad\varphi(q)=\varphi(q/m)^m=1_F.
```



## Exercice 19

### 1



```math
\varphi:\mathbb Z^n\to F\Rightarrow\varphi(k_1,\ldots,k_n)=\varphi(e_1)^{k_1}\cdots\varphi(e_n)^{k_n}.
```




```math
\varphi\mapsto(\varphi(e_1),\ldots,\varphi(e_n))\text{ injective}\Rightarrow|\operatorname{Hom}(\mathbb Z^n,F)|\le|F|^n.
```



### 2



```math
a\in\mathbb F_2^n,\qquad\varphi_a(k)=\sum_{j=1}^na_jk_j\pmod2.
```




```math
\boxed{|\operatorname{Hom}(\mathbb Z^n,\mathbb F_2)|=2^n.}
```



### 3



```math
\mathbb Z^n\simeq\mathbb Z^m\Rightarrow2^n=2^m\Rightarrow n=m.
```


La réciproque est immédiate.

## Exercice 20



```math
\sigma_g\sigma_h=\sigma_{gh},\qquad\sigma_g^{-1}=\sigma_{g^{-1}}.
```




```math
\sigma_g=\sigma_h\Rightarrow g=\sigma_g(1)=\sigma_h(1)=h.
```



## Autocorrection E



```math
\zeta=e^{2i\pi/12},\quad i=\zeta^3,\quad j=\zeta^4,\quad i^{-1}j=\zeta.
```




```math
\boxed{\langle i,j\rangle=\langle\zeta\rangle=\mathbb U_{12}.}
```



## Autocorrection F



```math
\text{1.}\quad(x^{-1})^k=1\iff x^k=1.
```




```math
\text{2.}\quad(yxy^{-1})^k=yx^ky^{-1}=1\iff x^k=1.
```




```math
\text{3.}\quad yx=x^{-1}(xy)x\Rightarrow\operatorname{ord}(yx)=\operatorname{ord}(xy).
```



## Exercice 21

### 1



```math
G=\langle S\rangle,\quad|S|=r<\infty,\quad T=S\cup S^{-1},\quad A_n=\{t_1\cdots t_k:0\le k\le n,\ t_i\in T\}.
```




```math
|A_n|\le\sum_{k=0}^n(2r)^k<\infty,\qquad A_n\subseteq A_{n+1},\qquad G=\bigcup_{n\ge0}A_n.
```



### 2



```math
q_i=a_i/b_i,\quad D=\prod_{i=1}^r b_i\ne0\Rightarrow\langle q_1,\ldots,q_r\rangle\subseteq D^{-1}\mathbb Z.
```




```math
1/(2D)\notin D^{-1}\mathbb Z\Rightarrow\mathbb Q\text{ n'est pas de type fini}.
```



## Exercice 22



```math
x\ne1\Rightarrow\langle x\rangle=G.
```




```math
\operatorname{ord}(x)=\infty\Rightarrow\{1\}\subsetneq\langle x^2\rangle\subsetneq G,\quad\bot.
```




```math
|G|=n,\quad n\text{ composé}\Rightarrow\exists p\text{ premier},\quad1<p<n,\quad p\mid n.
```




```math
|\langle x^p\rangle|=n/p\in\{2,\ldots,n-1\},\quad\bot.
```




```math
\boxed{G\simeq\mathbb Z/p\mathbb Z\quad(p\text{ premier}).}
```



## Exercice 23



```math
M\subseteq G,\quad1\in M,\quad MM\subseteq M.
```




```math
x\in M,\quad d=\operatorname{ord}(x)<\infty\Rightarrow x^{-1}=x^{d-1}\in M.
```



## Exercice 24

### 1



```math
x\ne1,\quad\operatorname{ord}(x)\mid p\Rightarrow\operatorname{ord}(x)=p\Rightarrow G=\langle x\rangle.
```



### 2



```math
|G|=4:\quad\exists x,\ \operatorname{ord}(x)=4\Rightarrow G\simeq C_4.
```




```math
\text{Sinon, }x^2=1\ (\forall x),\quad G\text{ abélien},\quad a,b\ne1,\ a\ne b\Rightarrow G=\{1,a,b,ab\}\simeq C_2^2.
```




```math
|G|=6:\quad\text{l'involution }x\mapsto x^{-1}\text{ possède un nombre pair de points fixes}.
```




```math
1\text{ est fixe}\Rightarrow\exists b\ne1,\quad b^2=1.
```




```math
\forall x\ne1,\ \operatorname{ord}(x)=2\Rightarrow G\text{ abélien}\Rightarrow\exists H\simeq C_2^2\le G,\quad4\mid6,\quad\bot.
```




```math
\exists a,\quad\operatorname{ord}(a)\in\{3,6\}.
```




```math
\operatorname{ord}(a)=6\Rightarrow G\simeq C_6.
```




```math
\operatorname{ord}(a)=3:\quad H=\langle a\rangle,\quad G=H\sqcup bH=H\sqcup Hb,\quad bab^{-1}\in\{a,a^{-1}\}.
```




```math
bab^{-1}=a\Rightarrow G\text{ abélien}.\quad\operatorname{ord}(b)\in\{2,6\}.
```


Si $\operatorname{ord}(b)=6$, alors $G\simeq C_6$; si $\operatorname{ord}(b)=2$, alors $ab$ a ordre $6$.
Ainsi $G\simeq C_6$.


```math
bab^{-1}=a^{-1}\Rightarrow a^3=b^2=1,\quad ba=a^{-1}b,\quad G=\{a^ib^j:0\le i<3,\ 0\le j<2\}\simeq\mathfrak S_3.
```



| Ordre | Groupes |
|---|---|
| 1 | $\{1\}$ |
| 2, 3, 5, 7 | $C_2,C_3,C_5,C_7$ respectivement |
| 4 | $C_4$, $C_2\times C_2$ |
| 6 | $C_6$, $\mathfrak S_3$ |

## Exercice 25

### 1



```math
\operatorname{ord}(g)\in\{1,2,4,8\}.
```




```math
\operatorname{ord}(g)=8\Rightarrow G\text{ cyclique};\qquad\forall g,\ g^2=1\Rightarrow G\text{ abélien}.
```




```math
G\text{ non abélien}\Rightarrow\exists x,\quad\operatorname{ord}(x)=4.
```



### 2



```math
H=\langle x\rangle,\quad y\notin H\Rightarrow H\cap yH=\varnothing,\quad|H|+|yH|=8.
```




```math
G=H\sqcup yH=\langle x,y\rangle,\qquad xy=yx\Rightarrow G\text{ abélien},\quad\bot.
```



### 3



```math
yH=G\setminus H=Hy\Rightarrow yHy^{-1}=H.
```




```math
\operatorname{ord}(yxy^{-1})=4\Rightarrow yxy^{-1}\in\{x,x^{-1}\}\Rightarrow yxy^{-1}=x^{-1}.
```



### 4



```math
y^2\in H,\quad y^2=x^k,\qquad yx^ky^{-1}=y^2=x^k=x^{-k}\Rightarrow k\in\{0,2\}\pmod4.
```




```math
x^4=1,\quad yx=x^{-1}y,\quad y^2=1\text{ ou }x^2.
```




```math
G=\{x^iy^j:0\le i<4,\ j\in\{0,1\}\}.
```


Ces relations déterminent tous les produits :


```math
y^2=1\Rightarrow G\simeq D_8,\qquad y^2=x^2\Rightarrow G\simeq Q_8.
```




```math
D_8:\ 5\text{ éléments d'ordre }2;\qquad Q_8:\ 1\text{ élément d'ordre }2.
```



## Exercice 26

### 1



```math
g\notin H\Rightarrow gH=Hg=G\setminus H.
```




```math
g,h\notin H\Rightarrow h\in g^{-1}H\Rightarrow gh\in H.
```




```math
g\in H,h\notin H\Rightarrow gh\notin H;\qquad g,h\in H\Rightarrow gh\in H.
```




```math
\boxed{\varphi(gh)=\varphi(g)\varphi(h).}
```



### 2



```math
\chi_a(x)=(-1)^{a_1x_1+\cdots+a_dx_d},\quad a\in\mathbb F_2^d\setminus\{0\}.
```




```math
\chi_a\text{ surjective}\Rightarrow|\ker\chi_a|=2^{d-1}.
```




```math
H\text{ d'indice }2\Rightarrow\chi_H(x)=\begin{cases}1&x\in H,\\-1&x\notin H\end{cases}\text{ unique}.
```




```math
\boxed{2^d-1\text{ sous-groupes}\qquad(d\ge1).}
```



### 3



```math
H_1\ne H_2\Rightarrow\chi_1\ne\chi_2,\qquad\chi_3=\chi_1\chi_2.
```




```math
\chi_3\ne1,\quad\chi_3\ne\chi_1,\chi_2\Rightarrow\ker\chi_3\text{ troisième sous-groupe d'indice }2.
```



## Exercice 27

### 1



```math
h\longmapsto(h,h^{-1}g):G\xrightarrow{\sim}\{(h,k):hk=g\}.
```



### 2



```math
m=|G|,\qquad M^2=\frac1{m^2}\sum_{h,k\in G}hk=\frac1{m^2}\sum_{g\in G}mg=M.
```



## Exercice 28

L'assertion est fausse pour des matrices.


```math
T=\begin{pmatrix}-1&0\\0&1\end{pmatrix},\quad G=\{I_2,T\},\quad r=1,\qquad\prod_{g\in G}g=T\ne-I_2.
```


La formule valable est


```math
\prod_{g\in G}g=\prod_{\substack{g\in G\\g^2=I_n}}g,
```


les autres facteurs se regroupant par paires $g,g^{-1}$.

## Exercice 29

### 1



```math
i^2(x)=(x^{-1})^{-1}=x,\qquad\operatorname{Fix}(i)=\{x:x^2=1\}.
```



### 2



```math
|G|=|\operatorname{Fix}(i)|+2r\text{ pair}\Rightarrow|\operatorname{Fix}(i)|\text{ pair}.
```




```math
1\in\operatorname{Fix}(i)\Rightarrow\exists x\ne1,\quad x^2=1\Rightarrow\operatorname{ord}(x)=2.
```



## Exercice 30

### 1



```math
C_n=\langle\overline1\rangle\ne\{0\}\Rightarrow\operatorname{rg}(C_n)=1.
```




```math
C_n^2=\langle(1,0),(0,1)\rangle,\qquad\operatorname{ord}(x)\le n<n^2\Rightarrow\operatorname{rg}(C_n^2)=2.
```




```math
\mathfrak S_3=\langle(12),(23)\rangle\text{ non abélien}\Rightarrow\operatorname{rg}(\mathfrak S_3)=2.
```



### 2(a)



```math
G_1=\langle S_1\rangle,\quad G_2=\langle S_2\rangle\Rightarrow G_1\times G_2=\langle(S_1\times\{1\})\cup(\{1\}\times S_2)\rangle.
```




```math
\operatorname{rg}(G_1\times G_2)\le\operatorname{rg}(G_1)+\operatorname{rg}(G_2).
```



### 2(b)



```math
\operatorname{ord}(1,1)=6\text{ dans }C_2\times C_3\Rightarrow\operatorname{rg}(C_2\times C_3)=1<2.
```



### 3



```math
H_0=\{1\},\quad H_k\ne G\Rightarrow g_{k+1}\notin H_k,\quad H_{k+1}=\langle H_k,g_{k+1}\rangle.
```




```math
H_k\cap g_{k+1}H_k=\varnothing\Rightarrow|H_{k+1}|\ge2|H_k|.
```




```math
H_m=G\Rightarrow2^m\le|G|,\quad G=\langle g_1,\ldots,g_m\rangle\Rightarrow\boxed{\operatorname{rg}(G)\le\log_2|G|.}
```



### 4



```math
G=\mathbb F_2^d,\quad|G|=2^d,\quad\langle r\text{ éléments}\rangle\text{ a au plus }2^r\text{ éléments}.
```




```math
\operatorname{rg}(G)\ge d,\quad G=\langle e_1,\ldots,e_d\rangle\Rightarrow\operatorname{rg}(G)=d.
```



## Exercice 31

### 1



```math
g\in G,\quad|A|+|gB^{-1}|=|A|+|B|>|G|\Rightarrow A\cap gB^{-1}\ne\varnothing.
```




```math
a=gb^{-1}\Rightarrow g=ab\Rightarrow AB=G.
```



### 2



```math
G=C_2,\quad A=B=\{0\},\quad|A|+|B|=|G|,\quad A+B=\{0\}\ne G.
```



## Exercice 32

Dans les deux formules imprimées, lire $xy=yx$. La probabilité est le nombre de couples divisé par $|G|^2$.

### 1



```math
G/Z(G)=\langle aZ(G)\rangle\Rightarrow x=a^rz,\ y=a^sw\ (z,w\in Z(G))\Rightarrow xy=a^{r+s}zw=yx.
```




```math
G\text{ non abélien}\Rightarrow G/Z(G)\text{ non cyclique}\Rightarrow[G:Z(G)]\ge4.
```



### 2



```math
x\notin Z(G)\Rightarrow C_G(x)\subsetneq G\Rightarrow|C_G(x)|\le|G|/2.
```




```math
\frac{\#\{(x,y):xy=yx\}}{|G|^2}=\frac1{|G|^2}\sum_{x\in G}|C_G(x)|
```




```math
\le\frac{|Z(G)|}{|G|}+\frac{|G|-|Z(G)|}{2|G|}=\frac12+\frac{|Z(G)|}{2|G|}\le\boxed{\frac58.}
```



## Exercice 33

Lire $xHx^{-1}=\{xhx^{-1}:h\in H\}$.

### 1



```math
x\sim y\iff xHx^{-1}=yHy^{-1}.
```


L'égalité donne réflexivité, symétrie et transitivité.


```math
(xh)H(xh)^{-1}=xHx^{-1}\qquad(h\in H).
```




```math
G/H\twoheadrightarrow\{xHx^{-1}:x\in G\}\Rightarrow r\le|G|/|H|.
```



### 2



```math
H_1,\ldots,H_r\text{ conjugués distincts},\quad1\in\bigcap_iH_i,\quad|H_i|=|H|.
```




```math
\left|\bigcup_iH_i\right|\le1+r(|H|-1)\le1+|G|-\frac{|G|}{|H|}<|G|.
```



## Exercice 34

### 1



```math
f_{a,b}(z)=az+b,\quad a\ne0,\qquad f_{a,b}\circ f_{c,d}=f_{ac,ad+b}.
```




```math
\operatorname{id}=f_{1,0},\qquad f_{a,b}^{-1}=f_{a^{-1},-b/a}.
```



### 2



```math
f_{u,v}f_{a,b}f_{u,v}^{-1}=f_{a,ub+(1-a)v}.
```




```math
a\ne1\Rightarrow\{\text{conjugués de }f_{a,b}\}=\{f_{a,c}:c\in\mathbb C\}.
```




```math
a=1,b=0:\quad\{\operatorname{id}\};\qquad a=1,b\ne0:\quad\{f_{1,c}:c\in\mathbb C^*\}.
```



## Exercice 35

### 1



```math
I^2=J^2=-1,\qquad IJ=K=-JI,\qquad K^2=-1.
```




```math
JK=I=-KJ,\qquad KI=J=-IK.
```




```math
Q=\{\pm1,\pm I,\pm J,\pm K\}\text{ stable par produit et inverse},\qquad Q=\langle I,J\rangle.
```



### 2



```math
\begin{array}{c|rrrrrrrr}
 &1&-1&I&-I&J&-J&K&-K\\\hline
1&1&-1&I&-I&J&-J&K&-K\\
-1&-1&1&-I&I&-J&J&-K&K\\
I&I&-I&-1&1&K&-K&-J&J\\
-I&-I&I&1&-1&-K&K&J&-J\\
J&J&-J&-K&K&-1&1&I&-I\\
-J&-J&J&K&-K&1&-1&-I&I\\
K&K&-K&J&-J&-I&I&-1&1\\
-K&-K&K&-J&J&I&-I&1&-1
\end{array}
```



### 3



```math
\operatorname{ord}(1)=1,\quad\operatorname{ord}(-1)=2,\quad\operatorname{ord}(\pm I)=\operatorname{ord}(\pm J)=\operatorname{ord}(\pm K)=4.
```




```math
Z(Q_8)=\{1,-1\},\quad JIJ^{-1}=-I,\quad IJI^{-1}=-J,\quad IKI^{-1}=-K.
```




```math
\boxed{\{1\},\{-1\},\{I,-I\},\{J,-J\},\{K,-K\}.}
```



## Exercice 36

### 1



```math
\sigma^2=\tau^2=\operatorname{id},\quad\gamma(x)=\tau(-x)=x+1,\quad\gamma^n(x)=x+n.
```




```math
\sigma^{-1}\gamma^n\sigma(x)=x-n=\gamma^{-n}(x).
```



### 2



```math
\tau=\gamma\sigma,\quad\sigma\gamma^n=\gamma^{-n}\sigma,\quad\sigma^2=1.
```


Tout mot se réduit à $\gamma^n$ ou $\sigma\gamma^n$ ; réciproquement, ces applications sont des mots en $\sigma,\tau$.

### 3 et 4



```math
T_n(x)=x+n,\quad R_n(x)=-x+n,\quad G=\{T_n,R_n:n\in\mathbb Z\}.
```




```math
T_nT_m=T_{n+m},\quad T_nR_m=R_{n+m},\quad R_nT_m=R_{n-m},\quad R_nR_m=T_{n-m}.
```




```math
T_0=1,\quad T_n^{-1}=T_{-n},\quad R_n^{-1}=R_n.
```



### 5



```math
R_nT_1=R_{n-1}\ne R_{n+1}=T_1R_n.
```




```math
T_nR_0=R_n,\quad R_0T_n=R_{-n}\Rightarrow n=0.
```




```math
\boxed{Z(G)=\{T_0\}.}
```



### 6



```math
\varepsilon,\delta\in\{-1,1\},\qquad\chi(T_n)=\varepsilon^n,\quad\chi(R_n)=\varepsilon^n\delta.
```


Les quatre règles de multiplication donnent $\chi(gh)=\chi(g)\chi(h)$.


```math
\chi\mapsto(\chi(T_1),\chi(R_0))\Rightarrow\boxed{4\text{ morphismes}.}
```



### 7



```math
n\ne0\Rightarrow T_n^k=T_{kn}\ne1\quad(k\ge1),\qquad R_n^2=1.
```




```math
T_kR_nT_{-k}=R_{n+2k}.
```




```math
R_{2m}\sim R_0=\sigma,\qquad R_{2m+1}\sim R_1=\tau.
```



## Exercice 37

### 1



```math
f\text{ isométrie}\Rightarrow f\text{ injective}\Rightarrow f\text{ bijective sur }\mathbb U_n.
```




```math
|f^{-1}(u)-f^{-1}(v)|=|u-v|.
```


Les compositions et l'identité préservent aussi les distances.

### 2



```math
\zeta=e^{2i\pi/n},\quad r^k(z)=\zeta^kz,\qquad r^k=1\iff n\mid k\Rightarrow\operatorname{ord}(r)=n.
```



### 3



```math
f(1)=1,\quad f(\zeta)=\zeta\Rightarrow|f(z)-1|=|z-1|,\quad|f(z)-\zeta|=|z-\zeta|.
```




```math
|z|=|f(z)|=1\Rightarrow\operatorname{Re}f(z)=\operatorname{Re}z,\quad\operatorname{Re}(f(z)\overline\zeta)=\operatorname{Re}(z\overline\zeta).
```




```math
\sin(2\pi/n)\ne0\Rightarrow\operatorname{Im}f(z)=\operatorname{Im}z\Rightarrow f(z)=z.
```



### 4



```math
f(1)=\zeta^k,\quad g=r^{-k}f\Rightarrow g(1)=1.
```




```math
\min_{z\in\mathbb U_n\setminus\{1\}}|z-1|=|\zeta-1|,\quad\text{atteint en }\zeta,\zeta^{-1}\Rightarrow g(\zeta)\in\{\zeta,\zeta^{-1}\}.
```




```math
c(z)=\overline z:\quad g(\zeta)=\zeta\Rightarrow g=1;\quad g(\zeta)=\zeta^{-1}\Rightarrow cg=1.
```




```math
\boxed{D_{2n}=\{r^k,r^kc:0\le k<n\},\qquad|D_{2n}|=2n.}
```



### 5



```math
crc=r^{-1}\ne r\qquad(n\ge3).
```



### 6



```math
(r^kc)^2=r^kr^{-k}=1,\qquad r^kc\ne1.
```




```math
\operatorname{ord}(r^k)=2\iff n\text{ pair et }k=n/2\pmod n.
```




```math
\boxed{r=(rc)c.}
```



### 7



```math
\chi(r)=\varepsilon,\quad\chi(c)=\delta,\qquad\varepsilon,\delta\in\{-1,1\},\quad\varepsilon^n=1.
```




```math
\chi(r^kc^b)=\varepsilon^k\delta^b,\qquad crc=r^{-1}\Rightarrow\delta\varepsilon\delta=\varepsilon^{-1}.
```




```math
\boxed{n\text{ impair}:2\text{ morphismes};\qquad n\text{ pair}:4\text{ morphismes}.}
```



## Exercice 38

### 1



```math
f_{a,b}(x)=ax+b,\quad a\in\mathbb R^*,\quad b\in\mathbb R.
```




```math
f_{a,b}f_{c,d}=f_{ac,ad+b},\quad f_{a,b}^{-1}=f_{a^{-1},-b/a},\quad1=f_{1,0}.
```



### 2



```math
f,g\in\Gamma\Rightarrow fgf^{-1}g^{-1}\text{ a pour coefficient directeur }1.
```




```math
\text{Une translation possède un point fixe}\iff\text{elle est l'identité}\Rightarrow fg=gf.
```




```math
\Gamma=\{1\}\Rightarrow\text{tout }\omega\text{ convient}.
```




```math
f_{a,b}\in\Gamma\setminus\{1\}\Rightarrow a\ne1,\qquad\omega=\frac b{1-a}\text{ unique point fixe de }f.
```




```math
g\in\Gamma\Rightarrow f(g(\omega))=g(f(\omega))=g(\omega)\Rightarrow g(\omega)=\omega.
```


