# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td28-series.pdf)

## Autocorrection A

1. $n\sin(1/n)\to1$ : divergence.
2. $(n/2)^n$ ne tend pas vers zéro : divergence.
3. $(1/2)^{\sqrt n}$ converge par condensation, car $2^k2^{-2^{k/2}}$ décroît superexponentiellement.
4. $n^{-1/2}\ln(1+n^{-1/2})\sim1/n$ : divergence.
5. $1-\cos(\pi/n)\sim\pi^2/(2n^2)$ : convergence.
6. $(({-1})^n+n)/(n^2+1)=1/n+O(n^{-2})$ : divergence.
7. Si $a=0$, les termes sont nuls pour $n\geq1$ : convergence. Si $a\ne0$, $|a|^nn!\not\to0$ : divergence.
8. $ne^{-\sqrt n}$ converge par condensation : $2^k(2^k)e^{-2^{k/2}}\to0$ et la série condensée converge.
9. $\ln n/n^a$ converge exactement si $a>1$.
10. $\ln\frac{n^2+n+1}{n^2+n-1}\sim2/n^2$ : convergence.
11. $\ln(n^2+3)\sqrt{2^n+1}/4^n$ : le quotient tend vers $\sqrt2/4<1$, donc convergence.
12. $\ln n/\ln(e^n-1)\sim(\ln n)/n$ : divergence.
13. $\sqrt{\cosh(1/n)-1}\sim1/(\sqrt2n)$ : divergence.
14. $(n/(n+1))^{n^2}\leq e^{-n/2}$ dès que $n$ est assez grand : convergence.
15. $n\sin(1/n)=1-1/(6n^2)+O(n^{-4})$, donc


```math
(n\sin(1/n))^{n^\alpha}=\exp\bigl(-\tfrac16n^{\alpha-2}(1+o(1))\bigr).
```


La série converge si $\alpha>2$; elle diverge si $\alpha\leq2$, car le terme ne tend alors pas vers zéro.
16.


```math
\sqrt[3]{n^3+an}-\sqrt{n^2+3}
=\left(\frac a3-\frac32\right)\frac1n
+\left(\frac98-\frac{a^2}9\right)\frac1{n^3}+O(n^{-5}).
```


Convergence si et seulement si $a=9/2$ ; dans ce cas le terme est équivalent à $-9/(8n^3)$.
17. Il faut $a=1$ pour que le terme tende vers zéro. Alors


```math
e^{1/n}-1-b/n=(1-b)/n+1/(2n^2)+O(n^{-3}).
```


La série converge exactement pour $a=b=1$.
18. Développements limités :


```math
(n+1)^{1+1/n}=n+1+\ln n+o(1),\qquad (n-1)^{1-1/n}=n-1-\ln n+o(1).
```


La différence est $2\ln n+O(1)$ ; après division par $n^a$, la série converge exactement si $a>1$.

## 1

1. $(\ln n)^{-\ln n}=n^{-\ln\ln n}\leq n^{-2}$ dès que $\ln\ln n\geq2$ : convergence.
2. $(1-1/\sqrt n)^n\leq e^{-\sqrt n}$ : convergence par condensation.
3. Le terme est $n^{\gamma-2}+\ln n/n^2$. La série converge si et seulement si $\gamma<1$.
4. Taylor donne


```math
\sqrt n+a\sqrt{n+1}+b\sqrt{n+2}=(1+a+b)\sqrt n+\frac{a+2b}{2\sqrt n}+O(n^{-3/2}).
```


Il faut $1+a+b=0$ et $a+2b=0$, donc $(a,b)=(-2,1)$. Alors les sommes partielles sont


```math
\sum_{n=1}^N(\sqrt n-2\sqrt{n+1}+\sqrt{n+2})=1-\sqrt2-\sqrt{N+1}+\sqrt{N+2}\longrightarrow1-\sqrt2.
```


À partir de $n=0$, il faut ajouter $-2+\sqrt2$ : la somme vaut alors $-1$.
5. Si $b>1$, le terme est équivalent à $(a/b)^n2^{\sqrt n}$ : convergence si $a<b$, divergence si $a\geq b$. Si $0<b\leq1$, il est équivalent à $a^n$ : convergence si $a<1$, divergence si $a\geq1$.
6. $1-\tanh n=2/(e^{2n}+1)\leq2e^{-2n}$ : convergence.
7. Le terme vaut


```math
\frac\alpha3-\frac12+\frac{1}{n}\left(\frac\beta3-\frac{\alpha^2}9-\frac38\right)+O(n^{-2}).
```


Il est sommable si les coefficients constant et en $1/n$ s’annulent : $\alpha=3/2$, $\beta=15/8$, quel que soit $\gamma$. Sinon il ne tend pas vers zéro ou est équivalent à une constante non nulle fois $1/n$.
8. Pour $n$ assez grand, l’argument appartient à $[-1,1]$. Au voisinage de $1/\sqrt2$, $\arccos'(x)=-\sqrt2$; le terme est équivalent à $-\sqrt2 n^{-\alpha}$. La queue converge exactement si $\alpha>1$.
9. $\cos(1/n)^{n^\alpha}=\exp(-\tfrac12n^{\alpha-2}(1+o(1)))$. Convergence si $\alpha>2$; divergence sinon.
10. Les sommes par blocs de trois termes sont


