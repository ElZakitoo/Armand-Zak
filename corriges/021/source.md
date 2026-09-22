# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td21-applications-lineaires.pdf)

## Autocorrection A



```math
\begin{array}{c|l}
\text{cas}&\text{conclusion}\\\hline
\text{(i)}&\text{non : }f(1,0)+f(0,1)=0\ne1=f(1,1)\\
\text{(ii)}&\text{non : }f(0,0)=(1,0,0)\ne0\\
\text{(iii)}&\text{oui : chaque coordonnée est une forme linéaire}\\
\text{(iv)}&\text{non : }f(0)=1\\
\text{(v)}&\text{non : }f(-1)=1\ne-f(1)\\
\text{(vi)}&\mathbb R_+\text{ n'est pas un espace vectoriel réel}\\
\text{(vii)}&\text{non : }f(2,0)=4\ne2f(1,0)\\
\text{(viii)}&\text{oui : chaque coordonnée est linéaire}\\
\text{(ix)}&\text{non : }f(1,0)+f(0,1)=0\ne f(1,1)\\
\text{(x)}&\text{oui : }(aP+bQ)(X^2)=aP(X^2)+bQ(X^2)\\
\text{(xi)}&\text{non sur }\mathbb R,\mathbb C:\ f(2)=4\ne2f(1)\\
\text{(xii)}&\text{oui : combinaison linéaire de dérivations}\\
\text{(xiii)}&\text{oui : somme de deux évaluations}\\
\text{(xiv)}&\text{non : }f(2\cdot1)=8\ne2f(1)=6\\
\text{(xv)}&\text{non : }f(-1)=1\ne-f(1)\\
\text{(xvi)}&\text{non : }f(2\cdot1)=4\ne2f(1)\\
\text{(xvii)}&\text{oui : linéarité de la dérivation itérée}\\
\text{(xviii)}&\text{oui : linéarité des deux limites}
\end{array}
```


Dans (xi), sur $\mathbb F_2$, l'application $P\mapsto P^2$ est linéaire ; sur un corps de caractéristique $2$ plus grand, elle n'est pas linéaire sur ce corps.

## Exercice 1

### 1



```math
f(x)=f(x\cdot1)=xf(1)\Rightarrow\boxed{f:x\mapsto ax,\quad a\in\mathbb K.}
```



### 2



```math
x=\sum_{j=1}^px_je_j\Rightarrow f(x)=\sum_jx_jf(e_j)=Ax,
```


où la colonne $j$ de $A$ est $f(e_j)$. Réciproquement, $x\mapsto Ax$ est linéaire.

### 3



```math
\Phi:M_{n,p}(\mathbb K)\to\mathcal L(\mathbb K^p,\mathbb K^n),\quad A\mapsto\varphi_A
```


est linéaire, surjective par 2 et injective car ses valeurs sur les $e_j$ déterminent ses colonnes.

### 4



```math
\varphi_{AB}(x)=ABx=\varphi_A(\varphi_B(x)),\qquad\varphi_{I_n}=\operatorname{id}.
```


L'isomorphisme vectoriel préserve le produit et l'unité.

### 5



```math
A\in GL_n\iff\varphi_A\in GL(\mathbb K^n),\qquad\varphi_{A^{-1}}=(\varphi_A)^{-1}.
```



## Exercice 2



```math
E=\ker(u\mapsto u_0).
```


$\Delta$ est linéaire. Pour $v\in\mathbb R^{\mathbb N}$,


```math
u_0=0,\qquad u_n=\sum_{k=0}^{n-1}v_k\quad(n\ge1)
```


est l'unique solution de $u_{n+1}-u_n=v_n$ avec $u\in E$.


```math
\boxed{\Delta^{-1}(v)_n=\sum_{k=0}^{n-1}v_k.}
```



## Exercice 3



```math
E_a=\ker(P\mapsto P(a))=(X-a)\mathbb K[X].
```




```math
\Phi:\mathbb K[X]\to E_a,\quad Q\mapsto(X-a)Q
```


est linéaire, injective par intégrité et surjective par factorisation en une racine.

## Exercice 4

Pour $n=0$, l'identité vaut $0=0$. Si $f^ng-gf^n=nf^n$,


```math
f^{n+1}g-gf^{n+1}=f(f^ng-gf^n)+(fg-gf)f^n=nf^{n+1}+f^{n+1}.
```



## Exercice 5



