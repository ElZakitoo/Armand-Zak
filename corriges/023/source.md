# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td23-representation-matricielle.pdf)

## Autocorrection A

### 1



```math
A=\begin{pmatrix}1&0&-1\\0&1&0\\0&1&0\end{pmatrix}.
```



### 2



```math
A^2=\begin{pmatrix}1&-1&-1\\0&1&0\\0&1&0\end{pmatrix},\quad A^3=\begin{pmatrix}1&-2&-1\\0&1&0\\0&1&0\end{pmatrix},\quad A^4=\begin{pmatrix}1&-3&-1\\0&1&0\\0&1&0\end{pmatrix}.
```



Pour $n\ge1$, posons $B_n=\begin{pmatrix}1&1-n&-1\\0&1&0\\0&1&0\end{pmatrix}$. Alors $B_1=A$ et $B_nA=B_{n+1}$, donc $A^n=B_n$.

### 3



```math
f^0=\operatorname{id},\qquad n\ge1:\quad f^n(x,y,z)=(x+(1-n)y-z,y,y).
```



## Autocorrection B

### 1



```math
A=I+N,\quad N^3=0,\qquad A^{-1}=I-N+N^2=\begin{pmatrix}1&-1&2\\0&1&-2\\0&0&1\end{pmatrix}.
```



### 2



```math
\Delta(1)=1,\quad\Delta(X)=1+X,\quad\Delta(X^2)=2X+X^2,\qquad\operatorname{Mat}(\Delta)=A.
```





```math
[P]=A^{-1}\begin{pmatrix}1\\1\\2\end{pmatrix}=\begin{pmatrix}4\\-3\\2\end{pmatrix},\qquad \boxed{P=4-3X+2X^2}.
```



## Autocorrection C

### 1



```math
P=\begin{pmatrix}1&0&1&1\\0&0&1&0\\0&1&1&0\\0&1&1&1\end{pmatrix},\quad Q=\begin{pmatrix}1&1&1\\1&1&0\\1&0&0\end{pmatrix},\qquad\det P=\det Q=-1.
```



### 2(a)



```math
u=ab_1+bb_2+cb_3+db_4\iff\begin{cases}a+c+d=1,\\c=-2,\\b+c=5,\\b+c+d=6.\end{cases}
```





```math
(a,b,c,d)=(2,7,-2,1).
```



### 2(b)



```math
[v]_{\rm can}=P[v]_{\mathcal B},\quad P^{-1}=\begin{pmatrix}1&-1&1&-1\\0&-1&1&0\\0&1&0&0\\0&0&-1&1\end{pmatrix},\quad [u]_{\mathcal B}=P^{-1}[u]_{\rm can}=\begin{pmatrix}2\\7\\-2\\1\end{pmatrix}.
```



### 3



```math
F=\begin{pmatrix}1&-2&2&5\\1&-2&3&4\\-1&0&2&-3\end{pmatrix},\qquad\operatorname{Mat}_{\mathcal B,\mathcal C}(f)=Q^{-1}FP=\begin{pmatrix}-1&-1&-2&-4\\2&8&8&9\\0&0&0&1\end{pmatrix}.
```



## Exercice 1

### 1



```math
2=\operatorname{rg}(AB)\le\min(\operatorname{rg}A,\operatorname{rg}B)\le2,\qquad\operatorname{rg}A=\operatorname{rg}B=2.
```



### 2



```math
\ker(AB)=\mathbb Re_1,\quad\operatorname{im}(AB)=\operatorname{Vect}(e_2,e_3).
```



$A$ est injective, donc $\ker B=\ker(AB)$. L'inclusion $\operatorname{im}(AB)\subset\operatorname{im}A$ et l'égalité des dimensions donnent $\operatorname{im}A=\operatorname{Vect}(e_2,e_3)$.

### 3

$AB$ vaut l'identité sur $\operatorname{im}A$, donc $ABA=A$. Ainsi $A(BA-I_2)=0$ et, par injectivité de $A$, $\boxed{BA=I_2}$.

## Exercice 2

Les opérations de dérivation, évaluation, substitution et multiplication par un polynôme fixé sont linéaires.

### 1



```math
L(1)=-1,\quad L(X)=2X^3,\quad L(X^2)=4X^4+2X^2-1,\quad L(X^3)=6X^5+3X^4-1.
```





