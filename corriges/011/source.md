# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td11-anneaux-corps.pdf)

Les sous-anneaux et morphismes considérés sont unitaires.

## Autocorrection A

### (i)

```math
1\in\mathbb N,\qquad-1\notin\mathbb N.
```

Non.

### (ii)

```math
1\in D,\qquad \frac a{10^m}-\frac b{10^n}=\frac{a10^n-b10^m}{10^{m+n}}\in D,\qquad\frac a{10^m}\frac b{10^n}=\frac{ab}{10^{m+n}}\in D.
```

Oui.

### (iii)

```math
I_2\notin B.
```

Non.

### (iv)

Pour $n\ge2$,

```math
E_{11},\ E_{12}+E_{21}\in S_n(\mathbb R),\qquad E_{11}(E_{12}+E_{21})=E_{12}\notin S_n(\mathbb R).
```

Non pour $n\ge2$ ; oui pour $n=1$.

### (v)

```math
I_n\in M_n(\mathbb R),\qquad A,B\in M_n(\mathbb R)\Rightarrow A-B,AB\in M_n(\mathbb R).
```

Oui.

### (vi)

```math
(1,1,\ldots)\notin B.
```

Non.

### (vii)

```math
(0,0,\ldots)\notin B.
```

Non.

### (viii)

```math
u_n\to\ell,\ v_n\to m\Rightarrow u_n-v_n\to\ell-m,\quad u_nv_n\to\ell m.
```

La suite constante $1$ appartient à $B$ : oui.

### (ix)

```math
f(-x)=f(x),\ g(-x)=g(x)\Rightarrow(f-g)(-x)=(f-g)(x),\quad(fg)(-x)=(fg)(x).
```

La fonction constante $1$ est paire : oui.

## Autocorrection B

### 1

```math
b\in B^\times\Rightarrow\exists c\in B,\ bc=cb=1_B=1_A\Rightarrow b\in A^\times.
```

### 2

```math
A=\mathbb Q,\quad B=\mathbb Z,\qquad B^\times=\{-1,1\}\ne\mathbb Z\setminus\{0\}=A^\times\cap B.
```

## Exercice 1

### 1

```math
[x(y+1)]^2=x^2(y+1)^2
```

```math
\Rightarrow xyxy+xyx+x^2y+x^2=x^2y^2+2x^2y+x^2\Rightarrow xyx=x^2y.
```

```math
[(y+1)x]^2=(y+1)^2x^2
```

```math
\Rightarrow yxyx+yx^2+xyx+x^2=y^2x^2+2yx^2+x^2\Rightarrow xyx=yx^2.
```

### 2

```math
(x+1)y(x+1)=(x+1)^2y
```

```math
\Rightarrow xyx+xy+yx+y=x^2y+2xy+y\Rightarrow\boxed{yx=xy.}
```

## Exercice 2

```math
u=(ab)^{-1},\qquad abu=uab=1.
```

```math
(bua-1)b=b(uab)-b=0\Rightarrow bua=1.
```

```math
a(bu)=1=(bu)a,\qquad(ua)b=1=b(ua).
```

```math
\boxed{a^{-1}=bu,\qquad b^{-1}=ua.}
```

## Exercice 3

### 1

```math
r^2=s^2\Rightarrow(r-s)(r+s)=0\Rightarrow s=r\text{ ou }s=-r.
```

### 2

Dans $\mathbb Z/8\mathbb Z$,

```math
\overline1^{\,2}=\overline3^{\,2}=\overline5^{\,2}=\overline7^{\,2}=\overline1.
```

## Exercice 4

Fixons $x,y$. Si $xy=-yx$, alors :

```math
x(y+1)=(y+1)x\Rightarrow xy=yx,
```

```math
x(y+1)=-(y+1)x\Rightarrow xy+x=-yx-x=xy-x\Rightarrow2x=0.
```

```math
2x=0\Rightarrow2xy=0\Rightarrow xy=-xy=yx.
```

Ainsi $xy=yx$ dans tous les cas.

## Exercice 5

### 1

```math
\overline2\ne\overline0\text{ dans }\mathbb Z/4\mathbb Z,\qquad\overline2^{\,2}=\overline0.
```

```math
E_{12}\ne0\text{ dans }M_2(\mathbb R),\qquad E_{12}^2=0.
```

### 2

```math
A\text{ intègre},\ x^n=0\Rightarrow x=0
```