```math
f^N=0\Rightarrow(\operatorname{id}-f)\left(\sum_{k=0}^{N-1}f^k\right)=\left(\sum_{k=0}^{N-1}f^k\right)(\operatorname{id}-f)=\operatorname{id}.
```




```math
\boxed{(\operatorname{id}-f)^{-1}=\sum_{k=0}^{N-1}f^k.}
```



## Autocorrection B

La linéarité résulte dans chaque cas des expressions linéaires des coordonnées.


```math
\text{(i)}\quad\boxed{\ker f=\mathbb R(-2,1),\quad\operatorname{im}f=\mathbb R(1,-2).}
```




```math
\text{(ii)}\quad f(x,y,z)=0\Rightarrow x=z=y=0\Rightarrow\boxed{\ker f=0,\quad\operatorname{im}f=\mathbb R^3}.
```




```math
\text{(iii)}\quad x=2y=-2z\Rightarrow\boxed{\ker f=\mathbb R(2,1,-1)}.
```




```math
f(0,-a/2,b/2)=(a,b)\Rightarrow\boxed{\operatorname{im}f=\mathbb R^2}.
```




```math
\text{(iv)}\quad x-2y=x+2y=0\Rightarrow x=y=0\Rightarrow\boxed{\ker f=0,\quad\operatorname{im}f=\mathbb R^2}.
```



## Autocorrection C

### 1

La dérivation seconde est linéaire et diminue le degré ; $T_n$ est donc un endomorphisme.

### 2



```math
T_n(X^k)=\omega^2X^k+k(k-1)X^{k-2}.
```


Sa matrice dans la base canonique est triangulaire, de diagonale constante $\omega^2\ne0$ ; elle est inversible.

### 3

Pour tout polynôme non nul $P$, $\deg(P''+\omega^2P)=\deg P$. Une solution a donc degré $n$ et est unique par 2.


```math
\boxed{P=\sum_{j=0}^{\lfloor n/2\rfloor}\frac{(-1)^j n!}{(n-2j)!\omega^{2j+2}}X^{n-2j}.}
```


La substitution dans $P''+\omega^2P$ annule deux à deux les termes sauf $X^n$.

## Exercice 6

### 1



```math
\Delta(aP+bQ)=a\Delta P+b\Delta Q.
```



### 2



```math
\deg P=d\ge1\Rightarrow\deg\Delta P=d-1
```


en caractéristique nulle. Donc $\ker\Delta=\mathbb K$.

### 3



```math
\Delta(X^{k+1})=(k+1)X^k+\text{termes de degré inférieur}.
```


Les polynômes $\Delta X,\ldots,\Delta X^{n+1}$ forment une base de $\mathbb K_n[X]$ pour tout $n$.


```math
\boxed{\operatorname{im}\Delta=\mathbb K[X].}
```



### 4



```math
E=X\mathbb K[X],\qquad E\cap\ker\Delta=0.
```


Pour toute préimage $P$ d'un polynôme $Q$, $P-P(0)\in E$ est encore une préimage. Ainsi $\Delta|_E:E\simeq\mathbb K[X]$.

## Exercice 7



```math
P=\sum_{k=0}^na_kX^k\Rightarrow f(P)=\sum_{k=0}^n(2^k-1)a_kX^k.
```




```math
\boxed{\ker f=\mathbb R,\quad\operatorname{im}f=X\mathbb R[X].}
```


Pour $Q=\sum_{k\ge1}b_kX^k$, une préimage est $\sum_{k\ge1}b_kX^k/(2^k-1)$.

## Exercice 8

### 1

La résolution des trois systèmes donne


```math
\boxed{\ker u=\mathbb Rv_0,\quad v_0=(1,-1,\sqrt2),}
```




```math
\boxed{\ker(u-2I)=\mathbb Rv_+,\quad v_+=(2-\sqrt2,2+\sqrt2,2),}
```




```math
\boxed{\ker(u+2I)=\mathbb Rv_-,\quad v_-=(-2-\sqrt2,-2+\sqrt2,2).}
```



### 2

Les vecteurs propres associés aux trois valeurs propres distinctes $0,2,-2$ sont libres. Ces trois vecteurs forment donc une base de $\mathbb R^3$.

### 3



```math
u(av_++bv_-)=2av_+-2bv_-\in E.
```




```math
\boxed{(u|_E)^{-1}(av_++bv_-)=\tfrac a2v_+-\tfrac b2v_-.}
```



