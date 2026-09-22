# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td22-dimension.pdf)

## Autocorrection A

### 1



```math
a=(1,-1,1),\quad b=(0,-1,2),\quad c=a+b.
```





```math
\lambda a+\mu b=0\implies\lambda=0\implies\mu=0.
```



$(a,b)$ est une base ; la dimension vaut $2$.

### 2



```math
\lambda a+\mu b=(\lambda,-\lambda-\mu,\lambda+2\mu),
\qquad x+2y+z=0.
```



Réciproquement, $x+2y+z=0$ donne



```math
(x,y,z)=x a+(-x-y)b.
```



## Autocorrection B

### 1

$(t,t,1)\ne0$, donc $\dim D_t=1$. Si



```math
\lambda(1,t,1)+\mu(2,1,1)=0,
```



les première et troisième coordonnées donnent $\lambda+2\mu=\lambda+\mu=0$ ; donc $\dim P_t=2$.

### 2



```math
D_t\oplus P_t=\mathbb R^3
\iff\det\begin{pmatrix}t&1&2\\t&t&1\\1&1&1\end{pmatrix}\ne0
\iff(t-1)^2\ne0
\iff\boxed{t\ne1}.
```



## Exercice 1

### (i)



```math
\det\begin{pmatrix}1&4&7&11\\2&-2&2&4\\1&1&4&1\\0&1&2&3\end{pmatrix}=-44\ne0.
```



Les quatre vecteurs donnés forment une base de $E=\mathbb R^4$ ; $\dim E=4$.

### (ii)



```math
y=\frac{2z-t}{3},\qquad x=\frac{7z-8t}{9}.
```





```math
F=\operatorname{Vect}\big((7,6,9,0),(-8,-3,0,9)\big),\qquad\dim F=2.
```



Ces deux vecteurs sont indépendants par leurs troisième et quatrième coordonnées.

## Exercice 2



```math
\dim\mathbb K^n=n=\#(e_1,\ldots,e_n).
```



Une famille génératrice de $n$ vecteurs est une base ; sa sous-famille $(e_2,\ldots,e_n)$ est libre.

## Exercice 3

La matrice de colonnes $u_1,\ldots,u_n$ est triangulaire supérieure, de diagonale $(1,\ldots,1)$ ; son déterminant vaut $1$. La famille est une base de $\mathbb K^n$.

## Exercice 4



```math
(E_{ij})_{1\le i,j\le n}\text{ base de }M_n(\mathbb K),\qquad\dim M_n(\mathbb K)=n^2.
```





```math
\begin{array}{c|c|c}
\text{Espace}&\text{Base}&\text{Dimension}\\\hline
D_n&(E_{ii})&n\\
T_n^+&(E_{ij})_{i\le j}&n(n+1)/2\\
T_n^-&(E_{ij})_{i\ge j}&n(n+1)/2\\
S_n&(E_{ii}),\ (E_{ij}+E_{ji})_{i<j}&n(n+1)/2\\
A_n&(E_{ij}-E_{ji})_{i<j}&n(n-1)/2
\end{array}
```



La ligne $A_n$ suppose $\operatorname{car}\mathbb K\ne2$ ; en caractéristique $2$, $A_n=S_n$.



```math
\operatorname{tr}(E_{11})=1\implies\operatorname{rg}(\operatorname{tr})=1
\implies\dim\mathfrak{sl}_n=n^2-1.
```



Une base est $(E_{ij})_{i\ne j}$ complétée par $(E_{ii}-E_{nn})_{i<n}$.

## Exercice 5

Les sommes des lignes et colonnes sont linéaires ; leur égalité définit un sous-espace. Pour $n\ge2$, choisir librement $m$ et $(a_{ij})_{i,j<n}$ impose



```math
a_{in}=m-\sum_{j<n}a_{ij},\qquad
a_{nj}=m-\sum_{i<n}a_{ij},\qquad
a_{nn}=\sum_{i,j<n}a_{ij}-(n-2)m.
```



Toutes les lignes et colonnes ont alors somme $m$. Cette paramétrisation est un isomorphisme :



```math
\boxed{\dim\mathcal M=(n-1)^2+1}.
```



Pour $n=1$, $\mathcal M=M_1(\mathbb R)$, de dimension $1$.

## Exercice 6

### 1



