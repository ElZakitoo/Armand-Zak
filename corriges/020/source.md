# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td20-espaces-vectoriels.pdf)

## Exercice 1



```math
1\cdot(0,1)=(0,0)\ne(0,1).
```


L'axiome $1\cdot v=v$ est violé.

## Exercice 2

Dans la multiplication scalaire, le $b$ imprimé désigne $y$.


```math
\Phi:\mathbb R_+^*\times\mathbb R\to\mathbb R^2,\quad(x,y)\mapsto(\ln x,y).
```




```math
\Phi((x,y)+(x',y'))=\Phi(x,y)+\Phi(x',y'),\quad\Phi(\lambda\cdot(x,y))=\lambda\Phi(x,y).
```


$\Phi$ est bijective : les axiomes sont ceux de $\mathbb R^2$ transportés par $\Phi$.


```math
0_E=(1,0),\qquad-(x,y)=(x^{-1},-y).
```



## Exercice 3



```math
\Phi:(-1,1)^n\to\mathbb R^n,\quad\Phi(x)_i=\operatorname{artanh}(x_i).
```




```math
\boxed{(x\oplus y)_i=\frac{x_i+y_i}{1+x_iy_i},\qquad(\lambda\odot x)_i=\tanh(\lambda\operatorname{artanh}x_i).}
```


Ces opérations sont les images réciproques de l'addition et de la multiplication scalaire par la bijection $\Phi$ ; elles définissent un espace vectoriel réel.

## Exercice 4

### 1



```math
\overline k\cdot x=(\underbrace{1+\cdots+1}_{k\text{ termes}})\cdot x=kx\quad(0\le k<p).
```


La loi est nécessairement déterminée par l'addition.

### 2

Nécessité : $px=(p\cdot1_{\mathbb F_p})x=0$. Réciproquement, si $px=0$ pour tout $x$, posons $\overline k\cdot x=kx$.


```math
k\equiv\ell\pmod p\Rightarrow(k-\ell)x=0,
```


donc la définition est indépendante du représentant. Les distributivités et la compatibilité des produits résultent des identités des multiples entiers dans un groupe abélien.

## Exercice 5

### 1

Dans un espace vectoriel rationnel, l'application $m_n:x\mapsto nx$ est bijective, d'inverse $x\mapsto x/n$.


```math
\frac mn\cdot x=m\,m_n^{-1}(x).
```


Cette formule impose la loi.

### 2



```math
\boxed{\forall n\ge1,\quad m_n:A\to A\text{ est bijective}.}
```


Cette condition est nécessaire. Si elle est vérifiée, la formule précédente définit la loi : l'unicité de la division par $n$ assure l'indépendance de la représentation $m/n$ ; après multiplication par un dénominateur commun, chaque axiome se ramène aux identités des multiples entiers. Cela équivaut à la divisibilité et à l'absence de torsion de $A$.

## Autocorrection A

### 1

Toute combinaison de $(1,2,0),(2,1,0)$ a sa troisième coordonnée nulle. Réponse : non.

### 2



```math
\alpha(1,2,0)+\beta(1,1,1)=(3,3,1)\Rightarrow\beta=1,\ \alpha=2,\quad2\alpha+\beta=5\ne3.
```


Réponse : non.

### 3



```math
\cos(2x)=a\cos x+b\sin x\Rightarrow a=1\ (x=0),\quad1=-a\ (x=\pi),
```


contradiction.

### 4



```math
u_n=a+b(-1)^n\iff u_{2k}=a+b,\quad u_{2k+1}=a-b.
```


Ce sont exactement les suites $2$-périodiques, avec


```math
a=(u_0+u_1)/2,\qquad b=(u_0-u_1)/2.
```



## Autocorrection B

### 1



```math
3a_1+a_2+a_3=0,\quad3b_1+b_2+b_3=0.
```




```math
w=(1,0,0)\notin\operatorname{Vect}(a,b).
```



### 2



```math
u=-a+2b,\quad v=2a+b,\qquad a=(-u+2v)/5,\quad b=(2u+v)/5.
```