```math
\operatorname{Mat}(L)=\begin{pmatrix}-1&0&-1&-1\\0&0&0&0\\0&0&2&0\\0&2&0&0\\0&0&4&3\\0&0&0&6\end{pmatrix}\in M_{6,4}(K).
```



### 2



```math
\operatorname{Mat}(L)=\begin{pmatrix}1&-1&1&-1\\0&1&2&6\end{pmatrix}.
```



### 3



```math
L(X^j)=jX^j,\qquad\operatorname{Mat}(L)=\operatorname{diag}(0,1,\ldots,n).
```



### 4



```math
L(X^j)=(j+2)X^j-jX^{j-1}.
```



Dans la base indexée de $0$ à $n$, les seuls coefficients éventuellement non nuls sont $a_{j,j}=j+2$ et $a_{j-1,j}=-j$ pour $j\ge1$. Les degrés restent inférieurs ou égaux à $n$.

## Exercice 3

### 1



```math
\sum_{k=0}^na_kx^ke^{\alpha x}=0\ (x\in\mathbb R)\iff\sum_{k=0}^na_kx^k=0\iff a_0=\cdots=a_n=0.
```



Donc $(f_0,\ldots,f_n)$ est une base et $\dim E=n+1$.

### 2



```math
\partial f_0=\alpha f_0,\qquad\partial f_k=\alpha f_k+kf_{k-1}\quad(k\ge1).
```



La matrice est triangulaire, de diagonale constante $\alpha$ :



```math
\det(\partial_{|E})=\alpha^{n+1},\qquad\partial_{|E}\in GL(E)\iff\alpha\ne0.
```



## Exercice 4

### 1

Toute paire $(u_0,u_1)$ définit une unique suite de $F$. L'application $u\mapsto(u_0,u_1)$ est donc un isomorphisme $F\simeq\mathbb R^2$. Soient $a,b$ les suites associées à $(1,0)$ et $(0,1)$ ; $\mathcal B=(a,b)$ est une base.

### 2–3



```math
u_{n+3}=u_{n+2}+u_{n+1}\Longrightarrow Tu\in F,\qquad (u_0,u_1)\longmapsto(u_1,u_0+u_1).
```





```math
\operatorname{Mat}_{\mathcal B}(T)=\begin{pmatrix}0&1\\1&1\end{pmatrix},\quad\det=-1,\qquad(T^{-1}u)_n=u_{n+1}-u_n.
```



## Exercice 5

Pour $A=(a_{ij})$, $AE_{ij}=\sum_k a_{ki}E_{kj}$. Donc



```math
\operatorname{Mat}(M\mapsto AM)=\begin{pmatrix}a&b&0&0\\c&d&0&0\\0&0&a&b\\0&0&c&d\end{pmatrix}.
```



Pour $A\in M_p(K)$ et $M\in M_{p,q}(K)$, dans la base ordonnée colonne par colonne :



```math
\operatorname{Mat}(M\mapsto AM)=\operatorname{diag}(A,\ldots,A)\quad(q\text{ blocs}).
```



## Exercice 6

### 1



```math
f(X^j)=j(j+1)X^j,\qquad\operatorname{Mat}(f)=\operatorname{diag}(0,2,6,12).
```



En caractéristique $0$ :



```math
\ker f=K\cdot1,\qquad\operatorname{im}f=\operatorname{Vect}(X,X^2,X^3).
```



Sur un corps quelconque, le noyau est engendré par les $X^j$ tels que $j(j+1)=0$ dans $K$, et l'image par les autres monômes.

### 2



```math
g(1)=-1-2X,\quad g(X)=-1-X-X^2,\quad g(X^2)=-2X-X^2.
```



Les termes de degré $3$ s'annulent ; $g$ est bien un endomorphisme et



```math
\operatorname{Mat}(g)=\begin{pmatrix}-1&-1&0\\-2&-1&-2\\0&-1&-1\end{pmatrix},\quad\det g=3.
```



Donc $g$ est un automorphisme si et seulement si $\operatorname{car}K\ne3$ ; en particulier sur $\mathbb R$ ou $\mathbb C$.

## Exercice 7

### 1



```math
\operatorname{im}f=\ker f\Longrightarrow n=\operatorname{rg}f+\dim\ker f=2\operatorname{rg}f.
```



Réciproquement, pour $n=2r$, dans une base $(e_1,\ldots,e_r,h_1,\ldots,h_r)$, poser $f(e_i)=0$, $f(h_i)=e_i$. Alors $\ker f=\operatorname{im}f=\operatorname{Vect}(e_1,\ldots,e_r)$.