```math
\sum_{j\geq0}\left(\frac a{\sqrt{3j+1}}+\frac b{\sqrt{3j+2}}+\frac c{\sqrt{3j+3}}\right).
```


Si $a+b+c\ne0$, le bloc est équivalent à $(a+b+c)/\sqrt{3j}$ et la série diverge. Si $a+b+c=0$, le bloc est $O(j^{-3/2})$; les termes isolés tendent vers zéro, donc la série converge.

## 2

1. $1/(n+\sin n)=1/n+O(n^{-2})$; la série est alternée convergente, mais non absolument.
2. $e-(1+1/n)^n=e/(2n)+O(n^{-2})$, donc


```math
\frac{(-1)^n}{n^\alpha}\left(e-(1+1/n)^n\right)
=\frac{e(-1)^n}{2n^{\alpha+1}}+O(n^{-\alpha-2}).
```


Pour $\alpha>-1$, le premier terme donne une série alternée convergente et le reste une série absolument convergente.
Convergence absolue si $\alpha>0$, conditionnelle si $-1<\alpha\leq0$ ; divergence si $\alpha\leq-1$, car le terme ne tend pas vers zéro.
3. $u_n=(-1)^nn^\alpha/(\sqrt n+(-1)^n)$. Posons $\beta=\alpha-1/2$. Pour $n=2k$, en développant $1/(\sqrt n+(-1)^n)$,


```math
u_{2k-1}+u_{2k}=-2(2k)^{\alpha-1}+O(k^{\alpha-3/2}+k^{\alpha-2}).
```


Si $\alpha<0$, cette série de blocs converge (son terme principal est $O(k^{\alpha-1})$) et $u_n\to0$; la série converge. Elle est absolument convergente ssi $\alpha<-1/2$, puisque $|u_n|\sim n^{\alpha-1/2}$; elle est conditionnelle si $-1/2\leq\alpha<0$. Si $0\leq\alpha<1/2$, le terme tend vers zéro mais les sommes de blocs sont équivalentes à $-2(2k)^{\alpha-1}$, dont la série diverge. Si $\alpha\geq1/2$, le terme ne tend pas vers zéro. La série converge donc exactement si $\alpha<0$.

4. $\sqrt{1+n^2\pi^2}=n\pi+(2n\pi)^{-1}+O(n^{-3})$, donc le terme est $(-1)^n/(2n\pi)+O(n^{-3})$ : convergence conditionnelle.

## 3

La sous-série des carrés vaut $\sum_{k\geq1}1/k^2<\infty$; hors carrés, $u_n=1/n^2$. La série converge.

## 4

Sur le bloc $e^k\leq n<e^{k+1}$, $(-1)^{\lfloor\ln n\rfloor}=(-1)^k$ et


```math
\sum_{e^k\leq n<e^{k+1}}\frac1n\longrightarrow\int_{e^k}^{e^{k+1}}\frac{dx}{x}=1.
```


Les sommes de blocs alternées ont donc des termes qui ne tendent pas vers zéro; divergence.

## 5

Posons $b_n=\sin(\ln n)/n$. Alors $b_n\to0$ et $|b_{n+1}-b_n|=O(n^{-2})$, donc $\sum(-1)^nb_n$ converge par sommation par parties. Elle n’est pas absolument convergente : sur les intervalles où $|\sin(\ln x)|\geq1/2$, la comparaison intégrale à $dx/x$ donne une contribution minorée par une constante positive à une infinité de périodes logarithmiques.

## 6

Posons $f(x)=\ln\ln x$. Le terme est $2f(n+1)-f(n)-f(n+2)=-f''(n)+O(n^{-3})$, et


```math
-f''(n)=\frac{\ln n+1}{n^2(\ln n)^2}=O\!\left(\frac1{n^2\ln n}\right).
```


La série converge.

## 7

1. Pour $n\geq2$, $H_n\sim\ln n$ et $\ln(n!)\sim n\ln n$, donc $u_n\sim1/n$ : divergence.
2. $\sin^3x/(1+x)\sim x^3$ en $0$, donc $v_n\sim\pi^4/(4n^4)$ : convergence.
3. Pour $n\geq2$, $w_n>0$ et $w_{n+1}=e^{-w_n}n^{-\alpha}$. Si $\alpha>1$, $w_{n+1}\leq n^{-\alpha}$, donc convergence. Si $0<\alpha\leq1$, $w_n\leq1$ dès $n\geq3$, d’où $w_{n+1}\geq e^{-1}n^{-\alpha}$ : divergence. Pour $\alpha=0$, les termes ne tendent pas vers zéro : s’ils tendaient vers zéro, la récurrence imposerait $w_{n+1}\to1$. Si $\alpha<0$, $w_{n+1}=n^{|\alpha|}e^{-w_n}$; une convergence vers zéro est impossible, car alors $w_{n+1}\sim n^{|\alpha|}\to\infty$. Divergence.