```math
P_T=\ker(u\mapsto(u_{n+T}-u_n)_n),\qquad
P_T\longrightarrow\mathbb K^T,\quad u\longmapsto(u_0,\ldots,u_{T-1})
```



est un isomorphisme ; $\dim P_T=T$.

### 2

Ici $\mathbb K=\mathbb C$ ; plus généralement, $X^T-1$ doit avoir $T$ racines distinctes dans $\mathbb K$.



```math
e_\omega=(\omega^n)_{n\ge0}\in P_T,\qquad
\det(\omega_j^{i-1})_{1\le i,j\le T}=\prod_{i<j}(\omega_j-\omega_i)\ne0.
```



Les $T$ suites $e_\omega$, $\omega\in\mathbb U_T$, forment une base.

### 3

Lire $P$, et non $T$.



```math
u\in P_r,\ v\in P_s\implies\alpha u+\beta v\in P_{\operatorname{ppcm}(r,s)}.
```



Sur $\mathbb C$,



```math
\boxed{\big((\omega^n)_{n\ge0}\big)_{\omega\in\bigcup_{T\ge1}\mathbb U_T}\text{ est une base de }P.}
```



Toute suite périodique appartient à un $P_T$, donc à l'espace engendré. Toute sous-famille finie de racines distinctes est libre par le déterminant de Vandermonde sur les premières coordonnées.

Sur $\mathbb R$, une base est constituée de $(1)_n$, $((-1)^n)_n$ et



```math
\big(\cos(2\pi rn)\big)_n,\quad\big(\sin(2\pi rn)\big)_n,
\qquad r\in\mathbb Q\cap(0,1/2).
```



Elle s'obtient en remplaçant chaque paire $e^{\pm2\pi irn}$ par sa partie réelle et sa partie imaginaire.

## Exercice 7

### 1

Les deux premières valeurs déterminent une unique suite par récurrence ; l'application



```math
R\longrightarrow\mathbb K^2,\qquad u\longmapsto(u_0,u_1)
```



est un isomorphisme. Pour une racine $r$, la suite $(r^n)_n$, avec $r^0=1$, vérifie la relation.



```math
\det\begin{pmatrix}1&1\\\rho&\sigma\end{pmatrix}=\sigma-\rho\ne0.
```



Donc $\dim R=2$ et les deux suites géométriques forment une base.

### 2

Lire $\rho_1,\ldots,\rho_k$ et $\mathbb K^{\mathbb N}$.



```math
R'\overset\sim\longrightarrow\mathbb K^k,\qquad u\longmapsto(u_0,\ldots,u_{k-1}),
\qquad\dim R'=k.
```





```math
\det(\rho_j^{i-1})_{1\le i,j\le k}=\prod_{i<j}(\rho_j-\rho_i)\ne0.
```



Une base est $\big((\rho_j^n)_{n\ge0}\big)_{1\le j\le k}$.

## Autocorrection C

On suppose $\operatorname{car}\mathbb K\ne2$.

### 1–2

Pour $\sigma(P)=P(-X)$,



```math
\mathcal P=\ker(\sigma-I),\qquad\mathcal I=\ker(\sigma+I),\qquad
P\in\mathcal P\cap\mathcal I\implies2P=0\implies P=0.
```



### 3–4



```math
(1,X^2,\ldots,X^{2n})\subset\mathcal P,\qquad
(X,X^3,\ldots,X^{2n-1})\subset\mathcal I
```



sont libres. Donc



```math
2n+1\ge\dim(\mathcal P\oplus\mathcal I)
=\dim\mathcal P+\dim\mathcal I\ge(n+1)+n=2n+1.
```



Toutes les inégalités sont des égalités : les deux familles sont des bases et $\mathbb K_{2n}[X]=\mathcal P\oplus\mathcal I$. En caractéristique $2$, les deux espaces sont égaux à $\mathbb K_{2n}[X]$ et la somme n'est pas directe.

## Exercice 8

Lire $y_n$ au dernier terme de la famille.



```math
\operatorname{Vect}(x_i+y_i:1\le i\le n)
\subset\operatorname{Vect}(x_1,\ldots,x_n,y_1,\ldots,y_n).
```



Le premier espace a dimension $n$ ; le second a donc dimension au moins $n$.

## Exercice 9

### 1

Compléter une base de $E$ en prélevant des vecteurs dans la base canonique, qui engendre $\mathbb K^n$. Les vecteurs ajoutés engendrent un supplémentaire de $E$.

### 2