## Exercice 9

### 1

Supposons $T^2=D$. Alors $TD=DT$, donc $T$ préserve $\ker D=\mathbb R1$.


```math
T1=c1\Rightarrow0=D1=T^21=c^21\Rightarrow c=0.
```


Pour $\iota:x\mapsto x$,


```math
D(T\iota)=T(D\iota)=T1=0\Rightarrow T\iota\text{ constant}\Rightarrow T^2\iota=0,
```


mais $D\iota=1$. Contradiction.

### 2

Une racine carrée réelle existe sur $E=C^\infty(\mathbb R^*)$. La construction suivante utilise le choix d'une base et le lemme de Zorn.

Posons $R=\mathbb R[t]$ et faisons agir $R$ sur $E$ par


```math
P(t)\cdot f=P(D)f.
```


Pour tout $P\ne0$, $P(D):E\to E$ est surjectif : sur chacun des intervalles $(-\infty,0)$ et $(0,+\infty)$, l'équation différentielle linéaire à coefficients constants $P(D)u=f$ possède une solution globale, obtenue par des conditions initiales en $-1$ et $1$. Ainsi $E$ est un $R$-module divisible.

Définissons sa partie de torsion :


```math
N=\{f\in E:\exists P\in R\setminus\{0\},\ P(D)f=0\}.
```


C'est un sous-module : si $Pf=0$ et $Qg=0$, alors $PQ(f+g)=0$. Il est divisible : pour $Q\ne0$ et $f\in N$, choisissons $u$ avec $Qu=f$ ; si $Pf=0$, alors $PQu=0$, donc $u\in N$.

**Lemme.** Un sous-module divisible $N$ d'un module $M$ sur l'anneau principal $R$ admet un supplémentaire.

Partons de l'identité $N\to N$ et prolongeons-la à un morphisme $h:U\to N$, où $N\subset U\subset M$, maximal par le lemme de Zorn. Si $x\notin U$, l'ensemble


```math
I=\{r\in R:rx\in U\}
```


est un idéal, donc $I=(a)$. Si $a=0$, choisissons $v=0$. Si $a\ne0$, la divisibilité fournit $v\in N$ tel que $av=h(ax)$. La formule


```math
\widetilde h(u+rx)=h(u)+rv
```


est bien définie : si $rx\in U$, alors $r=as$ et $h(rx)=sh(ax)=rv$ ; pour $I=0$, il n'y a aucune relation non triviale. Elle prolonge $h$ à $U+Rx$, contradiction. Ainsi $U=M$.


```math
h|_N=I_N\Rightarrow M=N\oplus\ker h.
```



Appliquons le lemme :


```math
E=N\oplus W,
```


où $W$ est stable par $D$. Le module $W$ est sans torsion et divisible. Pour chaque $P\ne0$, $P(D)|_W$ est donc bijectif, et $W$ devient un espace vectoriel sur $K=\mathbb R(t)$.

La dimension de $W$ sur $K$ est infinie. Choisissons une suite de fonctions non nulles $f_j\in C_c^\infty((0,+\infty))$ dont les supports sont contenus dans des intervalles deux à deux disjoints. Leurs classes dans $E/N\simeq W$ sont $K$-libres. En effet, après multiplication par un dénominateur commun, une relation donnerait


```math
\sum_{j\in J}P_j(D)f_j\in N
```


avec $J$ fini. Le membre de gauche est à support compact. Or une fonction à support compact annulée par un opérateur différentiel constant non nul est nulle, par unicité des solutions de l'équation homogène avec données initiales nulles hors du support. Ainsi


```math
\sum_{j\in J}P_j(D)f_j=0.
```


La disjonction des supports implique $P_j(D)f_j=0$ pour chaque $j$. Comme $f_j\ne0$ est à support compact, nécessairement $P_j=0$.

Une base infinie de $W$ peut se partitionner en paires $(e_\lambda,f_\lambda)$. Définissons $S_W$, $K$-linéairement, par


```math
S_W(e_\lambda)=f_\lambda,\qquad S_W(f_\lambda)=t e_\lambda.
```




```math
S_W^2=tI=D|_W.
```



Enfin, posons


```math
H=\{h\in C^\infty(\mathbb R):\exists P\ne0,\ P(D)h=0\}.
```


Chaque solution d'une équation homogène constante sur une demi-droite se prolonge de façon unique à $\mathbb R$. Pour deux équations différentes, l'unicité du prolongement résulte en appliquant le produit des opérateurs et l'unicité de l'équation homogène correspondante. Par restriction aux deux composantes,