## 8

1. Pour $n\geq1$ et $x\geq1$, $0\leq e^{-x^n}\leq e^{-x}$ ; l’intégrale impropre converge. Pour $n=0$, elle vaut $(A-1)/e$ avant passage à la limite et diverge vers $+\infty$ : ce cas doit être exclu si une limite finie est demandée.
2. Sur $1\leq x\leq1+1/n$, $x^n\leq(1+1/n)^n\leq e$, donc $e^{-x^n}\geq e^{-e}$. Ainsi


```math
\int_1^\infty e^{-x^n}\,dx\geq e^{-e}/n,
```


et la série diverge.

## 9

Posons $A=1+\sqrt2$ et $B=1-\sqrt2$. Alors $A^n+B^n$ est entier et $A^n=(A^n+B^n)-B^n$. Par conséquent


```math
|\sin(\pi A^n)|=|\sin(\pi B^n)|\leq\pi|B|^n,
```


avec $|B|=\sqrt2-1<1$; la série converge absolument.

## 10

1. $\sum_{n=2}^N\ln(1-1/n^2)=\ln((N+1)/(2N))\to-\ln2$.
2. Les termes d’indices $2j$ et $2j+1$ s’annulent : $\ln((2j+1)/(2j))+\ln(2j/(2j+1))=0$. Somme $0$.
3. Le terme est $\ln((n+1)(n+2)/(n(n+3)))$. Le produit jusqu’à $N$ vaut $2(N+1)/(N+3)\to2$; somme $\ln2$.
4. Le terme $k=0$ vaut $1$. Les termes pairs $k=2j\geq2$ somment à $\sum_{j\geq1}16^{-j}=1/15$; les termes impairs valent $2^{-(2j+1)}$ et somment à $2/3$. Total $26/15$.

## 11

1. $1/[k(k+1)]=1/k-1/(k+1)$; somme $1$.
2. $1/(k^2-1)=\frac12(1/(k-1)-1/(k+1))$; les sommes partielles tendent vers $3/4$.
3. $1/[k(k+1)(k+2)]=\frac12(1/[k(k+1)]-1/[(k+1)(k+2)])$; somme $1/4$.
4. Pour $p\geq1$,


```math
\frac1{k(k+1)\cdots(k+p)}=\frac1{p!}\int_0^1x^{k-1}(1-x)^p\,dx.
```


Tonelli donne la somme $\frac1{p!}\int_0^1(1-x)^{p-1}dx=1/(p\,p!)$. Pour $p=0$, on retrouve la série harmonique, divergente.

## 12

La somme partielle est


```math
S_N=(1+a+b)\ln(N!)+(a+b)\ln(N+1)+b\ln(N+2)-b\ln2.
```


La convergence impose $1+a+b=0$ et $a+2b=0$, donc $a=-2,b=1$. Alors $S_N=\ln((N+2)/(2(N+1)))\to-\ln2$.

## 13



```math
\frac1{n(2n+1)}=\frac1n-\frac2{2n+1}.
```


Comme $\sum_{n=1}^N1/(2n+1)=H_{2N+1}-\tfrac12H_N-1$, les sommes partielles tendent vers $2-2\ln2$.

## 14

Le critère alterné assure la convergence. Pour tout $N$,


```math
\sum_{n=0}^N\frac{(-1)^n}{2n+1}
=\int_0^1\sum_{n=0}^N(-x^2)^n\,dx
=\int_0^1\frac{1-(-x^2)^{N+1}}{1+x^2}\,dx.
```


Le reste a une valeur absolue au plus $\int_0^1x^{2N+2}\,dx=1/(2N+3)$.
Donc la somme vaut $\int_0^1dx/(1+x^2)=\pi/4$.

## 15

Écrivons


```math
u_n=\frac1n-5\,\mathbf1_{5\mid n}\frac1n.
```


Les sommes partielles valent $H_N-H_{\lfloor N/5\rfloor}\to\ln5$. La série converge et sa somme est $\ln5$.

## 16

La fonction $\ln x/x$ décroît vers $0$ pour $x>e$ : la série alternée converge.
Posons $T_N=\sum_{n=1}^N\ln n/n$. Pour $g(x)=\ln x/x$, $|g'(x)|=O(\ln x/x^2)$ est intégrable. Ainsi les différences


```math
g(n)-\int_n^{n+1}g(t)\,dt
```


forment une série absolument convergente. Il existe donc $C$ tel que


```math
T_N=\frac12(\ln N)^2+C+o(1).
```


Avec $H_N=\ln N+\gamma+o(1)$,


```math
\sum_{n=1}^{2N}(-1)^n\frac{\ln n}{n}
=\ln2\,H_N+T_N-T_{2N}
\longrightarrow\gamma\ln2-\frac12(\ln2)^2.
```


Les sommes impaires ont la même limite.

## Autocorrection B

1.


```math
\frac1{\sqrt n}\sum_{k=n+1}^{2n}\frac1{\sqrt k}
=\frac1n\sum_{k=n+1}^{2n}\frac1{\sqrt{k/n}}
\longrightarrow\int_1^2\frac{dx}{\sqrt x}=2(\sqrt2-1).
```