par récurrence et absence de diviseurs de zéro.

```math
A=\mathbb R\times\mathbb R:\quad(x,y)^n=0\Rightarrow x=y=0,
```

```math
(1,0)(0,1)=0.
```

### 3(a)

```math
(xy)^n=0\Rightarrow(yx)^{n+1}=y(xy)^nx=0.
```

### 3(b)

```math
x=E_{11},\quad y=E_{21},\qquad xy=0,\quad yx=E_{21}\ne0\qquad(n=1).
```

### 4(a)

```math
x^p=y^q=0,\quad xy=yx\Rightarrow(xy)^p=x^py^p=0,
```

```math
(x+y)^{p+q-1}=\sum_{k=0}^{p+q-1}\binom{p+q-1}kx^ky^{p+q-1-k}=0.
```

### 4(b)

```math
x=E_{12},\quad y=E_{21},\quad x^2=y^2=0,\quad(x+y)^2=I_2,\quad(xy)^n=E_{11}\quad(n\ge1).
```

## Exercice 6

### 1

```math
x^N=0\Rightarrow\sum_{k\in\mathbb N}x^k:=\sum_{k=0}^{N-1}x^k.
```

```math
(1-x)\sum_{k=0}^{N-1}x^k=\sum_{k=0}^{N-1}x^k(1-x)=1-x^N=1.
```

### 2

```math
u=(1-xy)^{-1},\qquad v=1+yux.
```

```math
(1-yx)v=1+y(u-1-xyu)x=1,
```

```math
v(1-yx)=1+y(u-1-uxy)x=1.
```

```math
\boxed{(1-yx)^{-1}=1+y(1-xy)^{-1}x.}
```

### 3

Le calcul précédent utilise seulement

```math
(1-xy)u=u(1-xy)=1.
```

Il vaut pour tous $x,y\in A$, sans hypothèse de nilpotence.

## Exercice 7

### 1

```math
n1_A=0\Rightarrow nx=(n1_A)x=0.
```

### 2

```math
\phi:(A,+)\simeq\mathbb Q/\mathbb Z\Rightarrow\exists n\ge1,\ n\phi(1_A)=0\Rightarrow n1_A=0.
```

```math
\forall x\in A,\ nx=0\Rightarrow\forall q\in\mathbb Q/\mathbb Z,\ nq=0.
```

```math
q=\frac1{n+1}+\mathbb Z\Rightarrow nq=\frac n{n+1}+\mathbb Z\ne0,\quad\bot.
```

## Exercice 8

Le groupe $\mathbb R/2\pi\mathbb Z$ est divisible : $n(t/n+2\pi\mathbb Z)=t+2\pi\mathbb Z$.

```math
nA=A\Rightarrow\exists u\in A,\ nu=1_A.
```

```math
ny=0\Rightarrow y=(nu)y=u(ny)=0.
```

Un tel groupe additif serait sans torsion, alors que

```math
\pi+2\pi\mathbb Z\ne0,\qquad2(\pi+2\pi\mathbb Z)=0.
```

## Exercice 9

### 1

```math
\varphi(1)=1_A\Rightarrow\forall n\in\mathbb Z,\ \varphi(n)=n1_A.
```

```math
\boxed{\varphi:\mathbb Z\to A,\ n\mapsto n1_A}
```

est additive, multiplicative et unitaire ; c'est l'unique morphisme.

### 2

```math
A=\mathbb Q,\quad\varphi:A\to\mathbb Z\Rightarrow2\varphi(1/2)=1,
```

impossible dans $\mathbb Z$.

## Exercice 10

### 1

```math
\operatorname{End}(\mathbb Z)=\{\operatorname{id}\}.
```

```math
\varphi:\mathbb Q\to\mathbb Q,\quad q\ne0\Rightarrow q\varphi(p/q)=p\Rightarrow\varphi(p/q)=p/q.
```

### 2(a)

Le même calcul dans $\mathbb R$ donne $\varphi|_{\mathbb Q}=\operatorname{id}_{\mathbb Q}$.

### 2(b)

```math
t>0\Rightarrow t=s^2,\ s\ne0,\quad\varphi(s)\varphi(1/s)=1\Rightarrow\varphi(t)=\varphi(s)^2>0.
```

```math
x<y\Rightarrow\varphi(y)-\varphi(x)=\varphi(y-x)>0.
```

### 2(c)