```math
N\simeq H\oplus H,
```


et $D$ agit sur les deux facteurs par la dérivation. Définissons


```math
S_N(h_+,h_-)=(Dh_-,h_+).
```




```math
S_N^2(h_+,h_-)=(Dh_+,Dh_-).
```


Sur $E=N\oplus W$, posons $T=S_N\oplus S_W$ ; c'est une application $\mathbb R$-linéaire et


```math
\boxed{T^2=D.}
```



## Autocorrection D



```math
f(E_1)\subset f(E_2)\Rightarrow\forall x\in E_1,\ \exists y\in E_2,\ f(x)=f(y)\Rightarrow x\in E_2+\ker f.
```


D'où $E_1+\ker f\subset E_2+\ker f$. Réciproquement, si $x=y+k$ avec $y\in E_2,k\in\ker f$, alors $f(x)=f(y)\in f(E_2)$.

## Exercice 10



```math
x\in\ker f\Rightarrow f(gx)=g(fx)=0\Rightarrow gx\in\ker f.
```




```math
y=fx\in\operatorname{im}f\Rightarrow gy=gfx=fgx\in\operatorname{im}f.
```



## Exercice 11



```math
gf=0\iff\forall x\in E,\ f(x)\in\ker g\iff\boxed{\operatorname{im}f\subset\ker g}.
```



## Exercice 12

### 1



```math
fx=0\Rightarrow gfx=0\Rightarrow\ker f\subset\ker(gf).
```


Si $\operatorname{im}f\cap\ker g=0$, $gfx=0$ implique $fx=0$. Réciproquement, si les deux noyaux sont égaux,


```math
y=fx\in\ker g\Rightarrow x\in\ker(gf)=\ker f\Rightarrow y=0.
```



### 2



```math
\operatorname{im}(gf)\subset\operatorname{im}g.
```




```math
\operatorname{im}(gf)=\operatorname{im}g\iff\forall y\in F,\ \exists x\in E,\ gy=gfx
```




```math
\iff\forall y\in F,\ y\in\operatorname{im}f+\ker g.
```



### 3



```math
\boxed{\ker(gf)=f^{-1}(\ker g),\qquad\operatorname{im}(gf)=g(\operatorname{im}f).}
```



## Exercice 13

### 1



```math
x\in f^{-1}(f(F))\iff\exists y\in F,\ f(x-y)=0\iff x\in F+\ker f.
```



### 2



```math
y\in f(f^{-1}(F))\iff y\in\operatorname{im}f\text{ et }y\in F.
```



### 3



```math
F\cap\operatorname{im}f=F+\ker f\iff\boxed{\ker f\subset F\subset\operatorname{im}f}.
```


Les inclusions $F\cap\operatorname{im}f\subset F\subset F+\ker f$ imposent que les trois espaces soient égaux.

## Exercice 14

### 1



```math
u(x_1+x_2)=u(x_1)+u(x_2)\Rightarrow u(S_1+S_2)=u(S_1)+u(S_2).
```



### 2



```math
u(x_1)=u(x_2),\quad x_i\in S_i\Rightarrow u(x_1-x_2)=0\Rightarrow x_1=x_2\in S_1\cap S_2=0.
```


L'intersection des deux images est nulle.

### 3



```math
u:\mathbb R^2\to\mathbb R,\quad u(x,y)=x+y,\quad S_1=\mathbb Re_1,\quad S_2=\mathbb Re_2.
```




```math
S_1\cap S_2=0,\qquad u(S_1)=u(S_2)=\mathbb R.
```



## Exercice 15

Pour $x\in E$, $fx\in\operatorname{im}(f+g)$ : il existe $y$ tel que $fy+gy=fx$. L'unicité de la décomposition dans $\operatorname{im}f\oplus\operatorname{im}g$ impose


```math
fy=fx,\qquad gy=0.
```




```math
x=(x-y)+y\in\ker f+\ker g.
```



## Exercice 16

### 1



```math
f(u_0)\ne0\Rightarrow\forall a\in\mathbb K,\ f\left(\frac a{f(u_0)}u_0\right)=a.
```



### 2



```math
x=\underbrace{x-\frac{f(x)}{f(u_0)}u_0}_{\in\ker f}+\underbrace{\frac{f(x)}{f(u_0)}u_0}_{\in\mathbb Ku_0}.
```