L'équivalent est $2(\sqrt2-1)\sqrt n$.

2. La comparaison somme-intégrale donne


```math
\sum_{k=2}^n\frac1{k\ln k}=\ln\ln n+O(1)\sim\ln\ln n.
```



## 17

1. Si $\alpha>1$, choisir $1<\gamma<\alpha$: $n^{-\alpha}(\ln n)^{-\beta}=O(n^{-\gamma})$. Si $\alpha<1$, choisir $\alpha<\gamma<1$: $n^{-\alpha}(\ln n)^{-\beta}\geq n^{-\gamma}$ à partir d’un rang. Donc convergence exactement lorsque $\alpha>1$.
2. Pour $\alpha=1$, la comparaison série-intégrale et le changement $u=\ln x$ donnent


```math
\int_2^\infty\frac{dx}{x(\ln x)^\beta}=\int_{\ln2}^\infty u^{-\beta}du,
```


qui converge exactement si $\beta>1$.

## 18

Pour $s>1$, la décroissance de $x^{-s}$ donne


```math
\int_1^\infty x^{-s}dx\leq\zeta(s)\leq1+\int_1^\infty x^{-s}dx.
```


Ainsi $1/(s-1)\leq\zeta(s)\leq1+1/(s-1)$; en multipliant par $s-1$ et en faisant $s\downarrow1$, on obtient $(s-1)\zeta(s)\to1$.

## 19

Pour $N=10^9$, la décroissance de $x^{-2/3}$ donne


```math
\int_1^{N+1}x^{-2/3}dx<\sum_{n=1}^Nn^{-2/3}<1+\int_1^Nx^{-2/3}dx.
```


Le membre de gauche vaut $3((N+1)^{1/3}-1)>2997$ et celui de droite vaut $2998$. Donc


```math
\left\lfloor\sum_{n=1}^{10^9}\frac1{n^{2/3}}\right\rfloor=2997.
```



## 20

1. Le changement $u=\ln t$ donne


```math
\int_1^x\frac{\sin(\ln t)}t dt=1-\cos(\ln x),
```


qui n’a pas de limite.
2. Sur $[k,k+1]$, $g(t)=\sin(\ln t)/t$ vérifie $|g'(t)|\leq2/k^2$. Ainsi $|g(k)-\int_k^{k+1}g(t)dt|\leq2/k^2$.
3. Si $\sum\sin(\ln n)/n$ convergait, ses sommes partielles différeraient de l’intégrale correspondante d’une série absolument convergente par 2), donc l’intégrale aurait une limite. Contradiction.

## 21

1. Pour chaque $n$,


```math
\left|f(n)-\int_n^{n+1}f(t)dt\right|\leq\int_n^{n+1}|f'(t)|dt.
```


La série des différences converge absolument. De plus, $\int_1^\infty|f'|<\infty$ implique $f(x)\to L\in\mathbb R$.
Si la série converge, $f(n)\to0$, donc $L=0$ ; si l'intégrale converge, $L=0$ également, sinon son intégrale divergerait.
Dans chacun des deux cas, $\int_N^xf(t)\,dt\to0$ uniformément pour $N\leq x\leq N+1$. Le passage des bornes entières à une borne réelle ne change donc pas la convergence : les deux conditions sont équivalentes.
2. Posons $g(x)=\sin(\sqrt x)/x^\alpha$. Si $\alpha>1/2$, $|g'(x)|=O(x^{-\alpha-1/2})$ est intégrable, donc la différence entre $\sum g(n)$ et $\int g$ converge. Le changement $t=\sqrt x$ donne $\int_1^Xg(x)dx=2\int_1^{\sqrt X}t^{1-2\alpha}\sin t\,dt$, convergente par Dirichlet. Si $0<\alpha\leq1/2$, considérons les blocs d’entiers pour lesquels $\sqrt n$ parcourt $[2k\pi+\pi/6,2k\pi+5\pi/6]$. Ils contiennent $\asymp k$ termes, chacun $\asymp k^{-2\alpha}$ et positif; leur somme est $\asymp k^{1-2\alpha}$, donc ne tend pas vers zéro. La série diverge pour $0<\alpha\leq1/2$. Les mêmes blocs, où $|\sin(\sqrt n)|\geq1/2$, montrent que la série des valeurs absolues diverge si $\alpha\leq1$. Pour $\alpha>1$, elle converge absolument par comparaison à $\sum n^{-\alpha}$. Elle est donc conditionnellement convergente si $1/2<\alpha\leq1$.

## 22

Posons $d_n=v_n-u_n\geq0$. Les séries $\sum(w_n-u_n)$ convergent, et $0\leq d_n\leq w_n-u_n$; donc $\sum d_n$ converge. Or $\sum v_n=\sum u_n+\sum d_n$ converge.

## 23