```math
p_n,q_n\in\mathbb Q,\quad p_n\le x\le q_n,\quad p_n,q_n\to x.
```

```math
p_n=\varphi(p_n)\le\varphi(x)\le\varphi(q_n)=q_n\Rightarrow\varphi(x)=x.
```

### 3

```math
\varphi(i)^2=-1\Rightarrow\varphi(i)=\pm i,
```

```math
\varphi(a+ib)=a+b\varphi(i)\Rightarrow\boxed{\varphi=\operatorname{id}_{\mathbb C}\text{ ou }\varphi:z\mapsto\overline z.}
```

Ces deux applications sont bien des endomorphismes fixant $\mathbb R$.

## Exercice 11

### 1

```math
1\in\mathcal P,\quad\sum_ia_iX^i-\sum_ib_iX^i=\sum_i(a_i-b_i)X^i\in\mathbb Z[X],
```

```math
\left(\sum_ia_iX^i\right)\left(\sum_jb_jX^j\right)=\sum_k\left(\sum_{i+j=k}a_ib_j\right)X^k\in\mathbb Z[X].
```

L'identification des polynômes avec leurs fonctions sur $\mathbb R$ est injective : un polynôme non nul n'a qu'un nombre fini de racines.

### 2

```math
\varphi\left(\sum_ka_kX^k\right)=\sum_k(a_k1_A)\varphi(X)^k.
```

```math
\operatorname{Hom}(\mathcal P,A)\longrightarrow A,\quad\varphi\longmapsto\varphi(X)
```

est injective. Pour tout $u\in A$,

```math
\operatorname{ev}_u\left(\sum_ka_kX^k\right)=\sum_k(a_k1_A)u^k
```

est un morphisme, car les $a_k1_A$ sont centraux. Ainsi cette application est bijective, d'inverse $u\mapsto\operatorname{ev}_u$.

## Exercice 12

```math
g:\mathbb Z/2\mathbb Z\to A\Rightarrow2\cdot1_A=0.
```

```math
f:\mathbb Q\to A\Rightarrow1_A=f(2)f(1/2)=(2\cdot1_A)f(1/2)=0.
```

```math
\boxed{A=\{0\}.}
```

Réciproquement, les deux applications vers l'anneau nul sont des morphismes unitaires.

## Exercice 13

Soit $B\subset\mathbb Z^2$ un sous-anneau.

```math
(1,1)\in B\Rightarrow\forall y\in\mathbb Z,\ (y,y)\in B.
```

```math
(x,y)\in B\iff(x-y,0)\in B.
```

```math
H=\{t\in\mathbb Z:(t,0)\in B\}\le(\mathbb Z,+)\Rightarrow\exists d\in\mathbb N,\ H=d\mathbb Z.
```

```math
\boxed{B=\{(x,y):x-y\in d\mathbb Z\}=A_d.}
```

Réciproquement,

```math
x-y,\ x'-y'\in d\mathbb Z\Rightarrow(x-x')-(y-y')\in d\mathbb Z,
```

```math
xx'-yy'=x(x'-y')+y'(x-y)\in d\mathbb Z,
```

et $(1,1)\in A_d$. Pour $d=0$, $A_0$ est la diagonale.

## Exercice 14

### 1(a)

```math
(a+ib)-(c+id)=(a-c)+i(b-d),
```

```math
(a+ib)(c+id)=(ac-bd)+i(ad+bc),\qquad1\in\mathbb Z[i].
```

### 1(b)

```math
N(a+ib)=a^2+b^2\in\mathbb N,\qquad N(zw)=N(z)N(w).
```

```math
z\in A^\times\Rightarrow N(z)N(z^{-1})=1\Rightarrow N(z)=1.
```

```math
N(z)=1\Rightarrow z^{-1}=\overline z\in A.
```

```math
\boxed{A^\times=A\cap\mathbb U=\{1,-1,i,-i\}.}
```

### 1(c)

```math
\frac{a+ib}{c+id}=\frac{ac+bd}{c^2+d^2}+i\frac{bc-ad}{c^2+d^2}\in\mathbb Q(i).
```

```math
r,s\in\mathbb Q\Rightarrow r+is=\frac{m+in}{q}\quad(m,n\in\mathbb Z,\ q\ne0).
```

```math
\boxed{\operatorname{Frac}(\mathbb Z[i])=\mathbb Q(i).}
```

### 2(a)