```math
\lambda u_0\in\ker f\Rightarrow\lambda f(u_0)=0\Rightarrow\lambda=0.
```



### 3



```math
\operatorname{tr}I_n=n1_{\mathbb K}.
```




```math
\boxed{M_n(\mathbb K)=\mathfrak{sl}_n(\mathbb K)\oplus\mathbb KI_n\iff n1_{\mathbb K}\ne0.}
```


Si $n1_{\mathbb K}=0$, $I_n\in\mathfrak{sl}_n$ et la somme n'est pas directe. Sinon,


```math
M=\left(M-\frac{\operatorname{tr}M}nI_n\right)+\frac{\operatorname{tr}M}nI_n.
```



## Exercice 17

Si $g=\lambda f$ et $g\ne0$, alors $\lambda\ne0$ et les noyaux sont égaux. Réciproquement, choisissons $u$ avec $f(u)=1$.


```math
x=f(x)u+(x-f(x)u),\quad x-f(x)u\in\ker f=\ker g.
```




```math
g(x)=g(u)f(x),\qquad g(u)\ne0.
```



## Exercice 18



```math
p=f^6,\quad p^2=f^{12}=f^6=p.
```




```math
fp=f^7=f,\quad p= f^5f\Rightarrow\ker p=\ker f.
```




```math
\operatorname{im}p\subset\operatorname{im}f,\quad pf=f\Rightarrow\operatorname{im}f\subset\operatorname{im}p.
```


Un projecteur donne $E=\ker p\oplus\operatorname{im}p$.

## Exercice 19

### 1



```math
\boxed{a=\frac1{\beta-\alpha},\qquad b=\frac1{\alpha-\beta}.}
```


Ces coefficients appartiennent au corps des scalaires ; ils ne sont pas nécessairement réels si ce corps est $\mathbb C$.

### 2



```math
x=a(f-\alpha I)x+b(f-\beta I)x
```


donne la somme des images.

### 3

Les deux facteurs commutent, et leur produit est nul. Ainsi


```math
\operatorname{im}(f-\beta I)\subset\ker(f-\alpha I),\quad\operatorname{im}(f-\alpha I)\subset\ker(f-\beta I).
```



### 4

Les questions 2–3 donnent la somme des noyaux. Si $x$ appartient aux deux,


```math
fx=\alpha x=\beta x\Rightarrow(\alpha-\beta)x=0\Rightarrow x=0.
```



## Exercice 20



```math
A=\{u:u|_G=0\}
```


est stable par combinaisons linéaires. La restriction


```math
\rho:A\to\mathcal L(H,F),\quad u\mapsto u|_H
```


est linéaire et bijective, d'inverse


```math
v\mapsto\widetilde v,\qquad\widetilde v(g+h)=v(h).
```


L'unicité de $g+h$ assure que cette extension est bien définie.

## Exercice 21

Les graphes $V_f$ de l'énoncé sont les supplémentaires de $G$, et non de $F$. Par exemple, $f=0$ donne $V_f=F$.

### 1

Pour $S$ supplémentaire de $G$, la projection $\pi_F$ parallèlement à $G$ induit une bijection $S\to F$ : elle est injective car $S\cap G=0$, et surjective car $E=S+G$.
Ainsi, pour chaque $x\in F$, il existe un unique $y\in G$ tel que $x+y\in S$.

### 2



```math
f=\pi_G\circ(\pi_F|_S)^{-1}:F\to G
```


est linéaire et vérifie $S=V_f$. L'unicité de $y$ impose celle de $f$. Réciproquement,


```math
x+y=(x+f(x))+(y-f(x)),\qquad V_f\cap G=0.
```


Pour les supplémentaires de $F$ effectivement demandés, la formule correcte est


```math
\boxed{S=\{y+h(y):y\in G\},\qquad h\in\mathcal L(G,F),}
```


avec un unique $h$.

### 3

Tous les supplémentaires de $F$ sont isomorphes à $G$ par la projection sur $G$ parallèlement à $F$ ; ils sont donc deux à deux isomorphes.

## Exercice 22

Si $E=0$, le résultat est immédiat. Sinon, fixons $a\ne0$ et écrivons $u(a)=\lambda a$.
Pour $x$ colinéaire à $a$, $u(x)=\lambda x$. Pour $x$ indépendant de $a$, écrivons $u(x)=\mu x$ et $u(a+x)=\nu(a+x)$.