1. Si $\sum u_n$ converge, $u_n\leq1$ dès un rang; alors $u_n^\alpha\leq u_n$ pour $\alpha>1$.
2. Pour tout $u_n\geq0$ et $0<\alpha<1$, $u_n^\alpha\geq u_n$ si $u_n\leq1$, et $u_n^\alpha\geq1$ si $u_n>1$. La divergence de $\sum u_n$ implique donc celle de $\sum u_n^\alpha$.

## 24

1. $\sqrt{a_na_{n+1}}\leq(a_n+a_{n+1})/2$; la convergence de $\sum a_n$ entraîne celle des produits géométriques.
2. Si $(a_n)$ décroît, $a_{n+1}\leq\sqrt{a_na_{n+1}}$, donc la convergence de la série des moyennes géométriques entraîne celle de $\sum a_n$. La réciproque générale est fausse : $a_{2n}=1/n$, $a_{2n+1}=1/n^3$ donne $\sqrt{a_na_{n+1}}=O(n^{-2})$, donc une série convergente des produits, alors que $\sum a_n$ diverge.

## 25

Pour $0\leq u_n\leq1$, $u_n/2\leq v_n\leq u_n$. Si $u_n>1$, alors $v_n>1/2$. Une infinité de tels indices entraîne la divergence des deux séries; sinon les comparaisons précédentes s’appliquent à la queue. Elles ont même nature.

## 26

1. Si $\ell<1$, choisir $q\in(\ell,1)$; finalement $u_{n+1}\leq qu_n$, donc convergence géométrique. Si $\ell>1$, choisir $q\in(1,\ell)$; finalement $u_{n+1}\geq qu_n$, donc $u_n\not\to0$ et la série diverge.
2. Pour $\ell=1$, $u_n=1/n^2$ donne une série convergente, tandis que $u_n=1/n$ donne une série divergente; dans les deux cas $u_{n+1}/u_n\to1$.

## 27

1. Sur $2^k\leq n<2^{k+1}$, la décroissance donne


```math
2^ka_{2^{k+1}}\leq\sum_{n=2^k}^{2^{k+1}-1}a_n\leq2^ka_{2^k}.
```


Les blocs ont donc même nature que la série condensée $\sum_k2^ka_{2^k}$.
2. En prenant $a_n=1/[n\ln n(\ln\ln n)^\alpha]$, la série condensée est équivalente, à un facteur constant près, à $\sum_k1/[k(\ln k)^\alpha]$, qui converge exactement si $\alpha>1$.
Plus généralement, pour $\ln_1=\ln$ et $\ln_{j+1}=\ln\circ\ln_j$, la série


```math
\sum_n\frac1{n\ln_1n\cdots\ln_{r-1}n\,(\ln_rn)^\alpha}
```


prise à partir d'un rang où tous les logarithmes sont positifs converge si et seulement si $\alpha>1$. Chaque condensation supprime un facteur logarithmique, jusqu'à la série de Riemann.

## 28

1. Avec $V_n=\sum_{k=0}^nv_k$, l’identité de sommation par parties est


```math
\sum_{k=0}^nu_kv_k=u_nV_n+\sum_{k=0}^{n-1}(u_k-u_{k+1})V_k.
```


2. Pour une série alternée, $v_k=(-1)^k$ a des sommes partielles bornées. En appliquant 1) à $u_k\geq0$ décroissante vers zéro, le terme de bord tend vers zéro et $\sum|u_k-u_{k+1}|<\infty$; la série converge.
3. Si $u_k$ décroît vers zéro et $V_k$ est bornée par $M$, la somme par parties sur $p\leq k\leq q$ est majorée en module par $2M u_p$. Le critère de Cauchy donne la convergence d’Abel.
4. Si $\alpha\leq0$, le module du terme ne tend pas vers zéro : divergence. Si $\theta\in2\pi\mathbb Z$, la série est $\sum n^{-\alpha}$ et converge ssi $\alpha>1$. Sinon les sommes partielles de $e^{in\theta}$ sont bornées; Abel donne la convergence pour $\alpha>0$. La convergence est absolue si $\alpha>1$, conditionnelle si $0<\alpha\leq1$.

## 29

1. Pour $P\geq0$,


```math
\sum_{p=0}^PS_p=\sum_{k=\varphi(0)}^{\varphi(P+1)-1}a_k.
```


La convergence de $\sum a_n$ entraîne donc celle de $\sum S_p$, avec


```math
\sum_{p\geq0}S_p=\sum_{n\geq\varphi(0)}a_n.
```


L'égalité imprimée avec la somme depuis $0$ suppose $\varphi(0)=0$ ; sinon il manque la somme des premiers termes.

2. Avec $\varphi(p)=2p$, $a_{2p}=1$ et $a_{2p+1}=-1$, tous les blocs sont nuls, mais les sommes partielles ordinaires oscillent entre $1$ et $0$.

3. Les sommes partielles aux extrémités des blocs convergent. À l'intérieur du bloc $p$, l'écart à l'extrémité est au plus


```math
\sum_{\varphi(p)\leq k<\varphi(p+1)}|a_k|\longrightarrow0.
```


Toutes les sommes partielles convergent ; les termes d'indice inférieur à $\varphi(0)$ ne font qu'ajouter une constante finie.

## 30

1. Par décroissance,