### 2



```math
\operatorname{im}f=\ker f\Longrightarrow f^2=0,\quad\operatorname{rg}f=n/2.
```



Réciproquement, $f^2=0$ donne $\operatorname{im}f\subset\ker f$ ; les deux dimensions valent $n/2$, donc les espaces sont égaux.

## Exercice 8

### 1



```math
P\in\ker\varphi\Longrightarrow P(x_0)=\cdots=P(x_n)=0,\quad\deg P\le n\Longrightarrow P=0.
```



Les deux dimensions valent $n+1$, donc $\varphi$ est un isomorphisme. Explicitement,



```math
L_i(X)=\prod_{j\ne i}\frac{X-x_j}{x_i-x_j},\qquad\varphi^{-1}(y_0,\ldots,y_n)=\sum_{i=0}^ny_iL_i.
```



### 2



```math
\operatorname{Mat}(\varphi)=(x_i^j)_{0\le i,j\le n}=V(x_0,\ldots,x_n)\in GL_{n+1}(K).
```



## Autocorrection D

### 1–3



```math
P=\begin{pmatrix}0&1&1\\1&-1&-1\\1&1&0\end{pmatrix},\quad\det P=1,\quad P^{-1}=\begin{pmatrix}1&1&0\\-1&-1&1\\2&1&-1\end{pmatrix}.
```





```math
[x]_{\mathcal B}=P[x]_{\mathcal B'},\qquad D=P^{-1}AP=\operatorname{diag}(1,-1,-2).
```



### 4–5



```math
A=PDP^{-1},\qquad A^n=PD^nP^{-1}.
```



Avec $a=(-1)^n$, $b=(-2)^n$ :



```math
\boxed{A^n=\begin{pmatrix}-a+2b&-a+b&a-b\\1+a-2b&1+a-b&-a+b\\1-a&1-a&a\end{pmatrix}}.
```



## Exercice 9

### 1



```math
A=\begin{pmatrix}3&-4&-2\\4&-7&-4\\-5&10&6\end{pmatrix},\qquad A^2=A.
```





```math
\operatorname{im}f=\operatorname{Vect}((3,4,-5),(-4,-7,10)),\qquad\ker f=\operatorname{Vect}((-2,-4,5)).
```



Les deux premiers vecteurs sont indépendants ; le troisième engendre le noyau. Comme $f$ est un projecteur, leur concaténation est une base et sa matrice y vaut $\operatorname{diag}(1,1,0)$.

### 2



```math
g=2f-I,\qquad g^2=4f^2-4f+I=I.
```



Dans la même base, $\operatorname{Mat}(g)=\operatorname{diag}(1,1,-1)$.

## Exercice 10

### 1



```math
\varphi(1)=1,\quad\varphi(X)=1+2X,\quad\varphi(X^2)=4+2X+5X^2.
```





```math
A=\begin{pmatrix}1&1&4\\0&2&2\\0&0&5\end{pmatrix}.
```



### 2

Pour $P=a+bX+cX^2$, $\varphi(P)=\lambda P$ équivaut à



```math
(1-\lambda)a+b+4c=0,\quad(2-\lambda)b+2c=0,\quad(5-\lambda)c=0.
```





```math
E_1=\mathbb R\cdot1,\quad E_2=\mathbb R(1+X),\quad E_5=\mathbb R(7+4X+6X^2).
```



Pour $\lambda\notin\{1,2,5\}$, le système triangulaire n'a que la solution nulle.

### 3

Les degrés $0,1,2$ sont distincts : $(1,1+X,7+4X+6X^2)$ est une base, dans laquelle la matrice est $\operatorname{diag}(1,2,5)$.

## Exercice 11

### 1



```math
\exists\mathcal B:\ \operatorname{Mat}_{\mathcal B}(f)=I_n\iff f=\operatorname{id}_E.
```



### 2



```math
\operatorname{Mat}_{\mathcal B,\mathcal C}(f)=I_n\iff f(b_i)=c_i\ (1\le i\le n).
```



Ceci impose $f\in GL(E)$. Réciproquement, pour $f\in GL(E)$, choisir une base $\mathcal B$ et $\mathcal C=f(\mathcal B)$.

## Exercice 12

Soit $x\ne0$. Si $u(x)=\lambda x$ avec $\lambda\in\mathbb R$, alors $-x=u^2(x)=\lambda^2x$, impossible. Ainsi $(x,u(x))$ est une base et