```math
\lambda a+\mu x=\nu a+\nu x\Rightarrow\lambda=\mu=\nu.
```




```math
\boxed{u=\lambda I.}
```



## Autocorrection E

### 1



```math
\ell(x,y,z)=x+y-z,\quad v=(1,1,3),\quad\ell(v)=-1\ne0.
```




```math
\mathbb R^3=\ker\ell\oplus\mathbb Rv=F\oplus G.
```



### 2



```math
p_F(w)=w+\ell(w)v,\quad\ell(2,2,3)=1\Rightarrow\boxed{p_F(2,2,3)=(3,3,6).}
```



### 3



```math
p_G(w)=-\ell(w)v,\quad\ell(1,-2,0)=-1\Rightarrow\boxed{p_G(1,-2,0)=(1,1,3).}
```



## Autocorrection F

### 1–2



```math
A=\begin{pmatrix}1&2&0\\4&-1&0\\-2&2&3\end{pmatrix},\qquad A^2=9I_3\Rightarrow f^2=9I.
```



### 3–4



```math
(f/3)^2=I\Rightarrow f/3\text{ est une symétrie},\qquad\boxed{f^{-1}=f/9.}
```



## Exercice 23

### 1



```math
x=x_0+x_1,\quad x_0\in\ker g,\quad x_1\in\operatorname{im}g.
```




```math
fgx=fx_1,\quad gfx=gfx_0+gfx_1=0+fx_1,
```


par stabilité et puisque $g$ vaut l'identité sur son image.

### 2



```math
g=\begin{pmatrix}1&0\\0&2\end{pmatrix},\quad f=\begin{pmatrix}0&1\\0&0\end{pmatrix}.
```




```math
\ker g=0,\quad\operatorname{im}g=\mathbb R^2\text{ stables par }f,\qquad fg=2f\ne f=gf.
```



## Exercice 24

Avec les deux axes complémentaires, pour $x=x_1+x_2$, $x_i\in S_i$,


```math
p_1x=x_1,\quad p_2x=x_2,\quad s_1x=x_1-x_2,\quad s_2x=-x_1+x_2.
```




```math
\boxed{p_1+p_2=I,\quad p_1p_2=p_2p_1=0,\quad s_1+s_2=0,\quad s_1s_2=s_2s_1=-I.}
```


L'axe de $s_2$ est $S_2$.

## Exercice 25

### 1



```math
pq=qp\Rightarrow(pq)^2=p^2q^2=pq.
```



### 2



```math
(p+q)^2=p+q\iff pq+qp=0.
```


En multipliant successivement cette égalité à gauche et à droite par $p$,


```math
pq+pqp=0,\quad pqp+qp=0\Rightarrow pq=qp\Rightarrow2pq=0.
```


La caractéristique n'est pas $2$ : $pq=qp=0$. Réciproquement, ces deux égalités donnent $(p+q)^2=p+q$.


```math
z\in\operatorname{im}p\cap\operatorname{im}q\Rightarrow z=pz=pqz=0.
```




```math
\operatorname{im}(p+q)\subset\operatorname{im}p+\operatorname{im}q,\quad(p+q)p=p,\quad(p+q)q=q.
```




```math
\boxed{\operatorname{im}(p+q)=\operatorname{im}p\oplus\operatorname{im}q.}
```




```math
px+qx=0\Rightarrow px=qx=0\Rightarrow\boxed{\ker(p+q)=\ker p\cap\ker q}.
```



## Exercice 26

### 1



```math
q=I-p,\quad pq=p-p^2=0\Rightarrow p^2=p,
```




```math
q^2=(I-p)^2=I-p=q,\qquad qp=p-p^2=0.
```



### 2



```math
qp=0\Rightarrow\operatorname{im}p\subset\ker q,\qquad qx=0\Rightarrow x=px.
```


Ainsi $\operatorname{im}p=\ker q$ ; par symétrie, $\operatorname{im}q=\ker p$.

## Exercice 27

### 1



```math
pq+qp=0\Rightarrow pq+pqp=0,\quad pqp+qp=0\Rightarrow pq=qp\Rightarrow2pq=0.
```



### 2



```math
(p-q)^2=p-q\iff pq+qp=2q.
```


Multiplication à gauche et à droite par $q$ :


```math
qpq+qp=2q,\quad pq+qpq=2q\Rightarrow pq=qp.
```