```math
j^2=-1-j,\qquad(a+bj)(c+dj)=(ac-bd)+(ad+bc-bd)j.
```

La stabilité par différence et la présence de $1$ donnent le sous-anneau $\mathbb Z[j]$.

### 2(b)

```math
\overline j=j^2=-1-j,\qquad N(a+bj)=a^2-ab+b^2\in\mathbb N.
```

```math
z\in\mathbb Z[j]^\times\iff N(z)=1.
```

```math
4N(a+bj)=(2a-b)^2+3b^2=4\Rightarrow b\in\{-1,0,1\}.
```

```math
(a,b)\in\{(1,0),(-1,0),(0,1),(1,1),(0,-1),(-1,-1)\}.
```

```math
\boxed{\mathbb Z[j]^\times=\{\pm1,\pm j,\pm j^2\}.}
```

### 2(c)

```math
z/w=z\overline w/N(w)\in\mathbb Q+\mathbb Qj,\qquad\boxed{\operatorname{Frac}(\mathbb Z[j])=\mathbb Q(j).}
```

## Exercice 15

### 1

```math
(a+b\sqrt2)(c+d\sqrt2)=(ac+2bd)+(ad+bc)\sqrt2,
```

```math
(a+b\sqrt2)-(c+d\sqrt2)=(a-c)+(b-d)\sqrt2,\qquad1\in A.
```

### 2

```math
\varphi(\sqrt2)^2=2\Rightarrow\varphi(\sqrt2)=\pm\sqrt2,
```

```math
\varphi(a+b\sqrt2)=a\pm b\sqrt2.
```

Les deux signes donnent des endomorphismes :

```math
\boxed{\operatorname{End}(A)=\{\operatorname{id},c\},\qquad c(a+b\sqrt2)=a-b\sqrt2.}
```

### 3

```math
x+c(x)=2a\in\mathbb Z,\qquad xc(x)=a^2-2b^2\in\mathbb Z.
```

### 4

```math
N(x)=xc(x),\quad N(xy)=N(x)N(y).
```

```math
x\in A^\times\Rightarrow N(x)N(x^{-1})=1\Rightarrow N(x)=\pm1.
```

```math
N(x)=\pm1\Rightarrow x^{-1}=\pm c(x)\in A.
```

### 5

```math
N(1+\sqrt2)=-1\Rightarrow(1+\sqrt2)^n\in A^\times\quad(n\ge0).
```

Ces nombres sont strictement croissants, donc deux à deux distincts.

## Exercice 16

### 1

```math
p^2=p\Rightarrow(1-p)^2=1-p,\quad p(1-p)=0.
```

Les anneaux $pA$ et $(1-p)A$ ont pour unités respectives $p$ et $1-p$.

```math
\Phi:A\to pA\times(1-p)A,\quad x\mapsto(px,(1-p)x),\qquad\Phi^{-1}(u,v)=u+v.
```

```math
\Phi\text{ isomorphisme},\quad p\notin\{0,1\}\Rightarrow pA\ne0,\ (1-p)A\ne0.
```

Réciproquement, si $A\simeq R\times S$ avec $R,S\ne0$, l'antécédent de $(1_R,0_S)$ est un idempotent distinct de $0,1$.

### 2

```math
p^2=p\Rightarrow p(p-1)=0\Rightarrow p=0\text{ ou }p=1.
```

### 3

```math
f\in C^0(\mathbb R),\ f^2=f\Rightarrow f(\mathbb R)\subset\{0,1\}.
```

Par le théorème des valeurs intermédiaires, $f$ est constante ; $C^0(\mathbb R)$ est connexe.

```math
g(x)=\mathbf1_{x>0}\quad(x\ne0),\qquad g\in C^0(\mathbb R^*),\quad g^2=g,\quad g\ne0,1.
```

### 4

```math
p\in\mathbb Z^r,\ p^2=p\iff p\in\{0,1\}^r.
```

```math
\mathbb Z^r\simeq\mathbb Z^s\Rightarrow2^r=2^s\Rightarrow r=s.
```

## Exercice 17

### 1

```math
\chi:\mathcal P(E)\to\mathbb F_2^E,\quad A\mapsto\mathbf1_A.
```

```math
\mathbf1_{A\triangle B}=\mathbf1_A+\mathbf1_B,\quad\mathbf1_{A\cap B}=\mathbf1_A\mathbf1_B,\quad\mathbf1_E=1.
```