```math
u(x)=u(x),\quad u(u(x))=-x,\qquad\operatorname{Mat}(u)=\begin{pmatrix}0&-1\\1&0\end{pmatrix}.
```



## Exercice 13

### 1



```math
p=\frac{u-\mu I}{\lambda-\mu},\qquad q=\frac{u-\lambda I}{\mu-\lambda},\qquad p+q=I.
```





```math
(u-\lambda I)p=0,\quad(u-\mu I)q=0.
```



Donc tout $x$ s'écrit $p(x)+q(x)$ dans les deux noyaux. Leur intersection est nulle car $(\lambda-\mu)x=0$. Ainsi



```math
E=\ker(u-\lambda I)\oplus\ker(u-\mu I).
```



### 2

Concaténer des bases des deux noyaux donne une base de $E$ dans laquelle la matrice est $\operatorname{diag}(\lambda I_r,\mu I_{n-r})$.

## Exercice 14

### 1



```math
\operatorname{tr}(BC)=\sum_{i,j}b_{ij}c_{ji}=\operatorname{tr}(CB),\qquad\operatorname{tr}(P^{-1}AP)=\operatorname{tr}(APP^{-1})=\operatorname{tr}A.
```



### 2



```math
E=\operatorname{im}\pi\oplus\ker\pi,\qquad\operatorname{Mat}(\pi)=\operatorname{diag}(I_r,0),\qquad\operatorname{tr}\pi=r.
```



Ainsi $M^2=M\Longrightarrow\operatorname{tr}M=\operatorname{rg}M\in\{0,\ldots,n\}$ sur $\mathbb R$ ou $\mathbb C$. Sur un corps de caractéristique positive, cette égalité se lit dans $K$.

### 3

En caractéristique différente de $2$, $s^2=I$ donne $E=\ker(s-I)\oplus\ker(s+I)$, donc



```math
\operatorname{tr}s=r-(n-r)=2r-n\in\{-n,-n+2,\ldots,n\}.
```



## Exercice 15

### 1

À un drapeau, associer une base $(e_1,\ldots,e_n)$ telle que $F_i=\operatorname{Vect}(e_1,\ldots,e_i)$, par complétions successives. Alors



```math
u(F_i)\subset F_i\ (\forall i)\iff u(e_j)\in\operatorname{Vect}(e_1,\ldots,e_j)\iff\operatorname{Mat}(u)\text{ triangulaire supérieure}.
```



### 2

Si la diagonale est nulle, $u(F_i)\subset F_{i-1}$. Par récurrence $u^k(F_i)\subset F_{\max(i-k,0)}$, d'où $u^n(E)=0$ et $A^n=0$.

## Exercice 16

Supposons $\sum_{k=0}^{n-1}a_kf^k(x)=0$ et soit $j$ le plus petit indice tel que $a_j\ne0$. Appliquer $f^{n-1-j}$ donne $a_jf^{n-1}(x)=0$, contradiction. La famille est libre de cardinal $n$, donc base.



```math
\operatorname{Mat}_{(x,f(x),\ldots,f^{n-1}(x))}(f)=\sum_{i=1}^{n-1}E_{i+1,i}.
```



## Exercice 17

### 1

Soit $u$ associé à $A$. Si $x,u(x)$ sont indépendants, choisir une forme $\ell$ telle que $\ell(x)=1$ et $\ell(u(x))=1$, puis une base commençant par $x$ et complétée dans $\ker\ell$. Le coefficient $(1,1)$ de $u$ y vaut $1$, contradiction.

Donc $u(x)=\lambda_xx$ pour tout $x\ne0$. Dans une base commençant par $x$, le coefficient $(1,1)$ vaut $\lambda_x$, donc $\lambda_x=0$. Ainsi



```math
\boxed{A=0}.
```



### 2

Les permutations des bases montrent que tous les coefficients hors diagonale de $u$ sont nuls dans toute base. Toute droite est donc stable par $u$.

Pour une base $(e_i)$, écrire $u(e_i)=\lambda_ie_i$. La stabilité de $K(e_i+e_j)$ impose $\lambda_i=\lambda_j$. Ainsi



```math
\boxed{A=\lambda I_n,\quad\lambda\in\mathbb C}.
```



La réciproque est immédiate dans les deux questions.

## Autocorrection E

### (i)