```math
0\leq nu_n\leq2\sum_{k=\lfloor n/2\rfloor}^{n}u_k\longrightarrow0,
```


car il y a au moins $n/2$ termes tous supérieurs à $u_n$ et la queue d’une série convergente tend vers zéro.
2. Poser $u_n=n^{-2}+n^{-1}\mathbf1_{\{n\text{ puissance de }2\}}$. La série est strictement positive et convergente, mais $2^ku_{2^k}=1+2^{-k}\to1$.
3. Les sommes partielles vérifient


```math
\sum_{n=1}^Nn(u_n-u_{n+1})=\sum_{n=1}^Nu_n-Nu_{N+1}\longrightarrow\sum_{n\geq1}u_n
```


par 1).
4. En posant $u_k=r^k$, on obtient $\sum_{k\geq1}kr^k=r/(1-r)^2$. Puis $\sum k^2r^k=\sum k(k-1)r^k+\sum kr^k=2r^2/(1-r)^3+r/(1-r)^2=r(1+r)/(1-r)^3$.

## 31

1. Pour $v_n=n^\beta a_n$,


```math
\frac{v_{n+1}}{v_n}=1+\frac{\beta-\alpha}n+o(1/n).
```


Si $\alpha>1$, choisir $1<\beta<\alpha$ : $v_n$ décroît à partir d'un rang, donc $a_n\leq Cn^{-\beta}$, d'où convergence.
Si $\alpha<1$, choisir $\alpha<\beta<1$ : $v_n$ croît à partir d'un rang, donc $a_n\geq cn^{-\beta}$, d'où divergence.
Pour $\alpha=1$, les suites $1/n$ et $1/[n(\ln n)^2]$ ont toutes deux un quotient $1-1/n+o(1/n)$, mais leurs séries sont respectivement divergente et convergente.

2. Posons $\mu=\min(2,\lambda)>1$. Alors


```math
\ln\frac{a_{n+1}}{a_n}=-\frac\alpha n+O(n^{-\mu}),\qquad
\ln\frac{(n+1)^\alpha a_{n+1}}{n^\alpha a_n}=O(n^{-\mu}).
```


La série de ces logarithmes converge, donc $n^\alpha a_n\to C>0$.
Ainsi $a_n\sim Cn^{-\alpha}$ et la série converge si et seulement si $\alpha>1$.

3. Pour $c_n=(\alpha)_n(\beta)_n/((\gamma)_n n!)$,


```math
\frac{c_{n+1}}{c_n}
=\frac{(n+\alpha)(n+\beta)}{(n+\gamma)(n+1)}
=1+\frac{\alpha+\beta-\gamma-1}n+O(n^{-2}).
```


À partir d'un rang, ce quotient est positif ; les coefficients ont donc un signe constant.
Par 2, $c_n\sim Cn^{\alpha+\beta-\gamma-1}$ avec $C\ne0$.

Pour $|x|<1$, convergence absolue par le quotient ; pour $|x|>1$, divergence.
Pour $x=1$, convergence si et seulement si $\gamma>\alpha+\beta$.
Pour $|x|=1$ avec $x\ne1$, si $\gamma>\alpha+\beta-1$, les modules $|c_n|$ décroissent finalement vers $0$ et les sommes partielles de $x^n$ sont bornées : Abel donne la convergence.
Si $\gamma\leq\alpha+\beta-1$, le terme ne tend pas vers $0$.
Sur tout le cercle $|x|=1$, la convergence absolue équivaut à $\gamma>\alpha+\beta$.

## 32

Si $\sum a_n<\infty$, choisissons $N_j$ croissants tels que $\sum_{n\geq N_j}a_n\leq2^{-j}/j^2$, puis posons $b_n=j$ sur $[N_j,N_{j+1})$. Alors $b_n\to\infty$ et $\sum a_nb_n\leq\sum_j2^{-j}/j<\infty$ (adapter le début par une constante finie). Si $\sum a_n=+\infty$, découpons en blocs consécutifs dont la somme est au moins $1$; sur le bloc $j$, posons $b_n=1/j$. Alors $b_n\to0$ et chaque bloc contribue au moins $1/j$, d’où $\sum a_nb_n=+\infty$.

## 33

1. Choisir des indices $n_j$ croissants tels que $\eta_{n_j}\leq2^{-j}$, poser $a_{n_j}=\eta_{n_j}$ et $a_n=0$ ailleurs. Alors $\sum a_n<\infty$, mais $a_{n_j}/\eta_{n_j}=1$, donc $a_n\ne o(\eta_n)$.
2. Pour $a_n$ décroissante positive, $\frac n2a_n\leq\sum_{k=\lfloor n/2\rfloor}^na_k$, dont la queue tend vers zéro. Donc $na_n\to0$.

## 34

Si $f(x)=cx$ au voisinage de $0$, toute série convergente $\sum a_n$ vérifie $a_n\to0$; à partir d’un rang $f(a_n)=ca_n$, donc $\sum f(a_n)$ converge.