C'est une bijection ; les lois transportées sont celles de l'anneau produit $\mathbb F_2^E$.

```math
A\cap A=A.
```

### 2

```math
x^2=x\Rightarrow x(x-1)=0\Rightarrow x\in\{0,1\}.
```

```math
\boxed{A\simeq\mathbb F_2.}
```

### 3

```math
(1+1)^2=1+1\Rightarrow4\cdot1=2\cdot1\Rightarrow2\cdot1=0\Rightarrow2x=0.
```

```math
(x+y)^2=x+y\Rightarrow xy+yx=0\Rightarrow xy=-yx=yx.
```

### 4(a)

```math
x^2=x\Rightarrow x\preceq x.
```

```math
xy=x,\ yx=y\Rightarrow x=y.
```

```math
xy=x,\ yz=y\Rightarrow xz=(xy)z=x(yz)=xy=x.
```

### 4(b)

Pour $x\ne0$, l'ensemble fini non vide $\{y\ne0:y\preceq x\}$ possède un élément minimal $m$. Tout $0\ne z\preceq m$ vérifie $z\preceq x$, donc $z=m$. Ainsi $m\in M$.

### 4(c)

```math
(mx)m=mx\Rightarrow mx\preceq m\Rightarrow mx=0\text{ ou }mx=m.
```

### 4(d)

```math
m(x+y)=mx+my\Rightarrow\varphi(x+y)=\varphi(x)\triangle\varphi(y),
```

```math
mxy=(mx)y\Rightarrow\varphi(xy)=\varphi(x)\cap\varphi(y),\qquad\varphi(1)=M.
```

```math
x\ne0\Rightarrow\exists m\in M,\ m\preceq x\Rightarrow\varphi(x)\ne\varnothing,
```

donc $\varphi$ est injective.

```math
m,m'\in M,\ m\ne m'\Rightarrow mm'\preceq m,m'\Rightarrow mm'=0.
```

```math
S\subset M,\quad x=\sum_{m\in S}m\Rightarrow m'x=\begin{cases}m'&m'\in S,\\0&m'\notin S,\end{cases}\Rightarrow\varphi(x)=S.
```

### 5

```math
A=\{S\subset\mathbb N:S\text{ fini ou }\mathbb N\setminus S\text{ fini}\}.
```

$A$ est stable par $\triangle,\cap$ et contient $\mathbb N$ ; c'est un anneau booléien dénombrable infini.

```math
E\text{ fini}\Rightarrow\mathcal P(E)\text{ fini};\qquad E\text{ infini}\Rightarrow\mathcal P(E)\text{ non dénombrable}.
```

Ainsi $A$ n'est isomorphe à aucun $\mathcal P(E)$.

## Autocorrection C

### (i)

```math
(1,0)(0,1)=(0,0),\quad(1,0),(0,1)\ne0.
```

Non.

### (ii)

```math
3^{-1}=1/3\notin D,
```

car $3k=10^n$ est impossible. Non.

### (iii)

```math
\begin{pmatrix}1&1\\1&1\end{pmatrix}\begin{pmatrix}1&-1\\-1&1\end{pmatrix}=0.
```

Non.

### (iv)

```math
\begin{pmatrix}1&-i\\i&1\end{pmatrix}\begin{pmatrix}1&i\\-i&1\end{pmatrix}=0.
```

Non.

### (v)

```math
\begin{pmatrix}\sqrt2&2\\1&\sqrt2\end{pmatrix}\begin{pmatrix}\sqrt2&-2\\-1&\sqrt2\end{pmatrix}=0.
```

Non.

### (vi)

```math
M=\begin{pmatrix}a&2b\\b&a\end{pmatrix}\ne0,\quad a,b\in\mathbb Q\Rightarrow a^2-2b^2\ne0.
```

```math
M^{-1}=\frac1{a^2-2b^2}\begin{pmatrix}a&-2b\\-b&a\end{pmatrix}.
```

Oui ; cet anneau est isomorphe à $\mathbb Q(\sqrt2)$.

## Exercice 18

### 1

```math
\rho_d^2=d,\quad(a+b\rho_d)(c+e\rho_d)=ac+dbe+(ae+bc)\rho_d.
```

```math
a+b\rho_d\ne0\Rightarrow a^2-db^2\ne0,
```

car $d<0$ donne une somme de carrés, et $d>0$ est un entier non carré.