Les deux vecteurs $v_1,v_2$ vérifient $v_2-2v_1=(0,0,0,-1)$. Ils sont indépendants : rang $2$, famille libre, non génératrice. Une base complétée est $(v_1,v_2,e_2,e_3)$ : la première coordonnée sépare $v_1$, la quatrième sépare $v_2-2v_1$.

### (ii)

$v_2=-5v_1\ne0$. Rang $1$, famille ni libre ni génératrice ; $(v_1)$ est une base de son espace engendré.

### (iii)

Le déterminant de la matrice des trois colonnes vaut $1\cdot(-12)\cdot2=-24\ne0$. Rang $3$ ; la famille est une base de $\mathbb R^3$.

### (iv)

Les deux premières colonnes sont indépendantes. Pour les lignes $(1,2,4)$, le mineur d'ordre $3$ vaut $2(a-1)$.

Si $a\ne1$, rang $3$, famille libre non génératrice ; l'ajout de $e_3$ donne un déterminant $2(1-a)\ne0$.

Si $a=1$, $v_3=(v_1-v_2)/2$ ; rang $2$, famille ni libre ni génératrice, et $(v_1,v_2)$ est une base de son espace engendré.

## Autocorrection F

### 1–2



```math
P=\begin{pmatrix}1&-1&0\\1&1&1\\0&1&1\end{pmatrix},\quad\det P=1,\quad P^{-1}AP=\operatorname{diag}(2,-1,0).
```



### 3



```math
\ker f=\mathbb Re_3,\qquad\operatorname{im}f=\operatorname{Vect}(e_1,e_2).
```



## Exercice 18

Avec la base $(E_{11},E_{12},E_{21},E_{22})$ de $M_2(\mathbb C)$ :

### (i)



```math
A=\begin{pmatrix}1&1\\1&-1\\2&1\end{pmatrix},\qquad\det A_{\{1,2\},\{1,2\}}=-2\ne0,\qquad\operatorname{rg}A=2.
```



### (ii)



```math
B=\begin{pmatrix}1&1&1\\1&-1&-1\end{pmatrix},\qquad\operatorname{rg}B=2.
```



### (iii)



```math
\operatorname{Mat}(\operatorname{tr})=\begin{pmatrix}1&0&0&1\end{pmatrix},\qquad\operatorname{rg}(\operatorname{tr})=1.
```



### (iv)



```math
\operatorname{Mat}(M\mapsto M^T)=\begin{pmatrix}1&0&0&0\\0&0&1&0\\0&1&0&0\\0&0&0&1\end{pmatrix},\qquad\operatorname{rg}=4.
```



## Exercice 19

### 1

Le mineur des deux premières lignes et des colonnes $2,3$ vaut $2$, donc le rang est au moins $2$. Les mineurs des colonnes $(1,2,3)$ et $(2,3,4)$ valent respectivement $-4(a-1)$ et $-4(b-3)$.



```math
\operatorname{rg}A=2\Longrightarrow(a,b)=(1,3).
```



Pour ces valeurs, $L_3=2L_1+L_2$, donc le rang vaut $2$. Pour toute autre paire, il vaut $3$.

### 2

Pour $B$, soustraire la troisième ligne aux trois autres donne $ae_2^T$, $ae_3^T$, $ae_4^T$ ; la troisième ligne a sa première coordonnée égale à $1$. Ainsi



```math
\operatorname{rg}B=\begin{cases}1,&a=0,\\4,&a\ne0.\end{cases}
```



Pour $C$, $\det C=a+20$. Le mineur des trois premières lignes et colonnes vaut $a$, donc est non nul lorsque $a=-20$ :



```math
\operatorname{rg}C=\begin{cases}3,&a=-20,\\4,&a\ne-20.\end{cases}
```



## Exercice 20

Chaque application est linéaire ; les images des monômes donnent directement les degrés autorisés et les rangs.

### (i)



```math
\operatorname{im}D=\mathbb R_{n-1}[X],\qquad\operatorname{rg}D=n.
```



### (ii)



```math
D^r(X^j)=\begin{cases}0,&j<r,\\\dfrac{j!}{(j-r)!}X^{j-r},&j\ge r,\end{cases}\qquad\operatorname{rg}D^r=n-r+1.
```



### (iii)

Avec $Q=X^4+3X^2-2X+7\ne0$, $QP=0\Longrightarrow P=0$. De plus $\deg(QP)\le7\le8$, donc le rang vaut $4$.

### (iv)