Les deux inclusions donnent l'égalité des espaces engendrés.

### 3



```math
\boxed{\alpha=3,\quad\beta=\gamma=1.}
```



### 4



```math
3x+y+z=0\Rightarrow(x,y,z)=-xa+(y+2x)b.
```


L'inclusion inverse résulte de la question 3.

## Autocorrection C



```math
\begin{aligned}
\text{(i)}&\quad\operatorname{Vect}((-2,1,0),(1,0,1));\\
\text{(ii)}&\quad\operatorname{Vect}((1,1,0),(-3,0,2));\\
\text{(iii)}&\quad\{(x,y,z):-3x+y-z=0\};\\
\text{(iv)}&\quad\{(x,y,z):x+y-2z=0\};\\
\text{(v)}&\quad\operatorname{Vect}(2,-3,1);\\
\text{(vi)}&\quad\operatorname{Vect}(2,0,1);\\
\text{(vii)}&\quad\{(x,y,z):y-2x=0,\ z+x=0\};\\
\text{(viii)}&\quad\{(x,y,z):3x-2y=0,\ 3x+2z=0\}.
\end{aligned}
```


Dans (i), (ii), (v), (vi), les écritures paramétriques donnent les inclusions réciproques ; dans (iii), (iv), les deux générateurs indépendants satisfont l'équation d'un plan.

## Exercice 6

### 1



```math
\cosh x=\frac{e^x+e^{-x}}2,\quad\sinh x=\frac{e^x-e^{-x}}2,
```




```math
e^x=\cosh x+\sinh x,\quad e^{-x}=\cosh x-\sinh x.
```



### 2



```math
\cos(2x)=\cos^2x-\sin^2x,\quad1=\cos^2x+\sin^2x.
```




```math
\cos^2x=\frac{1+\cos2x}2,\quad\sin^2x=\frac{1-\cos2x}2.
```




```math
\boxed{\operatorname{Vect}(\cos2x,\cos^2x,\sin^2x)=\operatorname{Vect}(1,\cos2x).}
```



## Exercice 7

### 1



```math
A=\begin{pmatrix}a&b\\c&d\end{pmatrix}\Rightarrow\boxed{A^2=(a+d)A-(ad-bc)I_2.}
```



### 2



```math
A=\operatorname{diag}(0,1,2).
```




```math
A^2=\lambda I+\mu A\Rightarrow\lambda=0,\ \mu=1,\quad4=2,\quad\bot.
```



## Autocorrection D

### 1



```math
\alpha(-1,1,1)+\beta(1,-1,1)+\gamma(1,1,-1)=(x,y,z).
```




```math
s=\alpha+\beta+\gamma=x+y+z,\quad\alpha=(s-x)/2,\quad\beta=(s-y)/2,\quad\gamma=(s-z)/2.
```


Tout vecteur a une unique décomposition ; c'est une base.


```math
\boxed{[(3,7,-2)]_{\mathcal B}=(5/2,1/2,5).}
```



### 2



```math
v_3=v_1+v_2,\qquad v_1=(1,-1,1),\quad v_2=(0,-1,2).
```


Les deux premiers vecteurs sont libres.


```math
\alpha v_1+\beta v_2=(\alpha,-\alpha-\beta,\alpha+2\beta),
```




```math
x+2y+z=0\Rightarrow(x,y,z)=xv_1+(-x-y)v_2.
```



### 3



```math
x=y-2z\Rightarrow(x,y,z)=y(1,1,0)+z(-2,0,1).
```


Une base est $((1,1,0),(-2,0,1))$.

### 4



```math
y=-2x,\quad z=-7x+2t.
```


Une base est $((1,-2,-7,0),(0,0,2,1))$.

## Autocorrection E

### (i)

Il suffit de montrer que le système


```math
\begin{cases}\alpha+4\beta+2\gamma=0,\\2\alpha+5\beta+\gamma=0,\\3\alpha+6\beta+\gamma=0\end{cases}
```


a pour unique solution $(0,0,0)$.

### (ii)

Il suffit de montrer que le système


