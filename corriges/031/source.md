# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td31-espaces-euclidiens.pdf)

## Autocorrection A

La forme est bilinéaire et symétrique. De plus,



```math
\langle P,P\rangle=\int_0^1P(t)^2\,dt\ge0.
```



Si cette intégrale est nulle, la continuité et la positivité de $P^2$ imposent $P=0$ sur $[0,1]$. Un polynôme ayant une infinité de racines est nul. La forme est donc définie positive.

## Exercice 1

Dans les trois cas, la bilinéarité et la symétrie résultent de celles des produits de formes linéaires.

### (i)



```math
\langle f,f\rangle=f(0)^2+\int_{-1}^1f'(t)^2\,dt\ge0.
```



L'égalité impose $f(0)=0$ et $f'=0$ par continuité. Donc $f$ est constante nulle.

### (ii)

La somme est finie, les dérivées d'ordre supérieur au degré étant nulles. Si $P=\sum_ka_kX^k$,



```math
\langle P,P\rangle=\sum_k(k!)^2a_k^2.
```



Elle est positive et ne s'annule que pour $P=0$.

### (iii)



```math
\langle P,P\rangle=\sum_{k=0}^n\bigl(P^{(k)}(a_k)\bigr)^2\ge0.
```



Si $P\ne0$ a degré $d\le n$ et coefficient dominant $c\ne0$, alors $P^{(d)}(a_d)=d!c\ne0$. L'égalité ne peut donc avoir lieu que pour $P=0$.

## Exercice 2

Correction : le terme doit être $2^{-n}f(a_n)g(a_n)$. Le terme imprimé $f(a_n)f(b_n)$ utilise une suite non définie et ne dépend pas de $g$.

Pour la forme corrigée,



```math
\sum_{n\ge0}2^{-n}|f(a_n)g(a_n)|\le2\|f\|_\infty\|g\|_\infty.
```



La série converge absolument ; elle définit une forme bilinéaire symétrique positive. De plus,



```math
\langle f,f\rangle=0\iff f(a_n)=0\quad(\forall n).
```



Si $D=\{a_n:n\ge0\}$ est dense dans $[0,1]$, la continuité impose $f=0$.

Sinon, la fonction continue $f(t)=d(t,\overline D)$ est non nulle et vérifie $f(a_n)=0$ pour tout $n$.



```math
\boxed{\text{Produit scalaire}\iff\overline{\{a_n:n\ge0\}}=[0,1]}.
```



## Exercice 3

Les conditions sur $w$ portent uniquement sur $[0,1]$, domaine d'intégration.

Si $w(t_0)<0$ en un point de $[0,1]$, la continuité fournit un intervalle relatif non trivial où $w<0$. Une fonction continue non nulle à support dans cet intervalle vérifie $\int f^2w<0$, impossible pour un produit scalaire. Donc $w\ge0$ sur $[0,1]$.

Si $w$ est nulle sur un intervalle non trivial, une fonction continue non nulle à support dans son intérieur vérifie $\int f^2w=0$. La forme n'est pas définie positive.

Réciproquement, supposons $w\ge0$ et son ensemble de zéros d'intérieur vide dans $[0,1]$. Pour $f\ne0$, il existe un intervalle non trivial où $f^2>0$. Cet intervalle contient un point où $w>0$ ; par continuité, $f^2w>0$ sur un sous-intervalle. Donc $\int_0^1f^2w>0$.



```math
\boxed{w_{|[0,1]}\ge0,\qquad\operatorname{Int}_{[0,1]}\{w=0\}=\varnothing}.
```