```math
G=\operatorname{Vect}(e_1,e_2).
```



Pour $(x,y,0,0)\in F\cap G$, les équations donnent $y=0$, puis $x=0$. Les deux équations de $F$ sont indépendantes, donc $\dim F=2=\dim G$ et $F\oplus G=\mathbb K^4$.

## Exercice 10

### 1



```math
\dim(F\cap G)=\dim F+\dim G-\dim(F+G)
\ge\dim F+\dim G-\dim E>0.
```



### 2



```math
\dim(F\cap G\cap H)
\ge\dim(F\cap G)+\dim H-\dim E
\ge\dim F+\dim G+\dim H-2\dim E.
```



La condition $\boxed{\dim F+\dim G+\dim H>2\dim E}$ suffit.

## Exercice 11

### 1

Si $H=H'$, la dimension vaut $n-1$. Sinon, $H+H'=E$, donc



```math
\dim(H\cap H')=2(n-1)-n=n-2.
```



### 2

Les deux formes données ne sont pas proportionnelles : la première a un coefficient de $e$ nul, la seconde un coefficient $5$. Elles sont indépendantes et l'intersection a dimension $9-2=\boxed7$.

### 3

Écrire $H_i=\ker\ell_i$ et $L=(\ell_1,\ldots,\ell_r):E\to\mathbb K^r$ :



```math
\dim\bigcap_{i=1}^rH_i=\dim\ker L=n-\operatorname{rg}L\ge n-r.
```



### 4



```math
\boxed{D=\ker(x-2y)\cap\ker(z+y)\cap\ker t.}
```



Les solutions sont $(2s,s,-s,0)$, $s\in\mathbb R$.

## Exercice 12

Si $E=F\oplus G=F\oplus H$, soit $p$ la projection sur $H$ parallèlement à $F$. Alors



```math
p|_G:G\to H,\qquad\ker(p|_G)=G\cap F=0.
```



Pour $h\in H$, écrire $h=f+g$ ; alors $h=p(h)=p(g)$. Ainsi $p|_G$ est un isomorphisme, même sans hypothèse de dimension finie.

## Exercice 13

Réunir des bases de $F$ et de $G$, puis compléter cette famille libre par $h_1,\ldots,h_s$. Poser



```math
\widehat F=F\oplus\operatorname{Vect}(h_1,\ldots,h_s).
```



Alors $F\subset\widehat F$ et $E=\widehat F\oplus G$.

## Exercice 14

Pour $d=\dim(F\cap G)$,



```math
0\le d\le\min(p,q),\qquad p+q-d=\dim(F+G)\le n.
```



Réciproquement, pour tout entier



```math
\boxed{\max(0,p+q-n)\le d\le\min(p,q)},
```



dans une base $(e_i)_{1\le i\le n}$, prendre



```math
F=\operatorname{Vect}(e_1,\ldots,e_p),\qquad
G=\operatorname{Vect}(e_1,\ldots,e_d,e_{p+1},\ldots,e_{p+q-d}).
```



Leur intersection est de dimension $d$.

## Exercice 15

### 1

Initialement, la famille $(f_j)_{1\le j\le m}$ engendre $E$. Supposons $e_1,\ldots,e_{r-1}$ déjà insérés. Dans la famille génératrice obtenue,



```math
e_r=\sum_{k<r}\alpha_ke_k+\sum_{j\notin\{i_1,\ldots,i_{r-1}\}}\beta_jf_j.
```



Au moins un $\beta_{i_r}$ est non nul, sinon $e_r\in\operatorname{Vect}(e_1,\ldots,e_{r-1})$. L'égalité permet d'exprimer $f_{i_r}$ à l'aide de $e_r$ et des autres vecteurs. Son remplacement préserve donc le caractère générateur. Cela établit la récurrence jusqu'à $r=n$.

### 2

Les indices $i_1,\ldots,i_n$ sont distincts : $n\le m$. Les vecteurs libres remplacent successivement autant de vecteurs de la famille génératrice ; si $n=m$, $(e_1,\ldots,e_n)$ engendre $E$ et constitue une base.

## Autocorrection D

### 1–3



```math
f=\begin{pmatrix}1&0&-1&0\\0&1&0&-1\end{pmatrix},\qquad
\ker f=\operatorname{Vect}\big((1,0,1,0),(0,1,0,1)\big).
```



Ces deux vecteurs sont libres ; $\dim\ker f=2$, donc $\operatorname{rg}f=4-2=2$ : $f$ est surjective.