```math
\begin{cases}2\alpha-\beta=3,\\\alpha=7,\\\alpha+\beta=4\end{cases}
```


n'a pas de solution.

### (iii)

Pour tout $(x,y,z)\in\mathbb R^3$, il suffit de montrer que


```math
\begin{cases}\alpha+3\beta-\gamma=x,\\\alpha+7\beta=y,\\\alpha+4\beta+\gamma=z\end{cases}
```


a une solution.

### (iv)

Il suffit de montrer que chacun des deux systèmes


```math
\begin{pmatrix}1&4&-1\\2&5&0\\3&6&1\end{pmatrix}\begin{pmatrix}\alpha\\\beta\\\gamma\end{pmatrix}=\begin{pmatrix}1\\1\\1\end{pmatrix},\qquad
\begin{pmatrix}1&4&-1\\2&5&0\\3&6&1\end{pmatrix}\begin{pmatrix}\alpha\\\beta\\\gamma\end{pmatrix}=\begin{pmatrix}2\\0\\-2\end{pmatrix}
```


a une solution.

### (v)

Il s'agit de déterminer toutes les solutions de


```math
\begin{cases}\alpha+4\beta+2\gamma+\delta=0,\\2\alpha+5\beta+\gamma+\delta=0,\\3\alpha+6\beta+\gamma+\delta=0.\end{cases}
```



## Exercice 8



```math
\sum_{i=1}^{n-1}\lambda_i(e_i+e_{i+1})=0.
```


Le coefficient de $e_1$ donne $\lambda_1=0$, puis ceux de $e_2,\ldots,e_{n-1}$ donnent successivement $\lambda_2=\cdots=\lambda_{n-1}=0$.

## Exercice 9



```math
\sum_ic_iv_i=0,\quad s=\sum_ic_i\Rightarrow\forall i,\ c_i+s\lambda_i=0.
```




```math
s\left(1+\sum_i\lambda_i\right)=0.
```


Si $\sum_i\lambda_i\ne-1$, tous les $c_i$ sont nuls. Si $\sum_i\lambda_i=-1$, les $\lambda_i$ ne sont pas tous nuls et


```math
\sum_i\lambda_iv_i=\left(1+\sum_i\lambda_i\right)u=0.
```



## Exercice 10

### 1



```math
a+bn^2+c2^n=0\quad(\forall n).
```


Division par $2^n$ puis limite : $c=0$. Alors $a+bn^2=0$ pour tout $n$, donc $a=b=0$.

### 2



```math
a\cos x+b\sin x+ce^x=0.
```


Division par $e^x$, puis $x\to+\infty$ : $c=0$. Les valeurs en $0$ et $\pi/2$ donnent $a=b=0$.

## Exercice 11

### 1



```math
\sum_{k=0}^na_k\cos^kx=0\Rightarrow Q(t)=\sum_{k=0}^na_kt^k=0\quad(t\in[-1,1]).
```


Un polynôme nul sur un intervalle est nul ; tous les $a_k$ sont nuls.

### 2



```math
T_0=1,\quad T_1=X,\quad T_{n+1}=2XT_n-T_{n-1},\quad T_n(\cos x)=\cos(nx).
```




```math
\deg T_n=n,\quad\operatorname{lc}(T_n)=2^{n-1}\ (n\ge1).
```


La famille $(T_0,\ldots,T_n)$ est une base de $\mathbb R_n[X]$, donc


```math
\operatorname{Vect}(1,\cos x,\ldots,\cos^nx)=\operatorname{Vect}(1,\cos x,\ldots,\cos(nx)).
```



### 3

Une combinaison nulle des $\cos(kx)$ donne un polynôme $\sum a_kT_k$ nul sur $[-1,1]$. Les degrés distincts des $T_k$ imposent tous les $a_k=0$.

## Exercice 12

### 1



```math
\alpha_1<\cdots<\alpha_r,\quad\sum_{j=1}^rc_je^{\alpha_jx}=0.
```


Division par $e^{\alpha_rx}$ puis limite en $+\infty$ : $c_r=0$. On recommence pour obtenir tous les coefficients nuls.

### 2