```math
\boxed{(a+b\rho_d)^{-1}=\frac{a-b\rho_d}{a^2-db^2}\in K_d.}
```

La stabilité par différence et $1\in K_d$ complètent la preuve.

### 2

```math
a+b\rho_d=a'+b'\rho_d,\quad b\ne b'\Rightarrow\rho_d=\frac{a'-a}{b-b'}\in\mathbb Q,
```

impossible. Donc $a=a'$ et $b=b'$.

### 3

```math
(a+b\rho_d)^2=\delta\Rightarrow a^2+db^2=\delta,\quad2ab=0.
```

```math
b=0\Rightarrow a^2=\delta,
```

impossible puisque $\delta\notin\{0,1\}$ est sans facteur carré.

```math
a=0\Rightarrow db^2=\delta.
```

Pour chaque premier $p$,

```math
v_p(\delta)-v_p(d)=2v_p(b),\qquad v_p(\delta),v_p(d)\in\{0,1\}.
```

La différence est paire, donc nulle ; $d$ et $\delta$ ont les mêmes facteurs premiers et le même signe. Ainsi $d=\delta$. Réciproquement, $\rho_d^2=d$.

### 4

```math
\phi:K_d\simeq K_\delta\Rightarrow\phi|_{\mathbb Q}=\operatorname{id},\quad\phi(\rho_d)^2=d\Rightarrow d=\delta.
```

A fortiori, $K_d\ne K_\delta$ si $d\ne\delta$.

### 5

```math
\phi(\rho_d)^2=d\Rightarrow\phi(\rho_d)=\pm\rho_d.
```

```math
\boxed{\phi_\pm(a+b\rho_d)=a\pm b\rho_d.}
```

Ces deux morphismes ont pour image $K_d$, sont involutifs et sont les deux automorphismes de $K_d$.

## Exercice 19

```math
\alpha=\sqrt[3]2,\qquad P=X^3-2.
```

### 1

$P$ n'a aucune racine rationnelle : $u^3=2v^3$ avec $\gcd(u,v)=1$ entraînerait $2\mid u$, puis $2\mid v$. Un polynôme de degré $3$ réductible sur $\mathbb Q$ aurait une racine rationnelle ; $P$ est donc irréductible.

```math
K=\mathbb Q[\alpha],\qquad\alpha^3=2
```

donne la stabilité par produit et différence. Pour $z=a+b\alpha+c\alpha^2\ne0$,

```math
z\bigl(a^2-2bc+(2c^2-ab)\alpha+(b^2-ac)\alpha^2\bigr)=N,
```

```math
N=a^3+2b^3+4c^3-6abc=\prod_{r=0}^2(a+b\alpha j^r+c\alpha^2j^{2r}),\quad j=e^{2i\pi/3}.
```

Aucun facteur n'est nul : sinon $P$ et le polynôme non nul $a+bX+cX^2$ auraient une racine commune, contrairement à l'irréductibilité de $P$. Ainsi $N\ne0$ et

```math
z^{-1}=\frac{a^2-2bc+(2c^2-ab)\alpha+(b^2-ac)\alpha^2}{N}\in K.
```

### 2

```math
\phi(\alpha)^3=2\Rightarrow\phi(\alpha)\in\{\alpha,\alpha j,\alpha j^2\}.
```

```math
\boxed{\phi_r(a+b\alpha+c\alpha^2)=a+b\alpha j^r+c\alpha^2j^{2r},\qquad r=0,1,2.}
```

L'unicité de l'écriture et la relation $(\alpha j^r)^3=2$ montrent que ces applications sont bien trois morphismes distincts.

### 3

```math
K\subset\mathbb R,\quad\alpha j,\alpha j^2\notin\mathbb R\Rightarrow\boxed{\operatorname{Aut}(K)=\{\operatorname{id}\}.}
```

## Exercice 20

### 1

```math
ab\ne0,\quad ab=a\Rightarrow b=1,\quad ab=b\Rightarrow a=1.
```

```math
\boxed{ab=1.}
```

### 2

La caractéristique est un nombre premier divisant l'ordre $4$ du groupe additif.

```math
\boxed{\operatorname{car}(\mathbb F_4)=2.}
```

### 3

```math
1+a=b,\quad1+b=a,\quad a+b=1,\quad a^2=b,\quad b^2=a.
```