### 4–5



```math
G=\operatorname{Vect}(e_1,e_4),\qquad\dim G=2.
```





```math
(x,0,0,t)\in\ker f\implies(x,-t)=(0,0).
```



Ainsi $\ker f\cap G=0$, puis $\mathbb K^4=\ker f\oplus G$.

## Exercice 16

### 1



```math
(f^2+f+I)(f-I)=f^3-I=0
\implies\operatorname{im}(f-I)\subset\ker(f^2+f+I).
```



### 2

Pour $x\in\operatorname{im}(f-I)\cap\ker(f-I)$,



```math
0=(f^2+f+I)x=3x.
```



Si $\operatorname{car}\mathbb K\ne3$, l'intersection est nulle. Le théorème du rang donne la somme des dimensions égale à $\dim E$, donc la supplémentarité.

En caractéristique $3$, l'assertion est fausse : sur $\mathbb K^2$, $f=I+E_{12}$ vérifie $f^3=I$, mais $\operatorname{im}(f-I)=\ker(f-I)=\mathbb K e_1$.

## Exercice 17

### 1

Si $E=\ker u\oplus\operatorname{im}u$, $u|_{\operatorname{im}u}$ est injective. Pour $ux$, écrire $x=k+uy$ : $ux=u^2y$, donc $\operatorname{im}u=\operatorname{im}u^2$. De plus



```math
u^2x=0\implies ux\in\ker u\cap\operatorname{im}u=0,
```



d'où $\ker u^2=\ker u$.

Réciproquement, $uy\in\ker u$ donne $y\in\ker u^2=\ker u$, donc $uy=0$. Enfin, pour $x\in E$, choisir $y$ tel que $ux=u^2y$ ; alors



```math
x=(x-uy)+uy\in\ker u+\operatorname{im}u.
```



### 2

En dimension finie,



```math
\operatorname{im}u^2\subset\operatorname{im}u,\quad\ker u\subset\ker u^2,
\quad\operatorname{rg}u^2=\dim E-\dim\ker u^2.
```



L'égalité de l'une des deux paires équivaut à celle des dimensions, donc à l'égalité de l'autre paire ; appliquer 1.

### 3

Sur $\mathbb K[X]$, $u(P)=XP$ est injectif, mais $X^2\mathbb K[X]\ne X\mathbb K[X]$. Inversement,



```math
v(P)=\frac{P-P(0)}X
```



est surjectif, tandis que $\ker v=\mathbb K$ et $\ker v^2=\mathbb K_1[X]$.

## Exercice 18

### 1

Noter $n=\dim E$, $r=\operatorname{rg}u$, $s=\operatorname{rg}v$. Les deux sommes donnent



```math
n\le r+s,\qquad n\le(n-r)+(n-s)\implies r+s=n.
```



La formule de Grassmann donne alors



```math
\dim(\operatorname{im}u\cap\operatorname{im}v)=r+s-n=0,
```





```math
\dim(\ker u\cap\ker v)=(n-r)+(n-s)-n=0.
```



### 2

Dans $E=\bigoplus_{j\ge0}\mathbb K e_j$, définir



```math
u(e_{2j})=e_j,\quad u(e_{2j+1})=0,\qquad
v(e_{2j})=0,\quad v(e_{2j+1})=e_j.
```



Les noyaux sont supplémentaires ; $u$ et $v$ sont surjectifs. Ainsi les deux sommes valent $E$, mais $\operatorname{im}u=\operatorname{im}v=E\ne0$.

## Exercice 19

Sur $\mathbb K_n[X]$, $D^{n+1}=0$ et



```math
(I-D)^{-1}=I+D+\cdots+D^n.
```



D'où



```math
\boxed{P_n=\sum_{k=0}^nD^k(X^n)=\sum_{k=0}^n n(n-1)\cdots(n-k+1)X^{n-k}.}
```