```math
\sum_{j=1}^rc_j|x-\alpha_j|=0,\quad\alpha_j\text{ distincts}.
```


Au point $\alpha_j$, la différence entre la dérivée droite et la dérivée gauche du membre de gauche vaut $2c_j$ ; celle de la fonction nulle vaut $0$. Donc $c_j=0$ pour tout $j$.

## Exercice 13



```math
e_k(n)=\mathbf1_{n=k}\quad(k,n\in\mathbb N).
```




```math
\sum_{k\in F}a_ke_k=0\Rightarrow\forall j\in F,\ a_j=0
```


par évaluation en $j$. La famille $(e_k)_{k\in\mathbb N}$ est libre.

## Exercice 14



```math
\sum_{k=0}^na_kf^k=0,\quad(a_k)\ne0\Rightarrow f(\mathbb R)\subset\{t:P(t)=0\},\quad P=\sum a_kX^k.
```


L'image continue d'un intervalle est un intervalle ; un intervalle fini est un singleton. Donc $f$ est constante.
Réciproquement, $f=c$ donne $f-c\cdot1=0$.


```math
\boxed{(f^n)_{n\ge0}\text{ liée}\iff f\text{ constante}.}
```



## Exercice 15

Pour $n\ge1$, considérons


```math
\mathcal B=\{I_n\}\cup\{I_n+E_{ij}:i\ne j\}\cup\{I_n+E_{ii}:1\le i<n\}.
```


Toutes ces matrices sont inversibles : $(I+E_{ij})^{-1}=I-E_{ij}$ pour $i\ne j$, et $I+E_{ii}$ est diagonale à diagonale non nulle.
Par différence avec $I$, leur espace engendré contient tous les $E_{ij}$ pour $i\ne j$ et tous les $E_{ii}$ pour $i<n$, puis


```math
E_{nn}=I-\sum_{i=1}^{n-1}E_{ii}.
```


La famille est génératrice de cardinal $n^2$ : c'est une base.

## Exercice 16

### 1



```math
a+b\sqrt2+c\sqrt3=0\quad(a,b,c\in\mathbb Q)\Rightarrow a^2=2b^2+3c^2+2bc\sqrt6.
```


Comme $\sqrt6\notin\mathbb Q$, $bc=0$. Puis l'irrationalité de $\sqrt2$ ou de $\sqrt3$ donne $a=b=c=0$.

### 2

Deux points rationnels $(x,y),(u,v)$ sur un même cercle de centre $(\sqrt2,\sqrt3)$ vérifient


```math
x^2+y^2-u^2-v^2-2(x-u)\sqrt2-2(y-v)\sqrt3=0.
```


La liberté précédente impose $x=u$ et $y=v$.

## Exercice 17



```math
\sum_{p\in F}q_p\ln p=0,\quad q_p\in\mathbb Q.
```


Après multiplication par un dénominateur commun,


```math
\sum_{p\in F}m_p\ln p=0\Rightarrow\prod_{m_p>0}p^{m_p}=\prod_{m_p<0}p^{-m_p}.
```


L'unicité de la factorisation première donne $m_p=0$, donc $q_p=0$.

## Exercice 18

Tout $z\in M$ s'écrit $z=\sum_j\lambda_jy_j$ avec $\lambda_j\in L$, puis $\lambda_j=\sum_i a_{ij}x_i$, les sommes étant finies.


```math
z=\sum_{i,j}a_{ij}x_iy_j.
```


Pour la liberté,


```math
\sum_{i,j}a_{ij}x_iy_j=0\Rightarrow\forall j,\ \sum_i a_{ij}x_i=0\Rightarrow\forall i,j,\ a_{ij}=0.
```



## Autocorrection F