Réciproquement, $f(0)=0$ en appliquant la propriété à la série nulle. Pour toute suite $x_j\to0$, la série $x_1,-x_1,x_2,-x_2,\ldots$ converge; sa série image converge, donc $f(x_j)\to0$. Ainsi $f$ est continue en $0$.

Il existe $\delta>0$ tel que $f(-x)=-f(x)$ pour $|x|<\delta$. Sinon, on choisit $x_j\to0$ avec $c_j=f(x_j)+f(-x_j)\ne0$; une sous-suite a des $c_j$ de même signe. Répéter le bloc $(x_j,-x_j)$ un nombre fini $m_j$ de fois, avec $m_j|c_j|\geq1$, donne une série convergente (termes $\to0$, chaque bloc d’entrée somme nulle) dont les sommes image par blocs ne sont pas de Cauchy, contradiction.

De même, il existe $\varepsilon>0$ tel que $f(x)+f(y)-f(x+y)=0$ si $|x|,|y|,|x+y|<\varepsilon$. Sinon, pour des couples $(x_j,y_j)\to(0,0)$ avec défaut non nul, les blocs $(x_j,y_j,-x_j-y_j)$ ont somme nulle et termes tendant vers zéro; après la propriété d’imparité locale, leurs sommes images sont les défauts. En répétant chaque bloc un nombre fini de fois pour que sa contribution image ait module au moins $1$ et en extrayant des défauts de même signe, on contredit la convergence de la série image.

L’additivité locale et la continuité en $0$ imposent $f(x)=cx$ sur un voisinage de $0$: pour un $h$ fixé assez petit, l’additivité donne $f(qh)=qf(h)$ pour les rationnels $q$ tels que $qh$ reste dans ce voisinage; l'additivité locale donne la continuité en tout point de cet intervalle via $f(t+h)-f(t)=f(h)\to0$. L'identité s'étend donc à tout réel de l'intervalle.

## 35

1. Par concavité de $\ln$,


```math
u_n=\int_n^{n+1}\ln x\,dx-\frac{\ln n+\ln(n+1)}2
=\left(n+\frac12\right)\ln(1+1/n)-1
\sim\frac1{12n^2}.
```



2. Posons $D_n=\ln(n!)-(n+\frac12)\ln n+n$. Alors $D_{n+1}-D_n=-u_n$.
Comme $\sum u_n$ converge, $D_n\to C$ et


```math
D_n-C=\sum_{k=n}^\infty u_k\sim\frac1{12n}.
```


Donc $n!\sim e^C\sqrt n(n/e)^n$ et


```math
\binom{2n}n\sim e^{-C}\frac{\sqrt2}{\sqrt n}4^n.
```


La formule de Wallis donne $\binom{2n}n\sim4^n/\sqrt{\pi n}$ ; ainsi $e^C=\sqrt{2\pi}$.
Finalement,


```math
\ln(n!)=n\ln n-n+\frac12\ln n+\frac12\ln(2\pi)+\frac1{12n}+o(1/n),
```




```math
n!=\sqrt{2\pi n}\left(\frac ne\right)^n
\left(1+\frac1{12n}+o(1/n)\right).
```



## 36

1. Si $u_k/v_k\to1$ et les deux séries convergent, pour tout $\varepsilon>0$, dès $k\geq N$, $(1-\varepsilon)v_k\leq u_k\leq(1+\varepsilon)v_k$. En sommant sur $k>n\geq N$, les queues vérifient les mêmes encadrements; leur quotient tend vers $1$.
2. $k^{-\alpha}\sim\int_k^{k+1}x^{-\alpha}dx$; donc $\sum_{k=n}^\infty k^{-\alpha}\sim\int_n^\infty x^{-\alpha}dx=n^{1-\alpha}/(\alpha-1)$. Le même équivalent découle directement de la comparaison intégrale.
3. Posons $C_n=H_n-\ln n-1/(2n)+1/(12n^2)$. Un développement de $\ln(1+1/n)$ et des fractions donne


```math
C_{n+1}-C_n
=\frac1{n+1}-\ln(1+1/n)-\frac1{2(n+1)}+\frac1{2n}
+\frac1{12(n+1)^2}-\frac1{12n^2}=O(n^{-4}).
```


Or $C_n\to\gamma$, donc $C_n-\gamma=O(\sum_{k\geq n}k^{-4})=O(n^{-3})$.
Ainsi $H_n=\ln n+\gamma+1/(2n)-1/(12n^2)+O(n^{-3})$.

## 37

Pour $k\geq2$, $0<2-3^{1/k}<1$, donc $u_n$ décroît et converge. De plus


```math
\ln(2-3^{1/k})=-\frac{\ln3}{k}+O(k^{-2}).
```


La série $\sum_{k\geq2}[\ln(2-3^{1/k})+(\ln3)/k]$ converge. Comme $H_n-\ln n\to\gamma$, on obtient $\ln u_n+\ln3\ln n\to C$; ainsi $u_n\sim C_0n^{-\ln3}$ avec $C_0=e^C>0$, et en particulier $u_n\to0$.

## 38