```math
P=a+bX+cX^2+dX^3\Longrightarrow X(P'-P'(0))=2cX^2+3dX^3.
```



L'image est $\operatorname{Vect}(X^2,X^3)$ ; rang $2$.

### (v)

La matrice de $D-I$ est triangulaire de diagonale $-1$, donc le rang vaut $n+1$.

### (vi)



```math
X^j\longmapsto X^{2j},\qquad\operatorname{im}=\operatorname{Vect}(1,X^2,\ldots,X^{2n}),\qquad\operatorname{rg}=n+1.
```



## Exercice 21

### 1

$S=\ker(D^3-D)$ est un sous-espace de $C^3(\mathbb R)$. Pour $f\in S$, $h=f'$ vérifie $h''=h$, donc $h=ae^x+be^{-x}$ et $f=ae^x-be^{-x}+c$. Ainsi



```math
S=\operatorname{Vect}(\cosh,\sinh,1).
```



Si $a\cosh+b\sinh+c=0$, les valeurs de $f(0),f'(0),f''(0)$ donnent $a+c=0,b=0,a=0$. La famille est une base.

### 2–3



```math
T(\cosh)=\cosh+\sinh,\quad T(\sinh)=\cosh+\sinh,\quad T(1)=1.
```





```math
\operatorname{Mat}_{\mathcal B}(T)=\begin{pmatrix}1&1&0\\1&1&0\\0&0&1\end{pmatrix},\qquad\boxed{\operatorname{rg}T=2}.
```



## Exercice 22

Posons $r=\operatorname{rg}A$, $s=\operatorname{rg}B$. Pour tous $U,V$ inversibles,



```math
\operatorname{rg}(UA+BV)\le\min(n,r+s).
```



Choisir une base $(e_i)$ de l'espace de départ telle que $\ker A=\operatorname{Vect}(e_{r+1},\ldots,e_n)$, et une base $(h_i)$ de l'espace d'arrivée telle que $\operatorname{im}B=\operatorname{Vect}(h_{n-s+1},\ldots,h_n)$.

Définir $X(e_i)=h_i$ pour $i\le r$, $X(e_i)=0$ sinon, et $Y(e_i)=h_i$ pour $i>n-s$, $Y(e_i)=0$ sinon. Alors $\ker X=\ker A$, donc l'isomorphisme $Ax\mapsto Xx$ entre leurs images se prolonge en $U\in GL_n(\mathbb R)$ et $X=UA$.

De même $\operatorname{im}Y=\operatorname{im}B$. En choisissant des supplémentaires des noyaux, l'isomorphisme entre ces supplémentaires induit par $B$ et $Y$, complété par un isomorphisme des noyaux, donne $V\in GL_n(\mathbb R)$ tel que $Y=BV$.

Dans les bases choisies, $X+Y$ est diagonal, avec des coefficients $0,1$ ou $2$, et un coefficient non nul exactement sur $\{1,\ldots,r\}\cup\{n-s+1,\ldots,n\}$. Donc



```math
\boxed{\max_{U,V\in GL_n(\mathbb R)}\operatorname{rg}(UA+BV)=\min(n,r+s)}.
```



## Exercice 23

Effectuer simultanément $L_i\leftarrow L_i-L_{i-1}$ pour $i=n,n-1,\ldots,2$. La ligne $i\ge2$ devient $(1,\ldots,1,0,\ldots,0)$ avec $i-1$ uns ; la dernière colonne est $(n,0,\ldots,0)^T$.

Le mineur obtenu en supprimant la première ligne et la dernière colonne est triangulaire inférieur de diagonale $1$. Ainsi



```math
\det(\max(i,j))=(-1)^{n+1}n\ne0,\qquad\boxed{\operatorname{rg}=n}.
```



## Exercice 24



```math
\sin(i+j)=\sin i\cos j+\cos i\sin j\Longrightarrow\operatorname{rg}A\le2.
```





```math
\det\begin{pmatrix}\sin2&\sin3\\\sin3&\sin4\end{pmatrix}=\sin2\sin4-\sin^23=-\sin^21\ne0.
```



Donc $\boxed{\operatorname{rg}A=2}$.

## Exercice 25

Si $A$ est de rang $1$, choisir $x\ne0$ engendrant son image. Chaque colonne s'écrit $y_jx$, donc $A=xy^T$ avec $y\ne0$.