```math
\begin{array}{c|l}
\text{cas}&\text{conclusion}\\\hline
\text{(i)}&\text{oui : }\operatorname{Vect}(1,1)\\
\text{(ii)}&\text{non : }(1,1)\text{ appartient, mais }(-1,-1)\text{ non}\\
\text{(iii)}&\text{oui : }\{0\}\\
\text{(iv)}&\text{non : }(1,1)+(1,-1)=(2,0)\text{ n'appartient pas}\\
\text{(v)}&\text{non : }(1,0)\text{ appartient, mais }(-1,0)\text{ non}\\
\text{(vi)}&\text{oui : }\operatorname{Vect}(1,-1)\\
\text{(vii)}&\text{non : }0\text{ n'appartient pas}\\
\text{(viii)}&\text{non : }0\text{ n'appartient pas}\\
\text{(ix)}&\text{oui : }\{0\}\\
\text{(x)}&\text{oui : }\mathbb R^2
\end{array}
```



## Autocorrection G



```math
\text{(i) oui : noyau de }(x,y,z)\mapsto2x+3y+4z.
```




```math
\text{(ii) non : }0\text{ n'appartient pas}.
```




```math
\text{(iii) oui : }\operatorname{Vect}(4,2,1).
```




```math
\text{(iv) oui : intersection des noyaux des deux formes linéaires}.
```




```math
\text{(v) oui : }\operatorname{Vect}(1,2,3).
```




```math
\text{(vi) non : }(1,0,1),(0,1,0)\text{ appartiennent, mais }(1,1,1)\text{ non}.
```



## Exercice 19



```math
\text{(i) oui : }\{0\};\qquad\text{(ii) oui : }\ker\left(x\mapsto\sum_ix_i\right);
```




```math
\text{(iii) non : }0\text{ exclu};\qquad\text{(iv) oui : }\ker\left(x\mapsto\sum_i2^ix_i\right).
```




```math
\text{(v) non : }e_1,e_2\text{ appartiennent, mais }e_1+e_2\text{ non}.
```




```math
\text{(vi) non : }e_1\in\mathbb Z^n,\quad e_1/2\notin\mathbb Z^n.
```



## Exercice 20

### (i)–(iii)

Non. Pour (i) et (iii), $(n)$ appartient, mais $(-n)$ n'appartient pas. Pour (ii), les suites $u_n=n$ et $v_n=-n+(-1)^n/4$ sont respectivement croissante et décroissante, mais leur somme n'est pas monotone.

### (iv)–(v)

Oui : une combinaison linéaire de suites bornées est bornée, et une combinaison linéaire de suites convergentes converge vers la même combinaison des limites.

### (vi)–(viii)

(vi) Non : la suite nulle n'est pas divergente. (vii) Oui : la limite d'une combinaison linéaire vaut $0$. (viii) Non : la suite nulle ne converge pas vers $1$.

### (ix)–(xii)

Oui dans les quatre cas. Les combinaisons linéaires conservent respectivement la constance, la constance à partir d'un rang commun, la période $12$, et une période commune égale au ppcm des deux périodes.

## Exercice 21



```math
\text{(i) non : le polynôme nul n'a pas degré }n.
```




```math
\text{(ii) oui : }\ker(P\mapsto P(0))\cap\ker(P\mapsto P(1)).
```


Pour (iii), $P=X(X-1)$ et $Q=-(X-2)(X-3)$ ont chacun deux racines réelles distinctes, mais $P+Q=4X-6$ n'en a qu'une : non.


```math
\text{(iv) oui : }P\mathbb R[X].
```


Pour (v), si $P\ne0$, le polynôme nul n'est pas un diviseur de $P$ : non. Si $P=0$, tout polynôme divise $P$ : oui, c'est $\mathbb R[X]$.

## Exercice 22

### (i)–(ii)

(i) Non : $x\mapsto x$ est croissante, son opposée ne l'est pas. (ii) Non : $x$ est croissante et $-x+\tfrac12\sin x$ est décroissante, mais leur somme n'est pas monotone.

### (iii)

Oui. Si $f=u-v$ et $g=s-t$ avec $u,v,s,t$ croissantes, alors $f+g=(u+s)-(v+t)$. Pour $\lambda\ge0$, $\lambda f=(\lambda u)-(\lambda v)$ ; pour $\lambda<0$, $\lambda f=(-\lambda)v-(-\lambda)u$.

### (iv)