1. $S_n\to+\infty$, sinon $a_nS_n\to0$; et $a_n\to0$, car $a_nS_n\to1$ tandis que $S_n\to\infty$.
2. $S_{n+1}/S_n=1+a_{n+1}/S_n\to1$, puisque $a_{n+1}S_{n+1}\to1$ et $S_n\to\infty$.
3. $S_{n+1}^2-S_n^2=2a_{n+1}S_n+a_{n+1}^2\to2$, par 2) et $a_{n+1}S_{n+1}\to1$. La différence imprimée $S_{n+1}^2-S_{n+2}^2$ a donc pour limite $-2$, et non $2$.
4. En sommant les accroissements de $S_n^2$, $S_n^2\sim2n$, donc $S_n\sim\sqrt{2n}$. Comme $a_nS_n\to1$, $a_n\sim1/\sqrt{2n}$.
5. Si $b_n\sim1/\sqrt{2n}$, alors $\sum_{k=0}^nb_k\sim\sqrt{2n}$ par comparaison aux sommes de Riemann; leur produit avec $b_n$ tend vers $1$.

## 39

1. On lit la somme $\sum_{k=0}^{\infty}a_k/3^k$ ; la borne supérieure $n$ imprimée ne définit pas une application sur les suites.
Elle converge absolument puisque $0\leq a_k\leq2$.
Si deux suites diffèrent pour la première fois à l'indice $m$, le terme d'indice $m$ diffère de $2/3^m$, alors que


```math
\sum_{k>m}\frac2{3^k}=\frac1{3^m}.
```


Leurs images sont donc distinctes.

2. Pour une suite de points de $K$ convergeant vers $x$, extraire successivement une sous-suite à chiffre $0$ constant, puis à chiffre $1$ constant, etc.
L'extraction diagonale fournit des chiffres $a_k\in\{0,2\}$ et converge vers $\sum a_k/3^k$, car le reste après le chiffre $m$ est au plus $3^{-m}$. Cette limite est $x$ : $x\in K$. Donc $K$ est fermé.

En fixant les chiffres $a_0,\ldots,a_m$, les points possibles sont contenus dans un intervalle


```math
\left[\sum_{k=0}^m\frac{a_k}{3^k},
\sum_{k=0}^m\frac{a_k}{3^k}+3^{-m}\right].
```


Ces $2^{m+1}$ intervalles sont séparés par des trous. Tout intervalle inclus dans $K$ doit donc être inclus dans un seul d'entre eux, de longueur $3^{-m}$, pour chaque $m$.
Sa longueur est nulle : $K$ ne contient aucun intervalle non trivial.

3. L'application $A\mapsto\sum_{k\geq0}2\mathbf1_A(k)/3^k$ injecte $\mathcal P(\mathbb N)$ dans $\mathbb R$.
Fixons une énumération $(q_n)$ de $\mathbb Q$. L'application


```math
x\longmapsto\{n\in\mathbb N:q_n<x\}
```


injecte $\mathbb R$ dans $\mathcal P(\mathbb N)$, par densité des rationnels.

## 40

1. Toute constante convient puisque $\sum_{n\geq1}2^{-n}=1$.
Réciproquement, posons $g=f-f(0)$ ; $g$ satisfait la même identité et $g(0)=0$.
Si $g$ n'est pas nulle sur $[0,1)$, quitte à changer son signe, il existe $x_0<1$ tel que


```math
M=\max_{[0,x_0]}g>0.
```


Soit $y\in(0,x_0]$ un point réalisant ce maximum. Tous les $y^n$ appartiennent à $[0,x_0]$, donc


```math
0=M-g(y)=\sum_{n\geq1}2^{-n}(M-g(y^n)).
```


Les termes sont positifs ; ils sont tous nuls. Mais $y^n\to0$, donc $M=\lim_ng(y^n)=g(0)=0$, contradiction.
Ainsi $f$ est constante sur $[0,1)$, puis sur $[0,1]$ par continuité.

2. Pour $M=\|f\|_\infty$,


```math
|f(x)|\leq M\sum_{n\geq1}3^{-n}=\frac M2.
```


En prenant le supremum, $M\leq M/2$, donc $f=0$ ; cette fonction convient.

## 41

Posons $T_n=\sum_{k\geq n}u_k$ et $R_0=S$. Pour $n\geq0$, définir


```math
\varepsilon_n=\begin{cases}1,&u_n\leq R_n,\\0,&u_n>R_n,\end{cases}
\qquad R_{n+1}=R_n-\varepsilon_nu_n.
```


Montrons par récurrence que $0\leq R_n\leq T_n$.
C'est vrai en $0$. Si $\varepsilon_n=1$, alors


```math
0\leq R_{n+1}\leq T_n-u_n=T_{n+1}.
```


Si $\varepsilon_n=0$, alors


```math
0\leq R_{n+1}=R_n<u_n\leq T_{n+1}
```


par l'hypothèse sur $u_n$.
Comme $T_n\to0$, $R_n\to0$. Or


```math
S-R_{N+1}=\sum_{n=0}^N\varepsilon_nu_n.
```


Ainsi $S=\sum_{n\geq0}\mathbf1_A(n)u_n$, avec $A=\{n:\varepsilon_n=1\}$.