Les valeurs de $w$ sur $[-1,0[$ n'interviennent pas.

## Exercice 4

La forme est bilinéaire et symétrique. Par Cauchy–Schwarz,



```math
\int_0^1(f')^2\ge\left(\int_0^1f'\right)^2=(f(1)-f(0))^2.
```



Ainsi



```math
\langle f,f\rangle\ge(f(1)-f(0))^2+2f(1)f(0)=f(0)^2+f(1)^2\ge0.
```



Si $\langle f,f\rangle=0$, alors $f(0)=f(1)=0$ et $\int(f')^2=0$. Donc $f'=0$ puis $f=0$.

## Exercice 5

### 1



```math
\|(1-t)x+ty\|^2=(1-t)\|x\|^2+t\|y\|^2-t(1-t)\|x-y\|^2.
```



Pour $\|x\|=\|y\|=1$, $x\ne y$ et $0<t<1$, le second membre vaut $1-t(1-t)\|x-y\|^2<1$.

### 2

Les fonctions $f(x)=1$ et $g(x)=x$ sont distinctes et de norme uniforme $1$, mais



```math
\left\|\frac{f+g}{2}\right\|_\infty=1.
```



Cette norme ne peut donc pas provenir d'un produit scalaire.

## Exercice 6

Sur l'espace vectoriel réel, poser $q(x)=\|x\|^2$ et



```math
B(x,y)=\frac14\bigl(q(x+y)-q(x-y)\bigr).
```



La parité de $q$ donne $B(x,y)=B(y,x)$ et $B(-x,y)=-B(x,y)$. L'identité du parallélogramme, appliquée aux couples $(x+y,z)$ et $(x-y,z)$, donne



```math
B(x+z,y)+B(x-z,y)=2B(x,y).
```



Avec $z=x$, on obtient $B(2x,y)=2B(x,y)$. En remplaçant ensuite $(x,z)$ par $((a+b)/2,(a-b)/2)$,



```math
B(a,y)+B(b,y)=2B((a+b)/2,y)=B(a+b,y).
```



L'additivité donne $B(rx,y)=rB(x,y)$ pour $r\in\mathbb Q$. La continuité de la norme, donc de $B$, étend cette égalité à $r\in\mathbb R$. Par symétrie, $B$ est bilinéaire. Enfin,



```math
B(x,x)=\tfrac14q(2x)=\|x\|^2.
```



Donc $B$ est un produit scalaire et sa norme associée est la norme donnée.

## Exercice 7

Pour chaque choix de signes,



```math
\left\|\sum_i\epsilon_iu_i\right\|^2=\sum_i\|u_i\|^2+2\sum_{i<j}\epsilon_i\epsilon_j\langle u_i,u_j\rangle.
```



La moyenne de $\epsilon_i\epsilon_j$ sur les $2^n$ choix vaut $0$ pour $i\ne j$. Comme chaque norme est au plus $C$,



```math
\boxed{\sum_i\|u_i\|^2=2^{-n}\sum_{\epsilon\in\{\pm1\}^n}\left\|\sum_i\epsilon_iu_i\right\|^2\le C^2}.
```



## Autocorrection B

### 1



```math
\left(\sum_{k=0}^n\sqrt{\binom nk}\right)^2\le\left(\sum_{k=0}^n1\right)\left(\sum_{k=0}^n\binom nk\right)=(n+1)2^n.
```



### 2

Pour le produit scalaire canonique des matrices,



```math
|\operatorname{tr}A|=|\langle A,I_n\rangle|\le\|A\|\|I_n\|=\sqrt n\,\|A\|.
```



### 3



```math
n^2=\left(\sum_{i=1}^n\sqrt{x_i}\frac1{\sqrt{x_i}}\right)^2\le\left(\sum_i x_i\right)\left(\sum_i\frac1{x_i}\right).
```



## Exercice 8

Pour $A,B$ symétriques,



```math
\operatorname{tr}(AB)=\langle A,B\rangle,\qquad\operatorname{tr}(A^2)=\|A\|^2,\qquad\operatorname{tr}(B^2)=\|B\|^2.
```





```math
\boxed{\bigl(\operatorname{tr}(AB+BA)\bigr)^2=4\langle A,B\rangle^2\le4\operatorname{tr}(A^2)\operatorname{tr}(B^2)}.
```



## Exercice 9

### 1

Soit $Q$ une primitive polynomiale de $P^2$. Alors



```math
\frac{d}{d\theta}Q(e^{i\theta})=iP(e^{i\theta})^2e^{i\theta}.
```



En intégrant de $0$ à $\pi$,



```math
i\int_0^\pi P(e^{i\theta})^2e^{i\theta}\,d\theta=Q(-1)-Q(1)=-\int_{-1}^1P(t)^2\,dt.
```



D'où $\boxed{\int_{-1}^1P^2=-i\int_0^\pi P(e^{i\theta})^2e^{i\theta}\,d\theta}$.

### 2

Pour $P(X)=\sum_{k=0}^na_kX^k$,



```math
\sum_{k,\ell=0}^n\frac{a_ka_\ell}{k+\ell+1}=\int_0^1P^2\le\int_{-1}^1P^2\le\int_0^\pi|P(e^{i\theta})|^2\,d\theta.
```



Les coefficients étant réels,



```math
|P(e^{i\theta})|^2=\sum_ka_k^2+2\sum_{k<\ell}a_ka_\ell\cos((\ell-k)\theta).
```



Les cosinus non constants ont une intégrale nulle sur $[0,\pi]$, donc



```math
\boxed{\sum_{k,\ell=0}^n\frac{a_ka_\ell}{k+\ell+1}\le\pi\sum_{k=0}^na_k^2}.
```



## Exercice 10

### 1



```math
X^TH_nX=\sum_{i,j=0}^nx_ix_js_{i+j}=\int_0^1\left(\sum_{i=0}^nx_it^i\right)^2f(t)\,dt\ge0.
```



### 2

En prenant des vecteurs portés par les coordonnées $p,q$ dans $H_N$, $N\ge\max(p,q)$, on obtient



```math
\alpha^2s_{2p}+2\alpha\beta s_{p+q}+\beta^2s_{2q}\ge0\quad(\forall\alpha,\beta\in\mathbb R).
```



Le discriminant, ou le cas où un coefficient diagonal est nul, donne $\boxed{s_{p+q}^2\le s_{2p}s_{2q}}$.

Directement, appliquer Cauchy–Schwarz aux fonctions $t^p\sqrt{f(t)}$ et $t^q\sqrt{f(t)}$ :



```math
\left(\int_0^1t^{p+q}f(t)\,dt\right)^2\le\left(\int_0^1t^{2p}f(t)\,dt\right)\left(\int_0^1t^{2q}f(t)\,dt\right).
```



## Exercice 11

### 1



```math
M_{ij}=\langle e_i,u_j\rangle,\qquad(M^TM)_{jk}=\sum_i\langle e_i,u_j\rangle\langle e_i,u_k\rangle=\langle u_j,u_k\rangle.
```



### 2

Pour la matrice de Gram $H$ et $a\in\mathbb R^n$,



```math
a^THa=\left\|\sum_i a_iu_i\right\|^2.
```



Si les $u_i$ sont liés, une relation non triviale donne $Ha=0$. Réciproquement, si $Ha=0$, l'égalité ci-dessus impose $\sum_i a_iu_i=0$. Ainsi $\ker H=0$ si et seulement si la famille est libre.

### 3

Si la famille est liée, $G=0$. Sinon, choisir une base orthonormée de son espace engendré, de dimension $n$. Alors $H=M^TM$ et $\boxed{G=(\det M)^2>0}$.

## Exercice 12



```math
\|v_1+v_2+v_3\|^2=3+2\cdot3\left(-\frac12\right)=0.
```



Donc $v_1+v_2+v_3=0$ ; leur espace engendré est de dimension au plus $2$.

## Exercice 13

Pour $n\ge1$, dans $\mathbb R^{n+1}$, poser $H=\mathbf1^\perp$ et



```math
y_i=\sqrt{\frac{n+1}{n}}\left(e_i-\frac1{n+1}\mathbf1\right),\qquad0\le i\le n.
```



Alors $y_i\in H$, $\dim H=n$ et



```math
\langle y_i,y_j\rangle=\frac{n+1}{n}\left(\delta_{ij}-\frac1{n+1}\right)=\begin{cases}1,&i=j,\\-1/n,&i\ne j.\end{cases}
```



Transporter ces vecteurs par un isomorphisme isométrique $H\to E$ fournit les $x_i$ demandés. La dimension $n=0$ est exclue par les conditions de l'énoncé.

## Exercice 14

Supposons $\sum_i a_ix_i=0$ et $\sum_i a_i=0$, avec les $a_i$ non tous nuls. Les ensembles $I_+=\{i:a_i>0\}$ et $I_-=\{i:a_i<0\}$ sont non vides. Poser



```math
y=\sum_{i\in I_+}a_ix_i=\sum_{j\in I_-}(-a_j)x_j.
```



Alors



```math
\|y\|^2=\sum_{i\in I_+,j\in I_-}a_i(-a_j)\langle x_i,x_j\rangle<0,
```



contradiction. Les vecteurs $(x_i,1)\in E\times\mathbb R$ sont donc libres ; $\boxed{p\le\dim E+1}$.

## Exercice 15

Posons $a_i=(1+\|x_i\|^2)^{-1}$ et $S=\sum_i a_i>0$. Alors



```math
\left\|\sum_i a_ix_i\right\|^2=\sum_i a_i^2(1+\|x_i\|^2)-\left(\sum_i a_i\right)^2=S-S^2.
```



Donc $S(1-S)\ge0$ et $\boxed{S\le1}$.

L'égalité a lieu si et seulement si $\sum_i a_ix_i=0$, et équivaut à la dépendance linéaire des $x_i$. En effet, si $\sum_i c_ix_i=0$ avec $c\ne0$, en posant $C=\sum_i c_i$, le produit scalaire avec $x_j$ donne



```math
c_j(1+\|x_j\|^2)=C.
```



Si $C=0$, tous les $c_j$ seraient nuls. Donc $C\ne0$, $c_j=Ca_j$ et $C=CS$, d'où $S=1$.

## Exercice 16



```math
x\in(F+G)^\perp\iff\langle x,f+g\rangle=0\ (\forall f\in F,g\in G)\iff x\in F^\perp\cap G^\perp.
```



Appliquer cette égalité à $F^\perp,G^\perp$, puis utiliser $(H^\perp)^\perp=H$ en dimension finie :



```math
(F^\perp+G^\perp)^\perp=F\cap G\Longrightarrow\boxed{(F\cap G)^\perp=F^\perp+G^\perp}.
```



## Exercice 17

Si $F\perp G$, $\|u+v\|^2=\|u\|^2+\|v\|^2\ge\|u\|^2$.

Réciproquement, pour $u\in F,v\in G$ et tout $t\in\mathbb R$,



```math
0\le\|u+tv\|^2-\|u\|^2=2t\langle u,v\rangle+t^2\|v\|^2.
```



Un tel polynôme est positif pour tout $t$ seulement si son coefficient linéaire est nul. Donc $\langle u,v\rangle=0$.

## Exercice 18

### 1(a)

Pour $R=a+bX+cX^2$,



```math
R\perp X,X^2\iff\begin{cases}a/2+b/3+c/4=0,\\a/3+b/4+c/5=0.\end{cases}
```



La résolution donne $(a,b,c)=\lambda(3,-12,10)$ ; donc $\operatorname{Vect}(X,X^2)^\perp=\mathbb R(3-12X+10X^2)$.

### 1(b)

$A_2$ doit être orthogonal à $X,X^2$ et vérifier $\int_0^1A_2=1$. Comme $\int_0^1(3-12t+10t^2)\,dt=1/3$,



```math
\boxed{A_2=9-36X+30X^2}.
```



### 2(a)

Dans une base orthonormée $(e_0,\ldots,e_n)$ de $\mathbb R_n[X]$, poser



```math
A_n=\sum_{k=0}^ne_k(0)e_k.
```



Pour $P=\sum_kp_ke_k$, $\langle A_n,P\rangle=\sum_ke_k(0)p_k=P(0)$. Si deux polynômes conviennent, leur différence est orthogonale à tout $\mathbb R_n[X]$, donc à elle-même : ils sont égaux.

### 2(b)

Si $\deg A_n\le n-1$, prendre $P=XA_n\in\mathbb R_n[X]$. Alors



```math
0=P(0)=\int_0^1tA_n(t)^2\,dt\Longrightarrow A_n=0,
```



ce qui contredit $\langle A_n,1\rangle=1$. Ainsi $\deg A_n=n$ ; pour $n=0$, $A_0=1$.

### 3

Si un tel $A$ existait dans $\mathbb R[X]$, le même choix $P=XA$ imposerait $A=0$, tandis que $P=1$ imposerait $\int A=1$. Donc aucun polynôme ne convient.

## Exercice 19

### 1(a)



```math
QQ^T=I\Longrightarrow Q\in GL_n(\mathbb R),\quad Q^{-1}=Q^T,\quad Q^TQ=I.
```



L'identité appartient à $O_n$ ; si $Q,R\in O_n$, $(QR)(QR)^T=QRR^TQ^T=I$, et $Q^{-1}=Q^T\in O_n$. C'est donc un sous-groupe.

### 1(b)



```math
(\det Q)^2=\det(QQ^T)=1\Longrightarrow\det Q\in\{-1,1\}.
```



### 1(c)

Pour une famille de $n$ vecteurs, $Q^TQ$ est sa matrice de Gram dans une base orthonormée. Ainsi la famille est orthonormée si et seulement si $Q^TQ=I$, équivalent à $Q\in O_n$.

### 2

Pour les colonnes $c_j$ de $M$, construire récursivement une famille orthonormée $(q_j)$ telle que $c_j\in\operatorname{Vect}(q_1,\ldots,q_j)$. À l'étape $j$, retirer à $c_j$ sa projection sur les $q_i$, $i<j$. Si le résidu est non nul, le normaliser ; sinon, choisir n'importe quel vecteur unitaire orthogonal aux précédents.

Poser $Q=(q_1\ \cdots\ q_n)$ et $r_{ij}=\langle q_i,c_j\rangle$. Alors $Q$ est orthogonale, $r_{ij}=0$ pour $i>j$, et $M=QR$.

### 3



```math
|\det M|=|\det R|=\prod_{j=1}^n|r_{jj}|\le\prod_{j=1}^n\left(\sum_{i=1}^jr_{ij}^2\right)^{1/2}=\boxed{\prod_{j=1}^n\|c_j\|}.
```



## Exercice 20

### 1

Poser $T(P)=((1-X^2)P')'$. Alors



```math
T(X^k)=k(k-1)X^{k-2}-k(k+1)X^k.
```



Dans $\mathbb R_n[X]$, la matrice de $T+n(n+1)I$ est triangulaire, avec diagonale $n(n+1)-k(k+1)$, nulle exactement pour $k=n$. Chercher $P_n=\sum_{k=0}^nc_kX^k$, $c_n=1$, conduit à



```math
(k+2)(k+1)c_{k+2}+[n(n+1)-k(k+1)]c_k=0\quad(0\le k<n),
```



avec $c_{n+1}=0$. Les dénominateurs étant non nuls pour $k<n$, ces relations déterminent successivement tous les coefficients. Elles donnent une unique solution unitaire, de degré exactement $n$.

### 2

L'intégration par parties et l'annulation de $1-x^2$ aux bornes donnent



```math
\langle T(P),Q\rangle=-\int_{-1}^1(1-x^2)P'Q'=\langle P,T(Q)\rangle.
```



Ainsi



```math
[n(n+1)-m(m+1)]\langle P_n,P_m\rangle=0,
```



et les $P_n$ sont orthogonaux pour $n\ne m$.

Si $1$ était racine de multiplicité $r\ge1$ de $P_n$, écrire $P_n(x)=c(x-1)^r+O((x-1)^{r+1})$, $c\ne0$. Le premier terme de $T(P_n)$ serait $-2r^2c(x-1)^{r-1}$, tandis que $n(n+1)P_n$ s'annule à l'ordre au moins $r$ ; contradiction. Donc $P_n(1)\ne0$.

### 3

Poser $R_n=D^n((1-X^2)^n)$. Son degré est $n$, son coefficient dominant est $(-1)^n(2n)!/n!$. Pour tout $Q$ de degré inférieur à $n$, intégrer par parties $n$ fois : les termes de bord sont nuls puisque $(1-X^2)^n$ et ses dérivées d'ordre inférieur à $n$ s'annulent en $\pm1$.



```math
\int_{-1}^1R_nQ=(-1)^n\int_{-1}^1(1-x^2)^nQ^{(n)}=0.
```



$R_n$ et $P_n$ engendrent donc la même droite orthogonale à $\mathbb R_{n-1}[X]$ dans $\mathbb R_n[X]$. Enfin,



```math
R_n(1)=(-1)^n2^nn!,
```



par dérivation du produit $(1-X)^n(1+X)^n$. Par conséquent,



```math
\boxed{L_n=\frac{(-1)^n}{2^nn!}D^n((1-X^2)^n)=\frac1{2^nn!}D^n((X^2-1)^n)}.
```



## Autocorrection C

Correction : $p$ est le projecteur orthogonal sur $F$.



```math
x=p(x)+(x-p(x)),\qquad p(x)\perp x-p(x).
```





```math
d(x,F)^2=\|x-p(x)\|^2=\boxed{\langle x,x-p(x)\rangle}.
```



## Autocorrection D

### (i)

Les équations d'orthogonalité du résidu $t-a\sqrt t-b$ à $1,\sqrt t$ sont



```math
\frac12-\frac{2a}3-b=0,\qquad\frac25-\frac a2-\frac{2b}3=0.
```



Elles donnent $a=6/5$, $b=-3/10$. La famille $(1,\sqrt t)$ est libre, donc le minimiseur est unique. La valeur minimale vaut



```math
\frac13-\frac65\frac25+\frac3{10}\frac12=\boxed{\frac1{300}}.
```



### (ii)

Le domaine des paramètres est $\mathbb R^3$. Les équations normales sont



```math
\frac1{k+4}=\frac a{k+1}+\frac b{k+2}+\frac c{k+3}\qquad(k=0,1,2).
```



Elles donnent $(a,b,c)=(1/20,-3/5,3/2)$. Ainsi



```math
r(t)=t^3-\frac32t^2+\frac35t-\frac1{20}\perp\mathbb R_2[t],
```





```math
\min\int_0^1r(t)^2\,dt=\langle r,t^3\rangle=\frac17-\frac14+\frac3{25}-\frac1{80}=\boxed{\frac1{2800}}.
```



## Exercice 21

Les indices $i,j$ étant fixés, choisissons $S\in S_n(\mathbb R)$ tel que $s_{ij}=s_{ji}=m_{ij}$ (et choisissons librement les autres coefficients en respectant la symétrie). Alors $(m_{ij}-s_{ij})^2=0$. Comme cette quantité est toujours positive ou nulle,



```math
\boxed{\inf_{S\in S_n(\mathbb R)}(m_{ij}-s_{ij})^2=0}.
```



## Exercice 22

### 1

La forme est bilinéaire symétrique positive, et



```math
\langle P,P\rangle=0\iff P(a_0)=\cdots=P(a_n)=0.
```



Si les $a_k$ sont distincts, un tel polynôme de degré au plus $n$ est nul. Sinon, le produit des $(X-a)$ sur les valeurs distinctes $a$ est non nul, de degré au plus $n$, et annule toutes les évaluations.



```math
\boxed{\text{Produit scalaire}\iff a_0,\ldots,a_n\text{ deux à deux distincts}}.
```



### 2

Les polynômes de Lagrange



```math
L_i(X)=\prod_{j\ne i}\frac{X-a_j}{a_i-a_j}
```



vérifient $L_i(a_j)=\delta_{ij}$, donc $\langle L_i,L_j\rangle=\delta_{ij}$. Ils forment une base orthonormée.

### 3



```math
F=1^\perp,\qquad\|1\|^2=n+1,\qquad\boxed{d(X^n,F)=\frac{\left|\sum_{k=0}^na_k^n\right|}{\sqrt{n+1}}}.
```



Pour $n=0$, $X^0=1$ et $d(1,\{0\})=1$.

## Exercice 23

Pour $n\ge2$, poser $s=\sum_{i,j}m_{ij}$ et $K=J_n-I_n$. Alors



```math
\langle I_n,K\rangle=0,\quad\|I_n\|^2=n,\quad\|K\|^2=n(n-1),\quad\langle M,I_n\rangle=0,\quad\langle M,K\rangle=s.
```



La projection de $M$ sur $\operatorname{Vect}(I_n,J_n)$ vaut $\dfrac{s}{n(n-1)}K$. Donc



```math
\boxed{\inf_{\alpha,\beta}\|M-\alpha I_n-\beta J_n\|=\sqrt{\|M\|^2-\frac{s^2}{n(n-1)}}},
```



atteint pour $\beta=s/[n(n-1)]$, $\alpha=-\beta$. Pour $n=1$, la trace nulle impose $M=0$ et l'infimum vaut $0$.

## Exercice 24

### 1

Les termes de bord sont nuls, donc



```math
\int_0^1(t^3-t)P'(t)\,dt=\int_0^1(1-3t^2)P(t)\,dt.
```



L'égalité avec $\int P$ équivaut à $\int t^2P=0$. Ainsi $F=(X^2)^\perp$, un hyperplan de $E$.

### 2



```math
\langle Q,X^2\rangle=\frac13+\frac14+\frac15+\frac16=\frac{19}{20},\qquad\|X^2\|=\frac1{\sqrt5}.
```





```math
\boxed{d(Q,F)=\frac{19\sqrt5}{20}}.
```



## Exercice 25

### 1

La forme est bilinéaire symétrique et



```math
\langle f,f\rangle=\int_0^1(f^2+(f')^2)\ge0.
```



Si elle s'annule, la continuité impose $f=0$.

### 2



```math
F=\operatorname{Vect}(\cosh,\sinh).
```



Pour $g\in F$, intégrer par parties :



```math
\langle f,g\rangle=\int_0^1f(g-g'')+[fg']_0^1=f(1)g'(1)-f(0)g'(0).
```



Les fonctions nulles aux deux bornes sont donc dans $F^\perp$. Réciproquement, si $f\perp F$, prendre $g=\cosh$ puis $g=\sinh$ donne $f(1)\sinh1=0$, puis $f(1)\cosh1-f(0)=0$. Donc $f(0)=f(1)=0$.

### 3

La projection $p(f)$ est l'unique élément de $F$ ayant les mêmes valeurs aux bornes que $f$ :



```math
\boxed{p(f)(t)=\frac{f(0)\sinh(1-t)+f(1)\sinh t}{\sinh1}}.
```



En effet, $p(f)\in F$ et $f-p(f)\in F^\perp$.

### 4

Pour $g(t)=[\alpha\sinh(1-t)+\beta\sinh t]/\sinh1$, tout $f\in E_{\alpha,\beta}$ s'écrit $f=g+h$ avec $h\in F^\perp$. Donc $\|f\|^2=\|g\|^2+\|h\|^2\ge\|g\|^2$, égalité seulement pour $h=0$.



```math
\|g\|^2=[gg']_0^1=\beta\frac{-\alpha+\beta\cosh1}{\sinh1}-\alpha\frac{-\alpha\cosh1+\beta}{\sinh1}.
```





```math
\boxed{\inf_{f\in E_{\alpha,\beta}}\int_0^1(f^2+(f')^2)=\frac{(\alpha^2+\beta^2)\cosh1-2\alpha\beta}{\sinh1}}.
```



## Exercice 26

### 1

Pour $n\ge1$, le sous-espace $\mathbb R_{n-1}[X]$ est de dimension finie. La projection orthogonale de $X^n$ sur ce sous-espace fournit l'unique minimiseur $P=\sum_{j=0}^{n-1}a_jX^j$.

### 2(a)

Le résidu $R=X^n-P$ est orthogonal à $1,X,\ldots,X^{n-1}$, donc



```math
F(i)=\frac1{i+n+1}-\sum_{j=0}^{n-1}\frac{a_j}{i+j+1}=\int_0^1t^iR(t)\,dt=0\quad(0\le i<n).
```



### 2(b)

Le dénominateur commun est $D(X)=\prod_{j=0}^n(X+j+1)$ ; le numérateur a degré au plus $n$ et possède les racines $0,\ldots,n-1$. Donc



```math
F(X)=c\frac{\prod_{i=0}^{n-1}(X-i)}{\prod_{j=0}^n(X+j+1)}.
```



Le résidu au pôle $-n-1$ vaut $1$ dans la définition initiale. Dans cette expression il vaut $c\binom{2n}n$, donc



```math
\boxed{F(X)=\frac1{\binom{2n}n}\frac{\prod_{i=0}^{n-1}(X-i)}{\prod_{j=0}^n(X+j+1)}}.
```



### 2(c)



```math
F(n)=\frac1{\binom{2n}n}\frac{n!}{(2n+1)!/n!}=\frac1{(2n+1)\binom{2n}n^2}.
```



Comme $R\perp P$,



```math
I(P)=\langle R,R\rangle=\langle R,X^n\rangle-\langle R,P\rangle=F(n).
```





```math
\boxed{\min I=\frac1{(2n+1)\binom{2n}n^2}}.
```



## Exercice 27

Poser $g(x)=6x-2$. Alors



```math
\langle f,g\rangle=6\int_0^1xf-2\int_0^1f=4,\qquad\|g\|_2^2=\int_0^1(6x-2)^2\,dx=4.
```



Cauchy–Schwarz donne $16\le4\|f\|_2^2$, donc $\boxed{\int_0^1f^2\ge4}$. L'égalité a lieu exactement pour $f(x)=6x-2$.

## Exercice 28

Si $p$ est orthogonal, $\|x\|^2=\|p(x)\|^2+\|x-p(x)\|^2\ge\|p(x)\|^2$.

Réciproquement, pour $u\in\operatorname{im}p$, $v\in\ker p$ et $t\in\mathbb R$,



```math
\|u\|^2=\|p(u+tv)\|^2\le\|u+tv\|^2.
```



Donc $2t\langle u,v\rangle+t^2\|v\|^2\ge0$ pour tout $t$, ce qui impose $\langle u,v\rangle=0$. Ainsi $\operatorname{im}p\perp\ker p$ : $p$ est orthogonal.

## Exercice 29



```math
\|p(e_j)\|^2=\langle p(e_j),e_j\rangle,
```



car $e_j-p(e_j)\perp p(e_j)$. En sommant dans la base orthonormée,



```math
\boxed{\sum_{j=1}^n\|p(e_j)\|^2=\operatorname{tr}p=\dim F}.
```



## Exercice 30

### 1

Toute matrice de rang $1$ s'écrit $M=xy^T$ avec $x,y\ne0$. Alors



```math
\|M-I\|^2=\|x\|^2\|y\|^2-2\langle x,y\rangle+n\ge(\|x\|\|y\|-1)^2+n-1\ge n-1.
```



Pour un vecteur unitaire $u$, la matrice $uu^T$ est de rang $1$ et $\|uu^T-I\|^2=n-1$. Donc



```math
\boxed{\inf_{\operatorname{rg}M=1}\|M-I\|=\sqrt{n-1}}.
```



### 2

L'égalité impose simultanément $\langle x,y\rangle=\|x\|\|y\|$ et $\|x\|\|y\|=1$. Les vecteurs sont donc positivement colinéaires, et $xy^T=uu^T$ pour un vecteur unitaire $u$.

Les minimiseurs sont exactement les projecteurs orthogonaux sur les droites :



```math
\boxed{\{uu^T:\|u\|=1\}}.
```



## Exercice 31

### 1

Pour $f_m(x)=x^m$,



```math
\|f_m\|_\infty=1,\qquad\|f_m\|_2=(2m+1)^{-1/2}.
```



Si $V=C^0([0,1])$, l'hypothèse imposerait $1\le A/\sqrt{2m+1}$ pour tout $m$, impossible. Donc $V$ est strictement inclus.

### 2(a)

Pour une famille orthonormée $(f_1,\ldots,f_p)$,



```math
\boxed{\left\|\sum_{i=1}^pc_if_i\right\|_\infty\le A\left\|\sum_{i=1}^pc_if_i\right\|_2=A\left(\sum_{i=1}^pc_i^2\right)^{1/2}}.
```



### 2(b)

Fixer $x\in[0,1]$ et prendre $c_i=f_i(x)$. Avec $S(x)=\sum_if_i(x)^2$,



```math
S(x)\le\left\|\sum_if_i(x)f_i\right\|_\infty\le A\sqrt{S(x)}.
```



Donc $\boxed{\sum_{i=1}^pf_i(x)^2\le A^2}$ pour tout $x$.

### 3

En intégrant,



```math
p=\sum_i\|f_i\|_2^2\le A^2.
```



Toute famille libre finie de $V$ peut être orthonormalisée ; son cardinal est donc au plus $A^2$. Ainsi $\boxed{\dim V\le A^2<\infty}$.

### 4

Pour $n\ge1$, partitionner $[0,1]$ en $n$ intervalles de longueur $1/n$, en attribuant chaque point de coupure à un seul intervalle. Prendre $V$ formé des fonctions constantes, de valeur $a_k$, sur chaque intervalle. Alors $\dim V=n$ et



```math
\|f\|_\infty=\max_k|a_k|\le\left(\sum_ka_k^2\right)^{1/2}=\boxed{\sqrt n\,\|f\|_2}.
```



Pour $n=0$, prendre $V=\{0\}$.

## Exercice 32

### 1

Appliquer Gram–Schmidt à $(1,X,X^2,\ldots)$ pour $\langle P,Q\rangle=\int_{-1}^1PQ$. On obtient $\deg L_n=n$ et $\langle L_n,L_m\rangle=\delta_{nm}$.

Pour chaque $n$, $\mathbb R_n[X]\cap\mathbb R_{n-1}[X]^\perp$ est une droite ; sa normalisation laisse deux choix de signe. La famille n'est donc pas unique. Elle le devient en imposant un coefficient dominant positif à chaque $L_n$.

### 2

Soient $y_1,\ldots,y_r$ les racines intérieures de multiplicité impaire de $L_n$, et $Q=\prod_{j=1}^r(X-y_j)$. Le produit $L_nQ$ ne change pas de signe sur $[-1,1]$ et n'est pas nul ; donc $\int_{-1}^1L_nQ\ne0$.

Si $r<n$, cette intégrale serait nulle par orthogonalité à $\mathbb R_{n-1}[X]$. Ainsi $r\ge n$. Comme $\deg L_n=n$, il y a exactement $n$ racines distinctes dans $]-1,1[$, toutes simples.

### 3(a)

Pour les questions de quadrature, $n\ge1$. Soient $\ell_{i,n}$ les polynômes de Lagrange des nœuds $x_{1,n},\ldots,x_{n,n}$. Tout $f\in\mathbb R_{n-1}[X]$ vérifie



```math
f=\sum_{i=1}^nf(x_{i,n})\ell_{i,n}.
```



Ainsi les poids existent et valent nécessairement



```math
\boxed{\lambda_{i,n}=\int_{-1}^1\ell_{i,n}(t)\,dt}.
```



L'unicité résulte de l'application de la formule à chacun des $\ell_{i,n}$.

### 3(b)

Pour $\deg f\le2n-1$, effectuer la division $f=QL_n+R$ avec $\deg Q\le n-1$ et $\deg R\le n-1$. Alors



```math
\int_{-1}^1QL_n=0,\qquad f(x_{i,n})=R(x_{i,n}).
```



La formule pour $R$ donne donc celle pour $f$.

Réciproquement, si une formule à $n$ nœuds $y_1,\ldots,y_n$ est exacte jusqu'au degré $2n-1$, poser $Q=\prod_i(X-y_i)$. Pour tout $R\in\mathbb R_{n-1}[X]$,



```math
\int_{-1}^1QR=\sum_i\lambda_iQ(y_i)R(y_i)=0.
```



Ainsi $Q$ appartient à la droite $\mathbb R_n[X]\cap\mathbb R_{n-1}[X]^\perp$ ; il est proportionnel à $L_n$. Ses racines sont donc exactement les nœuds de Legendre.

### 4

Appliquer l'exactitude à $\ell_{i,n}^2$, de degré $2n-2$ :



```math
\boxed{\lambda_{i,n}=\int_{-1}^1\ell_{i,n}(t)^2\,dt>0}.
```



L'application à la constante $1$ donne $\boxed{\sum_{i=1}^n\lambda_{i,n}=2}$.

### 5

Pour $\epsilon>0$, choisir un polynôme $P$ tel que $\|f-P\|_\infty<\epsilon$. Pour $n$ assez grand, $\deg P\le2n-1$, donc $\sum_i\lambda_{i,n}P(x_{i,n})=\int P$. Par positivité des poids,



```math
\left|I_n-\int_{-1}^1f\right|\le\sum_i\lambda_{i,n}|f-P|(x_{i,n})+\int_{-1}^1|f-P|\le2\epsilon+2\epsilon.
```



Comme $\epsilon$ est arbitraire, $\boxed{I_n\longrightarrow\int_{-1}^1f}$.

## Exercice 33

Pour une matrice triangulaire supérieure dans $\mathcal B=(b_1,\ldots,b_n)$, les espaces $F_k=\operatorname{Vect}(b_1,\ldots,b_k)$ sont stables par $u$.

L'orthonormalisation de Gram–Schmidt donne une base $(e_1,\ldots,e_n)$ vérifiant $\operatorname{Vect}(e_1,\ldots,e_k)=F_k$. Donc $u(e_k)\in F_k$ et la matrice dans cette base orthonormée est encore triangulaire supérieure.

Pour une matrice triangulaire inférieure, appliquer le même raisonnement à la base renversée, puis renverser la base orthonormée obtenue.

## Exercice 34

### 1

Supposons $\sum_ka_kf_k=0$, avec les $a_k$ non tous nuls. Alors



```math
\left\|\sum_ka_ke_k\right\|=\left\|\sum_ka_k(e_k-f_k)\right\|\le\sum_k|a_k|\|e_k-f_k\|<\frac1{\sqrt n}\sum_k|a_k|\le\left(\sum_ka_k^2\right)^{1/2}.
```



Or, par orthonormalité, le membre de gauche vaut exactement $\sqrt{\sum_ka_k^2}$, contradiction. Les $f_k$ sont libres et forment donc une base.

### 2

Non. Poser



```math
f_k=e_k-\frac1n\sum_{j=1}^ne_j.
```



Alors $\|f_k-e_k\|=1/\sqrt n$, mais $\sum_{k=1}^nf_k=0$ ; la famille est liée.