Oui : c'est le noyau de la forme linéaire $f\mapsto f(0)+f(1)-f'(0)$ sur l'espace des fonctions dérivables.

### (v)



```math
\boxed{\text{Oui si et seulement si }y_0=0.}
```


Pour $y_0\ne0$, la fonction nulle est exclue ; pour $y_0=0$, il s'agit du noyau de l'évaluation en $x_0$.

### (vi)



```math
A\cos(x+\varphi)=A\cos\varphi\cos x-A\sin\varphi\sin x.
```


Tout couple réel $(a,b)$ s'écrit $(A\cos\varphi,-A\sin\varphi)$ : l'ensemble vaut $\operatorname{Vect}(\cos,\sin)$, donc oui.

### (vii)



```math
f(\mathbb R)\subset F,\ g(\mathbb R)\subset G,\quad F,G\text{ finis}\Rightarrow(\lambda f+\mu g)(\mathbb R)\subset\lambda F+\mu G,
```


ensemble fini. La fonction nulle appartient à l'ensemble : oui.

## Exercice 23

Si $E=\{0\}$, prendre $v=0$. Sinon, choisissons $v\in E\setminus\{0\}$ ; alors $v_1\ne0$.


```math
x\in E\Rightarrow y=x-\frac{x_1}{v_1}v\in E,\quad y_1=0\Rightarrow y=0.
```




```math
\boxed{E=\operatorname{Vect}(v).}
```



## Exercice 24

### 1



```math
f=\frac{|f|+f}2-\frac{|f|-f}2.
```


Les deux fonctions sont continues et positives.


```math
\boxed{\operatorname{Vect}\{f\in C^0(\mathbb R):f\ge0\}=C^0(\mathbb R).}
```



### 2



```math
P=\left(\frac{P+1}2\right)^2-\left(\frac{P-1}2\right)^2.
```




```math
\boxed{\operatorname{Vect}\{P\in\mathbb R[X]:P\ge0\}=\mathbb R[X].}
```



## Exercice 25

Si $F=E$, $\operatorname{Vect}(E\setminus F)=\{0\}$. Sinon, choisissons $u\notin F$. Pour tout $f\in F$, $u+f\notin F$, donc


```math
f=(u+f)-u\in\operatorname{Vect}(E\setminus F).
```




```math
\boxed{F\ne E\Rightarrow\operatorname{Vect}(E\setminus F)=E.}
```



## Exercice 26

Supposons $F\not\subset G$ et $G\not\subset F$. Choisissons $u\in F\setminus G$, $v\in G\setminus F$.


```math
u+v\in F\Rightarrow v\in F,\qquad u+v\in G\Rightarrow u\in G.
```


Donc $u+v\notin F\cup G$ : cette réunion n'est pas un sous-espace. Si l'un des espaces est inclus dans l'autre, leur réunion est le plus grand et est un sous-espace.

## Exercice 27

### 1



```math
w=\alpha u+\beta v\iff\begin{cases}a\alpha+b\beta=x,\\c\alpha+d\beta=y.\end{cases}
```



### 2



```math
u,v\text{ non colinéaires}\iff ad-bc\ne0.
```




```math
\alpha=\frac{dx-by}{ad-bc},\qquad\beta=\frac{ay-cx}{ad-bc}.
```


Tout $w$ est combinaison linéaire de $u,v$.

### 3



```math
\boxed{\{0\},\quad\text{les droites }\mathbb Ru\ (u\ne0),\quad\mathbb R^2.}
```


Un sous-espace non nul contenant deux vecteurs non colinéaires vaut $\mathbb R^2$ ; sinon, tous ses vecteurs sont colinéaires à un vecteur non nul fixé.

## Exercice 28

Sur $\mathbb R$ ou $\mathbb C$, les trois familles sont des bases.


```math
\text{(i)}\quad X^2+X+1=3+3(X-1)+(X-1)^2\Rightarrow\boxed{(3,3,1)}.
```


Les degrés $0,1,2$ prouvent la liberté.


```math
\text{(ii)}\quad X^2+X+1=\tfrac12(X^2+X)+\tfrac12(X^2+1)+\tfrac12(X+1)\Rightarrow\boxed{(1/2,1/2,1/2)}.
```