Alors $2pq=2q$, donc $pq=qp=q$. La réciproque résulte de la même expansion.

## Exercice 28

### 1



```math
pq=0,\quad p^2=p,\quad q^2=q\Rightarrow r^2=(p+q-qp)^2=p+q-qp=r.
```



### 2



```math
z\in\operatorname{im}p\cap\operatorname{im}q\Rightarrow pz=z,\quad pz=pqz=0\Rightarrow z=0.
```



### 3



```math
rp=p,\quad rq=q,\quad\operatorname{im}r\subset\operatorname{im}p+\operatorname{im}q\Rightarrow\operatorname{im}r=F.
```




```math
pr=p,\quad qr=q\Rightarrow rx=0\Rightarrow px=qx=0.
```


La réciproque est immédiate, donc $\ker r=G$ et


```math
\boxed{E=F\oplus G,\qquad r\text{ projecteur sur }F\text{ parallèlement à }G.}
```



## Exercice 29



```math
a=u+v,\quad b=u-v,\quad c=uv-vu.
```




```math
a^2+b^2=4I,\qquad ab=-c,\quad ba=c.
```



### 1

Si $cx=0$, alors


```math
x=\tfrac14a^2x+\tfrac14b^2x,\qquad ba^2x=0,\quad ab^2x=0.
```


Ainsi $x\in\ker b+\ker a$. Réciproquement, $c=ba=-ab$ annule $\ker a$ et $\ker b$.


```math
x\in\ker a\cap\ker b\Rightarrow4x=(a^2+b^2)x=0.
```




```math
\boxed{\ker(uv-vu)=\ker(u+v)\oplus\ker(u-v).}
```



### 2



```math
c=ba=-ab\Rightarrow\operatorname{im}c\subset\operatorname{im}a\cap\operatorname{im}b.
```


Si $y=as=bt$, alors


```math
4y=(a^2+b^2)y=a^2bt+b^2as=c(at-bs).
```




```math
\boxed{\operatorname{im}(uv-vu)=\operatorname{im}(u+v)\cap\operatorname{im}(u-v).}
```



## Exercice 30

### 1

Dans une base propre $(e_i)$, $u(e_i)=\lambda_ie_i$.


```math
\ker u=\operatorname{Vect}(e_i:\lambda_i=0),\qquad\operatorname{im}u=\operatorname{Vect}(e_i:\lambda_i\ne0).
```


Ces deux sous-familles disjointes constituent la base entière : $E=\ker u\oplus\operatorname{im}u$.

### 2



```math
A=PDP^{-1},\quad D\text{ diagonale}\iff\text{les colonnes de }P\text{ forment une base propre de }\varphi_A.
```



## Exercice 31

L'hypothèse signifie que $x$ et $f(x)$ sont colinéaires pour tout $x$. L'exercice 22 donne $f=\lambda I$.

## Exercice 32

Récurrence sur $i+j$. Si $i=0$ ou $j=0$, le résultat est immédiat. Pour $i,j\ge1$ et $x\in\ker u^i\cap\ker v^j$, la commutation donne


```math
ux\in\ker u^{i-1}\cap\ker v^j,\qquad vx\in\ker u^i\cap\ker v^{j-1}.
```


Par récurrence, $ux=vx=0$, puis $x\in\ker u\cap\ker v=0$.

## Exercice 33

### 1

Pour $g\in G$, $g(F)=F$, car $g^{-1}\in G$ aussi. Ainsi $g^{-1}pg$ a image dans $F$ et vaut l'identité sur $F$.


```math
\pi(E)\subset F,\quad\pi|_F=I_F\Rightarrow\pi^2=\pi,\quad\operatorname{im}\pi=F.
```


Pour $h\in G$,


```math
h^{-1}\pi h=\frac1{|G|}\sum_{g\in G}(gh)^{-1}p(gh)=\frac1{|G|}\sum_{k\in G}k^{-1}pk=\pi.
```



### 2



```math
E=F\oplus\ker\pi,\qquad\pi h=h\pi\Rightarrow\ker\pi\text{ stable sous }G.
```



### 3

Sur $\mathbb F_p$, prenons $E=\mathbb F_p^2$, $F=\mathbb F_pe_1$ et


```math
g=\begin{pmatrix}1&1\\0&1\end{pmatrix},\qquad G=\langle g\rangle,\quad|G|=p.
```


Tout supplémentaire de $F$ est une droite $\mathbb F_p(e_2+ae_1)$. Or