Réciproquement, si $x,y\ne0$, $Az=x(y^Tz)$ ; la forme $y^T$ est non nulle, donc $\operatorname{im}A=Kx$ et $\operatorname{rg}A=1$.

## Exercice 26

Les conditions $F\subset\ker u$ et $\operatorname{im}u\subset F$ impliquent chacune $u(F)\subset F$.

Réciproquement, si $F$ est stable et n'est pas contenu dans $\ker u$, choisir $x\in F$ tel que $u(x)\ne0$. Alors



```math
\operatorname{im}u=K u(x)\subset F.
```



## Exercice 27

### 1

Écrire $Mx_1=\lambda x_1$, $\lambda\ne0$. Alors $Kx_1\cap\ker M=0$ ; la somme des dimensions vaut $n$. Dans une base constituée de $x_1$ puis d'une base du noyau,



```math
M\sim\operatorname{diag}(\lambda,0,\ldots,0)=\lambda E_{11}.
```



### 2

Choisir $x_2$ tel que $Mx_2=x_1$. Puisque $x_1\in\ker M$ et $x_2\notin\ker M$, compléter $x_1$ en une base $(x_1,x_3,\ldots,x_n)$ du noyau. Dans $(x_1,x_2,x_3,\ldots,x_n)$, $M\sim E_{12}$.

### 3

Dans le premier cas, $M^2=\lambda M$ et $\operatorname{tr}M=\lambda$. Dans le second, $M^2=0$ et $\operatorname{tr}M=0$. Donc



```math
\boxed{M^2=(\operatorname{tr}M)M}.
```



## Exercice 28

### 1

Soient $b_k,r_k$ les vecteurs indicateurs des deux équipes. Alors $M_k=b_kr_k^T$ ; les deux équipes étant non vides, $\operatorname{rg}M_k=1$.

### 2

Chaque paire de joueurs s'affronte une fois, et aucun joueur n'affronte lui-même :



```math
M+M^T=\mathbf1\mathbf1^T-I_n.
```



### 3



```math
\dim\ker A\ge2,\qquad H=\left\{v:\sum_iv_i=0\right\},\quad\dim H=n-1.
```





```math
\dim(\ker A\cap H)\ge2+(n-1)-n=1.
```



### 4

Si $m\le n-2$, alors $\operatorname{rg}M\le\sum_k\operatorname{rg}M_k=m\le n-2$. Choisir $v\ne0$ dans $\ker M\cap H$. D'une part,



```math
v^T(M+M^T)v=2v^TMv=0.
```



D'autre part,



```math
v^T(\mathbf1\mathbf1^T-I)v=\left(\sum_iv_i\right)^2-\sum_iv_i^2=-\|v\|^2<0.
```



Contradiction ; $\boxed{m\ge n-1}$.

### 5

Pour $k=1,\ldots,n-1$, prendre $B_k=\{k\}$ et $R_k=\{k+1,\ldots,n\}$. La paire $i<j$ s'affronte exactement au match $i$.

## Exercice 29

Si $M=0$ ou $N=0$, la condition est satisfaite. Réciproquement, si $M,N\ne0$, choisir $y$ tel que $Ny\ne0$ et $z$ tel que $Mz\ne0$. Il existe $X$ tel que $X(Ny)=z$ ; alors $MXNy=Mz\ne0$.



```math
\boxed{\{(M,N):\forall X,\ MXN=0\}=\bigl(\{0\}\times M_n(\mathbb C)\bigr)\cup\bigl(M_n(\mathbb C)\times\{0\}\bigr)}.
```



## Exercice 30

Posons $r=\operatorname{rg}A<n$. Il existe $P,Q$ inversibles tels que $A=PJ_rQ$, où $J_r=\operatorname{diag}(I_r,0)$.

Soit $C$ la permutation cyclique définie par $Ce_1=e_n$ et $Ce_{i+1}=e_i$ pour $i<n$. Alors $N=C^{-1}J_r$ vérifie



```math
Ne_i=\begin{cases}e_{i+1},&i\le r,\\0,&i>r,\end{cases}\qquad N^{r+1}=0.
```



Poser $B=PCQ$. Pour tout $\lambda\in\mathbb R$,



```math
B+\lambda A=PC(I+\lambda N)Q,\qquad(I+\lambda N)^{-1}=\sum_{k=0}^r(-\lambda N)^k.
```



Ainsi $B+\lambda A$ est inversible pour tout $\lambda$.

## Exercice 31

### 1