Le déterminant des coefficients vaut $2\ne0$.


```math
\text{(iii)}\quad X^2+X+1=\tfrac14(X-1)^2+0X^2+\tfrac34(X+1)^2\Rightarrow\boxed{(1/4,0,3/4)}.
```


Le déterminant des coefficients vaut $-4\ne0$. En caractéristique $2$, les familles (ii), (iii) ne sont pas des bases.

## Exercice 29



```math
\sum_{k=0}^nc_k(X-a)^k(X-b)^{n-k}=0.
```


Si $r$ est le plus petit indice de coefficient non nul, divisons par $(X-a)^r$ et évaluons en $a$ :


```math
c_r(a-b)^{n-r}=0,
```


contradiction. La famille est libre de cardinal $n+1=\dim\mathbb C_n[X]$ ; c'est une base.

## Exercice 30

### 1

Par récurrence sur $j$, chaque $x_j$ appartient à l'espace engendré par les $x_i$ conservés d'indice au plus $j$ : soit $j\in J$, soit $x_j$ est combinaison des précédents. La famille conservée est donc génératrice.
Une relation non triviale entre ses vecteurs, en isolant le plus grand indice de coefficient non nul, contredirait la définition de $J$. Elle est libre.

### 2



```math
x_3=2x_1+x_2,\qquad x_4=3x_1+2x_2.
```


Les vecteurs $x_1=(1,1,1)$ et $x_2=(-2,-1,0)$ sont indépendants :


```math
\boxed{\mathcal B=((1,1,1),(-2,-1,0)).}
```



### 3

La multiplication par $P\in GL_n$ conserve toutes les relations linéaires entre colonnes. Les indices des colonnes pivots de $B$ sont donc les indices d'une base extraite des colonnes de $A$.

## Exercice 31



```math
P_k=(X+1)^{k+1}-X^{k+1}=(k+1)X^k+\text{termes de degré inférieur}.
```


Sur $\mathbb R$ ou $\mathbb C$, $k+1\ne0$ : les degrés sont $0,\ldots,n$, donc la famille est une base. Cette conclusion suppose la caractéristique nulle, ou une caractéristique supérieure à $n+1$.

## Autocorrection H



```math
F=\{(s,s+t,t):s,t\in\mathbb R\}=\{(x,y,z):x-y+z=0\}.
```




```math
\lambda(1,1,1)\in F\Rightarrow\lambda=0\Rightarrow\boxed{F\cap G=\{0\}}.
```




```math
\dim F+\dim G=2+1=3\Rightarrow\boxed{F+G=\mathbb R^3}.
```



## Exercice 32



```math
x\in\mathbb R^n,\quad m=\frac1n\sum_{i=1}^nx_i\Rightarrow x=m(1,\ldots,1)+(x-m(1,\ldots,1))\in F+G.
```




```math
\lambda(1,\ldots,1)\in G\Rightarrow n\lambda=0\Rightarrow\lambda=0.
```




```math
\boxed{\mathbb R^n=F\oplus G.}
```



## Exercice 33



```math
x-y+z-t=0\iff x+z=y+t=s.
```




```math
v=\frac s2(1,1,1,1)+\left(v-\frac s2(1,1,1,1)\right),
```


et le second terme appartient à $G$. De plus,


```math
\lambda(1,1,1,1)\in G\Rightarrow2\lambda=0\Rightarrow\lambda=0.
```




```math
\boxed{E=F\oplus G.}
```



## Exercice 34



```math
P=a+bX+cX^2+dX^3,\quad P(X^2)=X^2P(X)\iff a=b=d=0.
```


Le premier espace est $F=\mathbb RX^2$. Le second est $G=\ker(P\mapsto P(2)-P(1))$.


```math
P=\frac{P(2)-P(1)}3X^2+\left(P-\frac{P(2)-P(1)}3X^2\right)\in F+G.
```




```math
cX^2\in G\Rightarrow4c=c\Rightarrow c=0.
```



## Exercice 35