```math
g(e_2+ae_1)=e_2+(a+1)e_1
```


n'appartient pas à cette droite. Aucun supplémentaire stable.
Sur $\mathbb R$, la même matrice engendre un groupe infini et donne le même contre-exemple.

## Exercice 34

### 1

Si $g$ est un pseudo-inverse, posons $p=fg=gf$.


```math
p^2=fgfg=fg=p,\quad pf=fp=f,\quad pg=gp=g.
```




```math
\operatorname{im}p=\operatorname{im}f,\qquad\ker p=\ker f=\ker g.
```


En effet, $p=gf$ donne $\ker f\subset\ker p$, et $f=fp$ donne l'inclusion inverse ; les mêmes arguments valent pour $g$.
Sur $\ker f$, $g=0$. Sur $\operatorname{im}f$, $fg=gf=I$, donc $g$ est l'inverse de la restriction de $f$. Ces deux propriétés déterminent $g$ sur


```math
E=\ker p\oplus\operatorname{im}p=\ker f\oplus\operatorname{im}f.
```



### 2



```math
f\text{ inversible}\Rightarrow\boxed{f^\#=f^{-1}};\qquad f^2=f\Rightarrow\boxed{f^\#=f}.
```


Les trois relations se vérifient directement.

### 3

Si $E=\ker f\oplus\operatorname{im}f$, la restriction $h=f|_{\operatorname{im}f}$ est injective. Elle est surjective : pour $y=fx$, écrivons $x=k+z$, $k\in\ker f,z\in\operatorname{im}f$ ; alors $y=fz$.


```math
g|_{\ker f}=0,\qquad g|_{\operatorname{im}f}=h^{-1}.
```


Sur chacun des deux facteurs de la somme directe, $fg=gf$, $fgf=f$ et $gfg=g$.

### 4(a)

Les calculs de 1 donnent


```math
ff^\#\text{ projecteur},\quad\ker(ff^\#)=\ker f^\#,\quad\operatorname{im}(ff^\#)=\operatorname{im}f.
```




```math
E=\ker f^\#\oplus\operatorname{im}f.
```



### 4(b)



```math
\ker f^\#=\ker f\Rightarrow\boxed{E=\ker f\oplus\operatorname{im}f}.
```



### 5

La somme directe implique $\ker f^2=\ker f$ et $\operatorname{im}f^2=\operatorname{im}f$, car la restriction à l'image est un automorphisme.
Réciproquement, si ces deux égalités valent,


```math
y=fx\in\ker f\Rightarrow f^2x=0\Rightarrow fx=0,
```


donc $\ker f\cap\operatorname{im}f=0$. Pour tout $x$, $fx\in\operatorname{im}f^2$, donc $fx=f^2z$ pour un certain $z$ ; alors


```math
x=(x-fz)+fz\in\ker f+\operatorname{im}f.
```


La question 3 conclut.

## Exercice 35



```math
a=(n)_{n\in\mathbb N},\qquad\varphi(a)=m\in\mathbb N.
```


Fixons $u\in\mathbb R^{\mathbb N}$. Pour tout $t\in\mathbb R$, la propriété appliquée à $a+tu$ impose un indice $n$ tel que


```math
n+tu_n=m+t\varphi(u).
```


Si $\varphi(u)\ne u_m$, pour $n=m$ cette égalité a au plus une solution en $t$. Pour chaque $n\ne m$, elle a également au plus une solution. L'ensemble des $t$ possibles serait donc dénombrable, contrairement à $\mathbb R$.


```math
\boxed{\forall u,\ \varphi(u)=u_m,\qquad\varphi=\operatorname{ev}_m.}
```



## Exercice 36

### 1



```math
\varphi(\lambda)=\varphi(\lambda1_{\mathbb K})=\lambda\varphi(1)=\lambda1_B.
```


L'unique morphisme est l'application structurale $\lambda\mapsto\lambda1_B$.

### 2



```math
\varphi\left(\sum_ka_kX^k\right)=\sum_ka_k\varphi(X)^k.
```


Chaque morphisme est déterminé par $b=\varphi(X)$. Réciproquement, pour tout $b\in B$, l'évaluation $P\mapsto P(b)$ est un morphisme de $\mathbb K$-algèbres, les scalaires étant centraux.


```math
\boxed{\operatorname{Hom}_{\mathbb K\text{-alg}}(\mathbb K[X],B)\simeq B.}
```