L'application $\Phi:A\mapsto(X\mapsto\operatorname{tr}(AX))$ est linéaire. Or



```math
\operatorname{tr}(AE_{ij})=a_{ji},\qquad\Phi(A)=0\Longrightarrow A=0.
```



Les deux dimensions valent $n^2$, donc $\Phi$ est un isomorphisme.

### 2

Condition nécessaire : $n\ge2$. Pour $n=1$, l'hyperplan $\{0\}$ ne contient aucune matrice inversible.

Pour $n\ge2$, tout hyperplan s'écrit $H=\{X:\operatorname{tr}(AX)=0\}$ avec $A\ne0$. Écrire $A=PJ_rQ$, $P,Q$ inversibles. Soit $C$ une matrice de permutation cyclique sans point fixe ; elle est inversible et sa diagonale est nulle.



```math
X=Q^{-1}CP^{-1}\in GL_n(K),\qquad\operatorname{tr}(AX)=\operatorname{tr}(PJ_rCP^{-1})=\operatorname{tr}(J_rC)=0.
```



Donc $X\in H\cap GL_n(K)$.

## Exercice 32

Soient $n=\dim E$, $r=\operatorname{rg}u$ et $L_u(v)=uv$. Alors



```math
\ker L_u=\{v:\operatorname{im}v\subset\ker u\}=\mathcal L(E,\ker u),\quad\dim\ker L_u=n(n-r).
```





```math
\boxed{\operatorname{rg}L_u=n^2-n(n-r)=nr}.
```



## Exercice 33

### 1



```math
GL_n(K)\longrightarrow\{\text{bases ordonnées de }K^n\},\qquad A\longmapsto(Ae_1,\ldots,Ae_n).
```



L'inverse associe à une base la matrice de ses colonnes.

### 2

Si $|K|=q$, après $k$ vecteurs indépendants, leur espace engendré possède $q^k$ éléments. Le vecteur suivant admet $q^n-q^k$ choix :



```math
\boxed{|GL_n(K)|=\prod_{k=0}^{n-1}(q^n-q^k)}.
```



## Exercice 34

Si $f=\beta\alpha$ à travers $V$,



```math
\operatorname{rg}f\le\operatorname{rg}\alpha\le\dim V.
```



La factorisation $E\xrightarrow{f}\operatorname{im}f\hookrightarrow F$ atteint cette borne. La dimension minimale est $\boxed{\operatorname{rg}f}$.

## Exercice 35

Pour $P,Q$ inversibles, l'inégalité donne $f(PAQ)\le f(A)$. Comme $A=P^{-1}(PAQ)Q^{-1}$, elle donne aussi $f(A)\le f(PAQ)$ ; donc $f$ est constante sur chaque classe d'équivalence de matrices, c'est-à-dire sur chaque rang.

Il existe donc $h:\{0,\ldots,n\}\to\mathbb R$ telle que $f(A)=h(\operatorname{rg}A)$. Pour $r\le s$, les matrices $J_r=\operatorname{diag}(I_r,0)$ vérifient $J_rJ_s=J_r$, d'où



```math
h(r)\le\min(h(r),h(s))\Longrightarrow h(r)\le h(s).
```



Réciproquement, pour toute fonction croissante $h$,



```math
\operatorname{rg}(AB)\le\min(\operatorname{rg}A,\operatorname{rg}B)\Longrightarrow h(\operatorname{rg}(AB))\le\min(h(\operatorname{rg}A),h(\operatorname{rg}B)).
```





```math
\boxed{f(A)=h(\operatorname{rg}A),\qquad h(0)\le h(1)\le\cdots\le h(n)}.
```



## Exercice 36

### 1



```math
\mathcal A(f)=\ker(g\mapsto gf)\cap\ker(g\mapsto fg)
```



est un sous-espace vectoriel.

### 2



```math
gf=0\iff g_{|\operatorname{im}f}=0,\qquad fg=0\iff\operatorname{im}g\subset\ker f.
```



Choisir $E=\operatorname{im}f\oplus S$. Toute application $h:S\to\ker f$ se prolonge de manière unique en $g\in\mathcal A(f)$ en posant $g=0$ sur $\operatorname{im}f$. Ainsi



```math
\mathcal A(f)\simeq\mathcal L(S,\ker f),\qquad\dim S=\dim E-\operatorname{rg}f=\dim\ker f,
```





```math
\boxed{\dim\mathcal A(f)=(\dim\ker f)^2}.
```