```math
L_j(X)=\prod_{i\ne j}\frac{X-a_i}{a_j-a_i},\quad L_j(a_i)=\delta_{ij},\qquad F_j=\mathbb KL_j.
```




```math
P=\sum_{j=0}^nP(a_j)L_j.
```


L'évaluation en chacun des $a_i$ impose l'unicité ; ainsi $\mathbb K_n[X]=\bigoplus_jF_j$.

## Exercice 36

### 1



```math
u_n\to\ell\Rightarrow u=(\ell)_{n\ge0}+(u_n-\ell)_{n\ge0}.
```


Une suite constante qui converge vers $0$ est nulle ; la somme est directe.

### 2



```math
f(x)=\underbrace{f(0)+xf'(0)}_{\text{affine}}+\underbrace{f(x)-f(0)-xf'(0)}_{\in F}.
```


Une fonction affine dont la valeur et la dérivée en $0$ sont nulles est nulle.
Plus généralement, pour les fonctions $n$ fois dérivables au voisinage de $a$,


```math
E=\{f:f^{(k)}(a)=0\ (0\le k\le n)\}\oplus\mathbb R_n[X],
```


avec projection polynomiale $f\mapsto\sum_{k=0}^nf^{(k)}(a)(X-a)^k/k!$.

## Exercice 37

Taylor–Young donne


```math
f(x)=o(x^n)\iff f^{(k)}(0)=0\quad(0\le k\le n).
```


C'est une intersection de noyaux de formes linéaires, donc un sous-espace, et


```math
\boxed{C^\infty(\mathbb R)=\{f:f=o(x^n)\}\oplus\mathbb R_n[X].}
```



## Exercice 38

### 1

Toute combinaison d'éléments de $B\cup C$ se partage en une combinaison d'éléments de $B$ et une combinaison d'éléments de $C$ ; réciproquement, leur somme est une combinaison d'éléments de l'union.


```math
\boxed{\operatorname{Vect}(B\cup C)=\operatorname{Vect}(B)+\operatorname{Vect}(C).}
```



### 2



```math
\boxed{\operatorname{Vect}(A)\subset\operatorname{Vect}(A\cup B)\cap\operatorname{Vect}(A\cup C).}
```


L'inclusion peut être stricte : dans $\mathbb R^2$, prendre $A=\{e_1\}$ et $B=C=\{e_2\}$.

## Exercice 39

### 1



```math
A\cap B=A+B\Rightarrow A\subset A+B=A\cap B\subset B,
```


et réciproquement $B\subset A$. Si $A=B$, les deux expressions valent $A$.

### 2



```math
x=u+v,\quad u\in A\cap B,\quad v\in A\cap C\Rightarrow x\in A\cap(B+C).
```


Dans $\mathbb R^2$, $A=\mathbb Re_1$, $B=\mathbb Re_2$, $C=\mathbb R(e_1+e_2)$ donnent un membre gauche nul et un membre droit égal à $A$.

### 3



```math
B\subset A,\quad x=b+c\in A,\ b\in B,\ c\in C\Rightarrow c=x-b\in A\cap C.
```




```math
x\in(A\cap B)+(A\cap C).
```


L'autre inclusion résulte de 2.

## Exercice 40



```math
G=(F\cap G)\oplus H\Rightarrow F+G=F+(F\cap G)+H=F+H.
```




```math
H\subset G\Rightarrow F\cap H\subset(F\cap G)\cap H=\{0\}.
```




```math
\boxed{F+G=F\oplus H.}
```



## Exercice 41



```math
g\in G\subset G+H=F+H\Rightarrow g=f+h,\quad f\in F,\ h\in H.
```




```math
F\subset G\Rightarrow h=g-f\in G\cap H=F\cap H\Rightarrow g=f+h\in F.
```


Donc $G\subset F$, puis $F=G$.
Sans la troisième hypothèse,


```math
F=\mathbb Re_1,\quad G=\mathbb R(e_1+e_2),\quad H=\mathbb Re_2
```


donnent $F+H=G+H=\mathbb R^2$, $F\cap H=G\cap H=0$, mais $F\ne G$.