```math
\begin{array}{c|cccc}+&0&1&a&b\\\hline0&0&1&a&b\\1&1&0&b&a\\a&a&b&0&1\\b&b&a&1&0\end{array}
\qquad
\begin{array}{c|cccc}\times&0&1&a&b\\\hline0&0&0&0&0\\1&0&1&a&b\\a&0&a&b&1\\b&0&b&1&a\end{array}
```

### 4

```math
\boxed{(\mathbb F_4,+)\simeq(\mathbb Z/2\mathbb Z)^2,\qquad(\mathbb F_4^\times,\times)\simeq\mathbb Z/3\mathbb Z.}
```

## Exercice 21

### 1

```math
M=\begin{pmatrix}a&b\\c&d\end{pmatrix}\Rightarrow M^2-(a+d)M+(ad-bc)I_2=0.
```

```math
\tau=\operatorname{tr}M,\quad\Delta=\det M,\qquad M^2=\tau M-\Delta I_2.
```

Les produits de deux combinaisons de $I_2,M$ sont encore des combinaisons de $I_2,M$ et commutent.

### 2

```math
M=\lambda I_2\Rightarrow\mathbb K[M]=\mathbb K I_2.
```

```math
aI+bM=(a+b\lambda)I+b(M-\lambda I)\Rightarrow\mathbb K[M]=\mathbb K[M-\lambda I].
```

### 3(a)

```math
N=P^{-1}MP,\qquad\Phi:\mathbb K[M]\to\mathbb K[N],\quad X\mapsto P^{-1}XP.
```

```math
\Phi\text{ isomorphisme},\qquad\Phi^{-1}(Y)=PYP^{-1}.
```

### 3(b)

```math
\chi_M(X)=(X-\lambda)^2\Rightarrow(M-\lambda I)^2=0,\qquad M-\lambda I\ne0.
```

### 3(c)

```math
\chi_M(X)=(X-\lambda)(X-\mu),\quad\mu=\tau-\lambda\in\mathbb K,
```

```math
(M-\lambda I)(M-\mu I)=0,
```

et les deux facteurs sont non nuls puisque $M$ n'est pas scalaire.

### 3(d)

```math
\tau^2-4\Delta<0,\quad t=\sqrt{\Delta-\tau^2/4}>0,\quad J=\frac{M-\tau I/2}{t}.
```

```math
J^2=-I,\qquad\Phi:\mathbb C\to A,\quad a+ib\mapsto aI+bJ.
```

```math
\Phi\text{ multiplicative, unitaire, bijective}\Rightarrow\boxed{A\simeq\mathbb C.}
```

## Exercice 22

Un morphisme de corps est injectif.

```math
\phi(n1_K)=n1_L\Rightarrow n1_K=0\iff n1_L=0.
```

```math
\operatorname{car}K=\operatorname{car}L.
```

## Exercice 23

```math
\phi:\mathbb Q\simeq\mathbb R\Rightarrow\phi|_{\mathbb Q}=\operatorname{id}\Rightarrow\phi(\mathbb Q)=\mathbb Q\ne\mathbb R.
```

```math
i^2=-1,\qquad x^2=-1\text{ n'a de solution ni dans }\mathbb Q\text{ ni dans }\mathbb R.
```

Les isomorphismes préservent les solutions de cette équation ; $\mathbb C$ n'est isomorphe à aucun de ces deux corps.

## Exercice 24

### 1

```math
1\le k\le p-1:\quad k!\binom pk=p(p-1)\cdots(p-k+1).
```

```math
p\nmid k!,\quad p\mid k!\binom pk\Rightarrow p\mid\binom pk.
```

### 2

```math
F(x+y)=(x+y)^p=x^p+y^p,\quad F(xy)=x^py^p,\quad F(1)=1.
```

```math
\boxed{F:x\mapsto x^p\text{ est un morphisme de corps}.}
```

## Exercice 25

Si $\operatorname{car}K\ne2$, $-1$ est d'ordre $2$ dans $K^\times$, tandis que

```math
2x=0\Rightarrow x=0
```

dans $(K,+)$ : aucun isomorphisme.

Si $\operatorname{car}K=2$ et $\phi:(K,+)\simeq K^\times$,

```math
\forall u\in K^\times,\quad u^2=1\Rightarrow(u-1)^2=0\Rightarrow u=1.
```

```math
K=\mathbb F_2,\qquad|(K,+)|=2\ne1=|K^\times|,\quad\bot.
```