En caractéristique nulle, $P_n=n!\sum_{j=0}^nX^j/j!$. Tout polynôme non nul $Q$ vérifie $\deg(Q-Q')=\deg Q$ ; toute solution a donc degré $n$, ce qui établit l'unicité dans $\mathbb K[X]$ entier.

## Exercice 20

### 1



```math
\ker(u|_V)=V\cap\ker u,\qquad\operatorname{im}(u|_V)=u[V].
```



Le théorème du rang donne $\dim u[V]=\dim V-\dim(V\cap\ker u)$.

### 2



```math
u:u^{-1}[W]\longrightarrow W\cap\operatorname{im}u
```



est surjective, de noyau $\ker u$. Donc



```math
\dim u^{-1}[W]=\dim(W\cap\operatorname{im}u)+\dim\ker u.
```



## Exercice 21

### 1

Prendre $E'=F$ et $\varphi:F\hookrightarrow E$ l'inclusion.

### 2

Choisir $E=G\oplus H$, $E''=H$, et $\psi(g+h)=h$. Alors $\ker\psi=G$.

### 3

Nécessairement $\dim F+\dim G=\dim E$. Réciproquement, choisir $E=G\oplus H$ et un isomorphisme $a:H\to F$, puis



```math
u(g+h)=a(h).
```



Ainsi



```math
\boxed{\exists u:\operatorname{im}u=F,\ \ker u=G\iff\dim F+\dim G=\dim E.}
```



## Exercice 22

On suppose $\operatorname{car}\mathbb K\ne2$.

$(i)\Rightarrow(ii)$ : $\operatorname{im}u\subset\ker u$. Prendre un projecteur $p$ sur $\operatorname{im}u$ ; alors $pu=u$ et $up=0$.

$(ii)\Rightarrow(iii)$ est immédiat.

$(iii)\Rightarrow(ii)$ : multiplier $pu-up=u$ à gauche, puis à droite, par $p$ :



```math
pup=0,\qquad pup=2up\implies up=0,\qquad pu=u.
```



Enfin $u^2=upu=0$.

En caractéristique $2$, prendre



```math
p=\begin{pmatrix}1&0\\0&0\end{pmatrix},\qquad
u=\begin{pmatrix}0&1\\1&0\end{pmatrix}.
```



Alors $pu-up=u$, mais $u^2=I$ ; l'équivalence ne subsiste pas.

## Exercice 23

### 1



```math
v=w\circ u,\quad x\in\ker u\implies v(x)=w(0)=0.
```



### 2

Choisir $E=\ker u\oplus S$ et $F=\operatorname{im}u\oplus T$. La restriction $u|_S:S\to\operatorname{im}u$ est un isomorphisme. Poser



```math
w(y+t)=v\big((u|_S)^{-1}y\big),\qquad y\in\operatorname{im}u,\ t\in T.
```



Pour $x=k+s$, $k\in\ker u$, $s\in S$,



```math
w(ux)=v(s)=v(x),
```



car $\ker u\subset\ker v$. Donc $v=w\circ u$.

## Exercice 24



```math
U:V\to\mathbb R^n,\quad U(x)=(f_1(x),\ldots,f_n(x)),\qquad\ker U\subset\ker f.
```



Par l'exercice 23, $f=w\circ U$ pour une forme $w$ sur $\mathbb R^n$. Avec $\lambda_i=w(e_i)$,



```math
\boxed{f=\sum_{i=1}^n\lambda_i f_i}.
```



## Exercice 25

Si $\operatorname{im}f=\ker f$, alors $f^2=0$. Choisir une base $(e_i)_{1\le i\le r}$ de cet espace et des $g_i$ tels que $f(g_i)=e_i$. Le théorème du rang donne $\dim E=2r$ ; la famille $(e_i,g_i)$ est libre, donc une base. Poser



```math
h(e_i)=g_i,\qquad h(g_i)=0.
```



Alors $(hf+fh)e_i=e_i$ et $(hf+fh)g_i=g_i$, donc $hf+fh=I$.

Réciproquement, $f^2=0$ donne $\operatorname{im}f\subset\ker f$. Si $x\in\ker f$,



```math
x=(hf+fh)x=fhx\in\operatorname{im}f.
```



## Exercice 26

Pour toute droite $D$, choisir un projecteur $p_D$ sur $D$. L'égalité $up_D=p_Du$ entraîne $u(D)\subset D$. Ainsi $u(x)=\lambda_xx$ pour $x\ne0$.

Pour $x,y$ indépendants,



```math
\lambda_{x+y}(x+y)=u(x+y)=\lambda_xx+\lambda_yy
\implies\lambda_x=\lambda_y=\lambda_{x+y}.
```



Pour des vecteurs proportionnels non nuls, l'égalité des scalaires vient de la linéarité. Donc $u=\lambda I$ ; le cas $E=0$ est immédiat.

## Exercice 27

### 1

Deux sous-espaces sont équivalents exactement lorsqu'ils ont même dimension : envoyer une base adaptée du premier sur une base adaptée du second. Les classes sont indexées par $0,\ldots,\dim E$.

### 2

Les invariants complets sont



```math
\boxed{(\dim F,\dim G,\dim(F\cap G))}.
```



En effet, une base de $F\cap G$, prolongée séparément dans $F$ et $G$, puis dans $E$, donne une base adaptée au couple. Deux couples de mêmes invariants possèdent des bases adaptées de mêmes longueurs, que l'on peut envoyer l'une sur l'autre.

### 3

Écrire $E=F_1\oplus F_2$. La projection $F_3\to F_1$ parallèlement à $F_2$ est un isomorphisme. Ainsi



```math
F_3=\{x+h(x):x\in F_1\},
```



où $h:F_1\to F_2$ est injective puisque $F_3\cap F_1=0$, donc bijective. Pour une base $(e_i)$ de $F_1$, poser $f_i=h(e_i)$. La base $(e_i,f_i)$ met le triplet sous la forme



```math
\big(\operatorname{Vect}(e_i),\operatorname{Vect}(f_i),\operatorname{Vect}(e_i+f_i)\big).
```



### 4

Pour $r\ge1$, dans $E=\mathbb R^r\oplus\mathbb R^r$, poser



```math
A=\mathbb R^r\oplus0,\quad B=0\oplus\mathbb R^r,\quad
C=\{(x,x)\},\quad D_\lambda=\{(x,\lambda x)\},\quad\lambda\in\mathbb R\setminus\{0,1\}.
```



Les quatre espaces ont dimension $r$ et leurs intersections deux à deux sont nulles. Un automorphisme conservant $A$ et $B$ a la forme $(x,y)\mapsto(Sx,Ty)$. La conservation de $C$ impose $S=T$ ; il conserve alors chaque $D_\lambda$. Donc



```math
(A,B,C,D_\lambda)\sim(A,B,C,D_\mu)\iff\lambda=\mu.
```



Il existe une infinité de classes. Pour $r=0$, cette assertion est fausse : il n'existe qu'un quadruplet.

## Exercice 28



```math
V_p\subset V_q=V_p+\operatorname{Vect}(u_{p+1},\ldots,u_q),
\qquad V_j=\operatorname{Vect}(u_1,\ldots,u_j).
```





```math
\dim V_p\le\dim V_q\le\dim V_p+q-p.
```



## Exercice 29

La restriction $b:\ker(ab)\to\ker a\cap\operatorname{im}b$ est surjective et a pour noyau $\ker b$. Donc



```math
\dim\ker(ab)=\dim\ker b+\dim(\ker a\cap\operatorname{im}b)
\le\dim\ker b+\dim\ker a.
```



## Exercice 30



```math
\operatorname{rg}(gf)=r-\dim(\operatorname{im}f\cap\ker g).
```



L'exercice 14, avec les dimensions $r$ et $n-s$, donne



```math
\boxed{R(r,s)=\{t\in\mathbb Z:\max(0,r+s-n)\le t\le\min(r,s)\}}.
```



Réalisation : dans une base $(e_i)$, prendre $f$ projection sur $\operatorname{Vect}(e_1,\ldots,e_r)$ ; définir $g$ non nul exactement sur



```math
e_1,\ldots,e_t,\ e_{r+1},\ldots,e_{r+s-t},
```



en envoyant ces $s$ vecteurs sur $e_1,\ldots,e_s$, respectivement. Les bornes sur $t$ assurent $r+s-t\le n$ ; alors $\operatorname{rg}g=s$ et $\operatorname{rg}(gf)=t$.

## Exercice 31

Poser $B=\operatorname{im}(vw)\subset A=\operatorname{im}v$. Alors



```math
\dim u(A)-\dim u(B)
=\dim A-\dim B-\big(\dim(A\cap\ker u)-\dim(B\cap\ker u)\big)
\le\dim A-\dim B.
```



Donc



```math
\boxed{\operatorname{rg}(uv)+\operatorname{rg}(vw)\le\operatorname{rg}v+\operatorname{rg}(uvw)}.
```



## Exercice 32



```math
\Phi:\mathbb K[X]\to\mathbb K\times\mathbb K[X],\qquad
P\mapsto\left(P(0),\frac{P-P(0)}X\right)
```



est linéaire, d'inverse $(a,Q)\mapsto a+XQ$. Une dimension finie $d$ imposerait $d=1+d$, contradiction.

## Exercice 33

Les fonctions $x\mapsto x^n$, $n\ge0$, sont continues. Une combinaison linéaire finie nulle est un polynôme ayant une infinité de racines, donc tous ses coefficients sont nuls. Cette famille libre infinie impose $\dim C^0(\mathbb R)=\infty$.

## Exercice 34

### 1

Choisir une base $\mathcal B$ de $E$ et des éléments distincts $e_n\in\mathcal B$, $n\ge0$. Poser



```math
H_n=\operatorname{Vect}(\mathcal B\setminus\{e_n\}).
```



Chaque $H_n$ est un hyperplan. Tout vecteur a un support fini dans $\mathcal B$, donc sa coordonnée selon au moins un $e_n$ est nulle :



```math
\boxed{E=\bigcup_{n\ge0}H_n}.
```



### 2

Pour $d=\dim E\ge1$, identifier $E$ à $\mathbb R^d$ et poser



```math
c(t)=(1,t,\ldots,t^{d-1}).
```



Si $H_n=\ker\ell_n$, $\ell_n\ne0$, alors $\ell_n(c(t))$ est un polynôme non nul de degré au plus $d-1$. L'ensemble des $t$ tels que $c(t)\in H_n$ est fini. Une réunion dénombrable de tels ensembles est dénombrable ; elle ne peut être $\mathbb R$. Donc $\bigcup_nH_n\ne E$. Pour $E=0$, il n'existe aucun hyperplan.

## Exercice 35

En dimension finie, une base et sa base duale donnent un isomorphisme $E\simeq E^*$.

Supposons $\kappa=\dim E$ infinie et fixons une base indexée par $I$, $|I|=\kappa$. Toute fonction $I\to\mathbb K$ se prolonge uniquement en une forme linéaire, donc



```math
E^*\simeq\mathbb K^I.
```



Si $|\mathbb K|\le\kappa$, les combinaisons linéaires finies donnent $|E|=\kappa$, tandis que



```math
|E^*|=|\mathbb K|^\kappa\ge2^\kappa>\kappa
```



par le théorème de Cantor. Les ensembles, donc les espaces, ne sont pas isomorphes.

Si $|\mathbb K|>\kappa$, choisir des indices distincts $i_0,i_1,\ldots\in I$. Pour chaque $a\in\mathbb K$, définir $\ell_a\in E^*$ par



```math
\ell_a(e_{i_n})=a^n\quad(n\ge0),\qquad
\ell_a(e_i)=0\quad\big(i\notin\{i_n:n\ge0\}\big),
```



avec $a^0=1$. Pour $a_1,\ldots,a_m$ distincts, une relation $\sum_jc_j\ell_{a_j}=0$, évaluée en $e_{i_0},\ldots,e_{i_{m-1}}$, donne un système de Vandermonde de déterminant



```math
\prod_{j<k}(a_k-a_j)\ne0.
```



La famille $(\ell_a)_{a\in\mathbb K}$ est libre, donc



```math
\dim E^*\ge|\mathbb K|>\kappa=\dim E.
```



Dans les deux cas, $E\not\simeq E^*$.

## Exercice 36

Correction de domaine : $b\in\mathcal L(E,G)$ ; avec le domaine $F$ imprimé, $b(x)$ n'est pas défini pour $x\in E$ en général.



```math
\dim(\ker a\cap\ker b)
\ge\dim\ker a+\dim\ker b-\dim E
=\dim E-\operatorname{rg}a-\operatorname{rg}b>0.
```



Tout vecteur non nul de cette intersection convient.

## Exercice 37



```math
T:\mathbb R^3\to\mathbb R^2,\qquad
(\lambda,\mu,\nu)\mapsto\big((\lambda A+\mu B+\nu C)_{21},\operatorname{tr}(\lambda A+\mu B+\nu C)\big).
```





```math
\dim\ker T\ge3-2=1.
```



Tout triplet non nul du noyau donne la matrice demandée ; celle-ci peut être nulle.

## Exercice 38

### 1



```math
Je_1=0,\qquad Je_j=e_{j-1}\quad(2\le j\le n+1).
```





```math
\operatorname{rg}J=n,\quad\ker J=\mathbb K e_1,\quad
\operatorname{im}J=\operatorname{Vect}(e_1,\ldots,e_n).
```



Sur $\mathbb K_n[X]$, l'endomorphisme associé est



```math
P\longmapsto\frac{P-P(0)}X.
```



### 2(a)

Lire $M\in M_{n+1}(\mathbb C)$ ; on suppose $n\ge1$.



```math
n=\operatorname{rg}M^2\le\operatorname{rg}M\le n+1.
```



$M$ n'est pas inversible, car $M^2=J$ ne l'est pas ; donc $\operatorname{rg}M=n$. Les inclusions et dimensions imposent



```math
\ker M=\ker J=\mathbb C e_1,\qquad\operatorname{im}M=\operatorname{im}J.
```



### 2(b)



```math
0\ne e_1\in\ker M\cap\operatorname{im}M.
```



Par le théorème du rang appliqué à $M|_{\operatorname{im}M}$,



```math
\operatorname{rg}M^2=\operatorname{rg}M-\dim(\ker M\cap\operatorname{im}M)=n-1,
```



contradiction. Pour $n=0$, $J=(0)$ possède bien la racine carrée $(0)$.

## Exercice 39

En dimensions finies, considérer



```math
\Sigma:F_1\times\cdots\times F_p\to F_1+\cdots+F_p,\qquad
(x_1,\ldots,x_p)\mapsto\sum_i x_i.
```



Elle est surjective et



```math
\dim\ker\Sigma=\sum_i\dim F_i-\dim\left(\sum_iF_i\right).
```



La somme est directe exactement lorsque $\ker\Sigma=0$, d'où l'équivalence.

Sans finitude des dimensions, la réciproque est fausse : pour $F_1=F_2=E=\mathbb K[X]$, la somme n'est pas directe alors que



```math
\dim(F_1+F_2)=\aleph_0=\aleph_0+\aleph_0=\dim F_1+\dim F_2.
```



## Exercice 40

### 1



```math
T:E\to\mathbb R^2,\qquad f\mapsto(f(0),f(1)).
```



Si $f\in\ker T$, la monotonie et $f(0)=f(1)=0$ imposent $f=0$ sur $[0,1]$. L'application $T$ est injective, donc $\dim E\le2$.

### 2

Supposons trois fonctions $f_1,f_2,f_3$ indépendantes. Les vecteurs



```math
(f_1(x),f_2(x),f_3(x)),\qquad x\in\mathbb R,
```



engendrent $\mathbb R^3$ : sinon un vecteur non nul orthogonal à leur espace fournirait une relation entre les fonctions. Choisir donc $x_1,x_2,x_3$ tels que la matrice d'évaluation soit inversible, puis $a=\min x_i$, $b=\max x_i$.

Deux équations homogènes à trois inconnues admettent une solution $(c_1,c_2,c_3)\ne0$ telle que



```math
f=\sum_{i=1}^3c_if_i,\qquad f(a)=f(b)=0.
```



La monotonie donne $f=0$ sur $[a,b]$, donc $f(x_j)=0$ pour les trois points. L'inversibilité de la matrice impose $c_1=c_2=c_3=0$, contradiction. Ainsi $\boxed{\dim E\le2}$ ; les fonctions affines atteignent cette borne.

## Exercice 41

Pour $F=\operatorname{Vect}(f_1,\ldots,f_n)$, $\dim F=n$. L'application de dérivation $D:F\to\mathbb R^{\mathbb R}$ a un noyau formé de fonctions constantes, donc de dimension au plus $1$.



```math
\boxed{\operatorname{rg}(f_1',\ldots,f_n')=\operatorname{rg}(D|_F)
=n-\dim\ker(D|_F)\ge n-1}.
```



## Exercice 42

La finitude fournit un plus petit entier $p\ge1$ tel que $p1_{\mathbb K}=0$. Il est premier : une factorisation $p=ab$ avec $1<a,b<p$ donnerait



```math
(a1_{\mathbb K})(b1_{\mathbb K})=0,
```



contrairement à l'intégrité et à la minimalité de $p$. L'application $\mathbb F_p\hookrightarrow\mathbb K$, $\bar m\mapsto m1_{\mathbb K}$, fait de $\mathbb K$ un espace vectoriel de dimension finie $d\ge1$ sur $\mathbb F_p$. Une base donne une bijection $\mathbb F_p^d\to\mathbb K$, donc



```math
\boxed{|\mathbb K|=p^d}.
```


