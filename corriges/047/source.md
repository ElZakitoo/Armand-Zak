# corrigé zakito

[Énoncé](https://christophebertault.fr/documents/coursetexercices/Exercices%20-%20Series%20et%20familles%20sommables.pdf)

## 1

1. $\sqrt[n]n=\exp(\ln n/n)\to1$, donc $1/(n\sqrt[n]n)\sim1/n$ : divergence.
2. $n/(2^n+n)\sim n/2^n$ : convergence.
3. $n^2e^{-\sqrt n}\to0$, donc comparaison à $1/n^2$ : convergence.
4. $\sin(1/\sqrt n)\sim n^{-1/2}$, donc le terme est équivalent à $n^{-3/2}$ : convergence.
5. Le quotient vaut $(n+1)^3/[(3n+1)(3n+2)(3n+3)]\to1/27$ : convergence.
6. $(n/(n+1))^{n^2}=\exp[-n^2\ln(1+1/n)]\leq e^{-n/2}$ pour $n$ grand : convergence.
7. $n^2\ln n/a^n$ : convergence si $a>1$ ; terme non nul à la limite si $0<a\leq1$, donc divergence.
8. $(\ln n)^{-\ln n}=n^{-\ln\ln n}\leq n^{-2}$ pour $n$ grand : convergence.
9. Si $|a|<1$, $|a^n/(1+a^{2n})|\leq|a|^n$ ; si $|a|>1$, le module est au plus $|a|^{-n}$. Convergence absolue dans les deux cas. Si $a=\pm1$, le terme ne tend pas vers zéro : divergence.
10. $(\ln n)^{-n}\leq2^{-n}$ pour $n$ grand : convergence.
11. $1/\ln(n^2+1)\sim1/(2\ln n)\geq1/n$ pour $n$ grand : divergence.
12. $\sqrt{4n^2+1}-2n=1/(\sqrt{4n^2+1}+2n)\sim1/(4n)$, donc


```math
\sin(\pi\sqrt{4n^2+1})=\sin\bigl(\pi(\sqrt{4n^2+1}-2n)\bigr)\sim\frac\pi{4n}>0.
```


Divergence.
13. Pour $a_n=(n!)^{-1}\prod_{k=2}^n\ln k$, $a_{n+1}/a_n=\ln(n+1)/(n+1)\to0$ : convergence.
14. Pour $a_n=(n!)^2/2^{n^2}$, $a_{n+1}/a_n=(n+1)^2/2^{2n+1}\to0$ : convergence.
15. $\ln(\cos^n(n^{-\alpha}))=-\frac12n^{1-2\alpha}(1+O(n^{-2\alpha}))$. Si $0<\alpha<1/2$, le terme est au plus $e^{-n^{1-2\alpha}/4}=o(n^{-2})$ : convergence. Si $\alpha=1/2$, il tend vers $e^{-1/2}$ ; si $\alpha>1/2$, vers $1$ : divergence.
16. $e-(1+1/n)^n\sim e/(2n)$ : divergence.
17. Avec $x=t/n$ et $\sin x/(1+x)\sim x$,


```math
\int_0^{\pi/n}\frac{\sin x}{1+x}\,dx\sim\frac{\pi^2}{2n^2}.
```


Convergence.
18. $n\ln(1+1/n)=1-1/(2n)+O(n^{-2})$, donc


```math
n^{-n\ln(1+1/n)}=\frac1n\exp\left(\frac{\ln n}{2n}+O\left(\frac{\ln n}{n^2}\right)\right)\sim\frac1n.
```


Divergence.
19. $e^x\tan x\sim x$ en $0$, donc l'intégrale est équivalente à $\pi^2/(8n)$ : divergence.
20. $(1-1/\ln n)^{\sqrt n}\leq e^{-\sqrt n/\ln n}=o(n^{-2})$ : convergence.
21. $a^{\ln n}/\sqrt[n]n\sim n^{\ln a}$ : convergence si et seulement si $0<a<e^{-1}$.
22. Le quotient vaut $(n+1)^\alpha/[(2n+2)(2n+1)]\sim n^{\alpha-2}/4$. Il tend vers $0$ pour $\alpha<2$, vers $1/4$ pour $\alpha=2$, et vers $+\infty$ pour $\alpha>2$. Convergence si et seulement si $\alpha\leq2$.
23. $\ln(n!)\geq\lfloor n/2\rfloor\ln(n/2)$, donc $1/[n\ln(n!)]=O(n^{-2})$ : convergence.
24. $1/(n\cos^2n)\geq1/n$ : divergence.
25. Le quotient vaut


```math
\frac{\ln(n+1)}{n+1}\left(\frac{\ln(n+1)}{\ln n}\right)^n
\sim\frac{\ln n}{n}e^{1/\ln n}\longrightarrow0.
```


Convergence.

## 2

1. Pour $n\geq2$,


```math
\ln(1+(-1)^n/n)=\frac{(-1)^n}{n}+O(n^{-2}).
```


Convergence conditionnelle ; la valeur absolue est équivalente à $1/n$.

2.


```math
\frac{(-1)^n}{\sqrt n+(-1)^n}
=\frac{(-1)^n}{\sqrt n}-\frac1n+O(n^{-3/2}).
```


La première série converge, la deuxième tend vers $-\infty$, la troisième converge absolument : divergence vers $-\infty$.

3. Pour $\alpha>1/2$,


```math
(-1)^n\sqrt n\sin(n^{-\alpha})
=(-1)^nn^{1/2-\alpha}+O(n^{1/2-3\alpha}),
```


avec un reste sommable. Convergence si $\alpha>1/2$, absolue si $\alpha>3/2$. Pour $0<\alpha\leq1/2$, le terme ne tend pas vers zéro.

4. La moyenne géométrique $(n!)^{1/n}$ est croissante et tend vers l'infini, puisque


```math
(n!)^{1/n}\geq(n/2)^{\lfloor n/2\rfloor/n}.
```


Le critère alterné donne la convergence. Mais $(n!)^{1/n}\leq n$, donc la série absolue majore l'harmonique : convergence conditionnelle.

5. $\sqrt{n+1}-\sqrt n=1/(\sqrt{n+1}+\sqrt n)$ décroît vers $0$ et est équivalent à $1/(2\sqrt n)$ : convergence conditionnelle.

6.


```math
\frac{(-1)^n}{n^{2/3}+\sin n}
=\frac{(-1)^n}{n^{2/3}}+O(n^{-4/3}).
```


Convergence conditionnelle ; le module est équivalent à $n^{-2/3}$.

7.


```math
\sin(\pi\sqrt{n^2+1})
=(-1)^n\left(\frac\pi{2n}+O(n^{-3})\right).
```


Convergence conditionnelle.

8. $b(x)=(\ln x)^2/\sqrt x\to0$ et


```math
b'(x)=x^{-3/2}\left(2\ln x-\frac12(\ln x)^2\right)<0\quad(x>e^4).
```


Le critère alterné donne la convergence. Comme $b(n)\geq1/\sqrt n$ pour $n\geq e$, elle n'est pas absolue.

9. Si $\alpha<0$, le terme tend vers $1$ : divergence. Pour $\alpha>0$ et $n$ assez grand,


```math
\frac{(-1)^n}{n^\alpha+(-1)^n}
=\frac{(-1)^n}{n^\alpha}
-\frac1{n^\alpha(n^\alpha+(-1)^n)}.
```


La première série converge et le second terme est positif, équivalent à $n^{-2\alpha}$.
Convergence si et seulement si $\alpha>1/2$ ; divergence vers $-\infty$ pour $0<\alpha\leq1/2$.
La convergence absolue a lieu si et seulement si $\alpha>1$.

## 3

1. (a) $\sum_{n=1}^N1/[n(n+1)]=1-1/(N+1)\to1$.

(b) $\sum_{n\geq1}nx^n=x/(1-x)^2$ pour $|x|<1$ ; avec $x=1/7$, somme $7/36$.

(c)


```math
\sum_{n=r}^N\frac1{(3n+1)(3n+4)}
=\frac13\left(\frac1{3r+1}-\frac1{3N+4}\right).
```


Somme $1/3$ à partir de $n=0$, ou $1/12$ à partir de $n=1$.

(d) Pour $n\geq2$,


```math
\prod_{n=2}^N\left(1-\frac1{n^2}\right)=\frac{N+1}{2N}\longrightarrow\frac12.
```


La somme des logarithmes vaut $-\ln2$.

2. (a) Avec $H_n=\ln n+\gamma+o(1)$,


```math
\sum_{k=1}^{2n}\frac{(-1)^{k-1}}k=H_{2n}-H_n\longrightarrow\ln2.
```


Les sommes impaires ont la même limite.

(b) Par $1/[n(n+1)]=1/n-1/(n+1)$, somme $1-2\ln2$.

3.


```math
\prod_{k=1}^N\cos(2^{-k})
=\frac{\sin1}{2^N\sin(2^{-N})}\longrightarrow\sin1.
```


La somme à partir de $n=1$ vaut $\ln(\sin1)$ ; à partir de $n=0$, elle vaut $\ln(\sin2/2)$.

## 4

La somme partielle est


```math
S_N=(1+a+b)\ln(N!)+(a+b)\ln(N+1)+b\ln(N+2)-b\ln2.
```


Pour qu’elle converge, il faut $1+a+b=0$ et $a+2b=0$: ainsi $a=-2$, $b=1$. Alors le terme est $\ln[n(n+2)/(n+1)^2]$ et $S_N=\ln((N+2)/(2(N+1)))\to-\ln2$.

## 5

1. $\ln(1+1/n)=1/n+O(n^{-2})$; le critère alterné donne la convergence.
2. La somme partielle est le logarithme du produit $P_n=\prod_{k=1}^n((k+1)/k)^{(-1)^k}$. Pour $n=2m$,


```math
P_{2m}=\prod_{j=1}^m\frac{(2j-1)(2j+1)}{(2j)^2}=\frac{(2m+1)\binom{2m}{m}^2}{16^m}.
```


3. Wallis donne $\binom{2m}{m}\sim4^m/\sqrt{\pi m}$, donc $P_{2m}\to2/\pi$. Les termes tendant vers zéro, les sommes partielles impaires ont la même limite; la somme est $\ln(2/\pi)$.

## 6

1. Posons $a_n=\sum_{k=1}^nk^{-1/2}-2\sqrt n$. Alors


```math
a_{n+1}-a_n
=-\frac1{\sqrt{n+1}(\sqrt{n+1}+\sqrt n)^2}=O(n^{-3/2}).
```


La série des différences converge absolument, donc $a_n\to a$.

2. Posons $f(x)=1/(x\ln x)$, décroissante pour $x\geq2$, et


```math
b_n=\sum_{k=2}^nf(k)-\ln\ln n.
```


Alors


```math
|b_{n+1}-b_n|
=\int_n^{n+1}f(t)\,dt-f(n+1)\leq f(n)-f(n+1).
```


La série des différences converge absolument, donc $b_n\to b$.

3. Pour $k\geq2$, $2-3^{1/k}>0$ et


```math
r_k=\ln(2-3^{1/k})+\frac{\ln3}{k}=O(k^{-2}).
```


Ainsi


```math
\ln\prod_{k=2}^n(2-3^{1/k})+\ln3\ln n
=\sum_{k=2}^nr_k-\ln3(H_n-1-\ln n)\longrightarrow L\in\mathbb R.
```


En exponentiant, l'équivalent est $c/n^{\ln3}$, avec $c=e^L>0$.

## 7

1. $\sin t/t$ se prolonge continûment en $0$, donc l’intégrale sur tout intervalle borné existe.
2. Posons $u_k=\int_{k\pi}^{(k+1)\pi}|\sin t|/t\,dt>0$. Le changement $t\mapsto t+k\pi$ donne la décomposition demandée.
3. Pour $k\geq1$, $u_{k+1}<u_k$ et $u_k\leq2/(k\pi)\to0$; $\sum(-1)^ku_k$ converge, donc les intégrales partielles aux multiples de $\pi$ convergent.

## 8

1. Si $\alpha>1$, choisir $1<\gamma<\alpha$; alors $n^{-\alpha}(\ln n)^{-\beta}=O(n^{-\gamma})$. Convergence.
2. Si $\alpha<1$, choisir $\gamma\in(\alpha,1)$. Pour $n$ assez grand, $n^{-\alpha}(\ln n)^{-\beta}\geq n^{-\gamma}$ : divergence.
3. Pour $\alpha=1$, l’intégrale $\int dx/[x(\ln x)^\beta]$ converge ssi $\beta>1$.
4. La série de Bertrand converge exactement si $\alpha>1$, ou si $\alpha=1$ et $\beta>1$.

## 9

1. $u_n=(-1)^{n(n+1)/2}n^{-\alpha}$, avec signes $-,-,+,+$ périodiquement. Si $\alpha\leq0$, le terme ne tend pas vers zéro; si $\alpha>1$, convergence absolue.
2. a) Les signes de $u_{2n-1}$ et $u_{2n}$ sont égaux, et alternent avec $n$; ainsi


```math
v_n=(-1)^n((2n-1)^{-\alpha}+(2n)^{-\alpha}).
```


Le facteur positif décroît vers zéro, donc le critère alterné donne la convergence. b) Les sommes aux indices pairs convergent; la différence entre deux sommes partielles consécutives est $u_n\to0$, donc $\sum u_n$ converge.

## 10

1. Les composantes de $\{x:\sin^2x\leq1/2\}$ sont $[k\pi-\pi/4,k\pi+\pi/4]$, de longueur $\pi/2<2$, séparées par des intervalles de longueur $\pi/2>1$.
Deux entiers consécutifs appartenant à cet ensemble sont donc dans la même composante. Trois entiers consécutifs y imposeraient une longueur au moins $2$, impossible.

2. Dans chaque bloc de trois entiers, au moins un vérifie $\sin^2n>1/2$. Donc


```math
\sum_{n=3k+1}^{3k+3}\frac{\sin^2n}{n}\geq\frac1{2(3k+3)}.
```


La série diverge par comparaison à l'harmonique.

## 11

La convergence simple ne suffit pas : $u_n=(-1)^n/\sqrt n$ donne une série convergente, alors que $\sum u_n^2=\sum1/n$ diverge.
Si $\sum|u_n|<\infty$, alors $u_n\to0$ et $u_n^2\leq|u_n|$ à partir d'un rang. Donc $\sum u_n^2$ converge.

## 12

1. Si $u_n\geq0$ ne tend pas vers $0$, les termes $u_n/(1+u_n)$ non plus : les deux séries divergent.
Si $u_n\to0$, alors


```math
\frac{u_n}2\leq\frac{u_n}{1+u_n}\leq u_n
```


à partir d'un rang. Les deux séries ont même nature.

2. La convergence de $\sum u_n$ entraîne $u_n\to0$. Pour $n$ assez grand, $|u_n|\leq1/2$, donc


```math
0\leq u_n-\frac{u_n}{1+u_n}=\frac{u_n^2}{1+u_n}\leq2u_n^2.
```


La série de cette différence converge absolument ; $\sum u_n/(1+u_n)$ converge.

## 13

1. (a) $v_n\leq\sum_jv_j$, donc $\sum u_nv_n\leq(\sum u_n)(\sum v_n)<\infty$.

(b) Sans positivité, $u_n=v_n=(-1)^n/\sqrt n$ donnent deux séries convergentes, mais $u_nv_n=1/n$.

2. Cauchy-Schwarz appliquée aux sommes partielles donne


```math
\sum_n\sqrt{u_nv_n}\leq\left(\sum_nu_n\right)^{1/2}\left(\sum_nv_n\right)^{1/2},
```




```math
\sum_{n\geq1}\frac{\sqrt{u_n}}n
\leq\left(\sum_{n\geq1}u_n\right)^{1/2}\left(\sum_{n\geq1}\frac1{n^2}\right)^{1/2}.
```


Les deux séries convergent.

## 14

1. (a) La suite décroissante $u_n$ tend vers $0$, donc $u_n\geq0$. De plus,


```math
\frac n2u_n\leq\sum_{k=\lfloor n/2\rfloor+1}^nu_k\longrightarrow0.
```


Donc $u_n=o(1/n)$.

(b) La réciproque est fausse : $u_n=1/(n\ln n)$ pour $n\geq2$ est décroissante, $o(1/n)$, et sa série diverge.

2. Posons $N=\lambda(x)$. Pour $M<N$,


```math
\frac{N-M}x\leq\sum_{n=M+1}^N\frac1{\varphi(n)}
\leq\sum_{n>M}\frac1{\varphi(n)}.
```


Donc $N/x\leq M/x+\sum_{n>M}1/\varphi(n)$. D'abord $x\to\infty$, puis $M\to\infty$ : $\lambda(x)=o(x)$.

## 15

1. (a)


```math
\frac{(n+1)^\beta u_{n+1}}{n^\beta u_n}
=1+\frac{\beta-\alpha}n+o(1/n)<1
```


à partir d'un rang si $\beta<\alpha$.

(b) Choisir $1<\beta<\alpha$ ; alors $u_n\leq Cn^{-\beta}$, donc convergence.

2. Pour $u_n=\binom{2n}{n}/(4^nn)$,


```math
\frac{u_{n+1}}{u_n}
=\frac{2n+1}{2n+2}\frac n{n+1}
=1-\frac3{2n}+O(n^{-2}).
```


La règle précédente, avec $\alpha=3/2$, donne la convergence.

## 16

1. a) Somme par parties : $\sum_{k=0}^nu_kv_k=u_nV_n+\sum_{k=0}^{n-1}(u_k-u_{k+1})V_k$. C’est l’analogue discret de l’intégration par parties. b) Pour $p\leq q$, la formule appliquée au bloc donne $|\sum_{k=p}^qu_kv_k|\leq2M u_p$, où $M=\sup|V_n|$. Cette borne tend vers zéro; la série converge.
2. $\sum u_n/n^\alpha$ converge par Abel : $u_n$ a des sommes partielles bornées et $n^{-\alpha}$ décroît vers 0.
3. Les sommes partielles de $\omega^n$ sont bornées pour $\omega\neq1$; Abel donne $\sum\omega^nu_n$.
4. a) Pour $\sum e^{in\theta}/n^\alpha$, si $\theta\in2\pi\mathbb Z$ la condition est $\alpha>1$; sinon Abel donne convergence exactement pour $\alpha>0$. Pour $\sum\cos(n\theta)/n^\alpha$, la condition est aussi $\alpha>1$ si $\theta\in2\pi\mathbb Z$, et $\alpha>0$ sinon. Pour $\sum\sin(n\theta)/n^\alpha$, elle est $\alpha>0$ si $\theta\notin\pi\mathbb Z$; si $\theta\in\pi\mathbb Z$, la série est nulle pour tout $\alpha$.
b) $|\sin x|\geq\sin^2x=(1-\cos2x)/2$ et $|\cos x|\geq\cos^2x=(1+\cos2x)/2$.
Pour $0<\alpha\leq1$ et $\theta\notin\pi\mathbb Z$, la série $\sum\cos(2n\theta)/n^\alpha$ converge par Abel, tandis que $\sum1/n^\alpha$ diverge. Les deux minorantes données par les carrés divergent donc.
Si $\theta\in\pi\mathbb Z$, la série des sinus est nulle et celle des cosinus absolus est la série de Riemann.
Pour $\alpha>1$, les deux séries convergent par comparaison à $\sum1/n^\alpha$.

## 17

1. Si $\sum u_n=S<\infty$, alors $S_n\geq S_1>0$ et $u_n/S_n\leq u_n/S_1$. Donc convergence.

2. Pour $N\geq2$,


```math
\sum_{n=2}^N\ln\frac{S_{n-1}}{S_n}=\ln S_1-\ln S_N\longrightarrow-\infty.
```


Posons $x_n=u_n/S_{n-1}$ pour $n\geq2$. Si $x_n>1$ une infinité de fois, $u_n/S_n=x_n/(1+x_n)>1/2$ sur une sous-suite : divergence.
Sinon, à partir d'un rang,


```math
\frac{u_n}{S_n}=\frac{x_n}{1+x_n}\geq\frac{x_n}2
\geq\frac12\ln(1+x_n).
```


Or $\sum_{n=2}^N\ln(1+x_n)=\ln S_N-\ln S_1\to+\infty$.

3. Pour $n\geq2$,


```math
\frac{u_n}{S_n^2}\leq\frac{u_n}{S_{n-1}S_n}
=\frac1{S_{n-1}}-\frac1{S_n}.
```


Le télescopage majore les sommes partielles ; le premier terme est fini. Convergence.

## 18

1. Posons $S_j=\sum_{k=1}^ju_k\to S$. Par sommation par parties,


```math
\frac1n\sum_{k=1}^nku_k=S_n-\frac1n\sum_{j=1}^{n-1}S_j\longrightarrow S-S=0
```


par Cesàro. Donc $\sum_{k=1}^nku_k=o(n)$.

2. En échangeant deux sommes finies,


```math
\sum_{n=1}^N\frac{\sum_{k=1}^nku_k}{n(n+1)}
=\sum_{k=1}^Nku_k\left(\frac1k-\frac1{N+1}\right)
=S_N-\frac1{N+1}\sum_{k=1}^Nku_k\longrightarrow S.
```


La série converge et sa somme est $\sum_{k\geq1}u_k$.

## 19

Les séries entières convergent absolument pour tout $x$ :


```math
\operatorname{ch}x=\sum_{k\geq0}\frac{x^{2k}}{(2k)!},\quad \operatorname{sh}x=\sum_{k\geq0}\frac{x^{2k+1}}{(2k+1)!},\quad \cos x=\sum_{k\geq0}\frac{(-1)^kx^{2k}}{(2k)!},\quad \sin x=\sum_{k\geq0}\frac{(-1)^kx^{2k+1}}{(2k+1)!}.
```



## 20

1. Écrivons $P(X)=\sum_{k=0}^d c_kX^k$. Alors $|P(n)|/n!\leq C(1+n^d)/n!$, dont la série converge par le critère du quotient.
2. Pour $n\geq k$, $L_k(n)/n!=1/(n-k)!$, donc $\sum_{n\geq0}L_k(n)/n!=e$. Or $X^4=L_4+6L_3+7L_2+L_1$, d’où $\sum n^4/n!=15e$.

## 21

1. Chaque $1/k!$ apparaît $k+1$ fois :


```math
\sum_{n\geq0}\sum_{k\geq n}\frac1{k!}
=\sum_{k\geq0}\frac{k+1}{k!}=2e.
```



2. La somme absolue vaut $\sum_{k\geq1}k/k^3<\infty$, donc


```math
\sum_{n\geq1}\sum_{k\geq n}\frac{(-1)^k}{k^3}
=\sum_{k\geq1}\frac{(-1)^k}{k^2}=-\frac{\pi^2}{12}.
```



3. Par positivité, $\sum_{n\geq1}\sum_{k\geq n}k^{-\alpha}=\sum_{k\geq1}k^{1-\alpha}$ : somme $\zeta(\alpha-1)$ si $\alpha>2$, divergence sinon.

4. Il y a $r-1$ couples $m,n\geq1$ tels que $m+n=r$. Somme $\zeta(\alpha-1)-\zeta(\alpha)$ si $\alpha>2$, divergence sinon.

5. La famille est absolument sommable, de somme absolue $\zeta(2)$. Donc


```math
\sum_{n\geq1}(-1)^n\sum_{k\geq n}\frac1{k^3}
=\sum_{k\geq1}\frac1{k^3}\sum_{n=1}^k(-1)^n
=-\sum_{\substack{k\geq1\\k\text{ impair}}}\frac1{k^3}
=-\frac78\zeta(3).
```



6. Tout entier $m\geq1$ s'écrit de façon unique $m=2^n(2k+1)$. Pour $|z|<1$,


```math
\sum_{n\geq0}\frac{z^{2^n}}{1-z^{2^{n+1}}}
=\sum_{n,k\geq0}z^{2^n(2k+1)}
=\sum_{m\geq1}z^m=\frac z{1-z}.
```


La même décomposition avec $|z|$ justifie la convergence absolue.

## 22

1. $\sum_{p,q}|z|^p/q!=e\sum_p|z|^p$ : sommabilité si et seulement si $|z|<1$, somme $e/(1-z)$.

2. Pour tous $a,b\in\mathbb C$, somme absolue $e^{|a|+|b|}$ et somme $e^{a+b}$.

3. Pour tout $z\in\mathbb C$, avec $q^0=1$,


```math
\sum_{q\geq0}\frac1{q!}\sum_{p\geq0}\frac{(q|z|)^p}{p!}
=\sum_{q\geq0}\frac{e^{q|z|}}{q!}=\exp(e^{|z|})<\infty.
```


La somme de la famille vaut donc


```math
\sum_{q\geq0}\frac{e^{qz}}{q!}=\exp(e^z).
```



4. En regroupant par $r=p+q$, la somme absolue vaut $\sum_{r\geq0}(2|z|)^r$ : condition $|z|<1/2$. La somme est $1/(1-2z)$.

## 23

Les familles développées sont absolument sommables : pour un exposant $m$ fixé, le nombre de couples est au plus $m+1$, et $\sum_{m\geq0}(m+1)|z|^m<\infty$.

1. Le coefficient de $z^m$ dans le membre gauche compte les décompositions $m=(2n+1)(j+1)$ avec $n,j\geq0$, soit les diviseurs impairs adéquats; dans le membre droit, il compte les décompositions $m=n(2j+1)$, même ensemble après échange des facteurs.
2. Après développement géométrique, les coefficients sont les sommes des signes $(-1)^n$ (à gauche) ou $(-1)^j$ (à droite) sur les couples $(n,j)\in\mathbb N^2$ vérifiant $m=n+(2n+1)j=n+j+2nj$. L’involution $(n,j)\mapsto(j,n)$ échange ces deux coefficients.
3. Dans $\sum_{n\geq1}z^n/(1-z^n)$, le coefficient de $z^m$ est le nombre de diviseurs positifs de $m$, donc $d(m)$.

## 24

1. $\sum_{n\geq0}(2n+1)^{-2}=(1-2^{-2})\zeta(2)=\pi^2/8$; $\sum_{n\geq1}(-1)^n/n^2=-\eta(2)=-\pi^2/12$.
2. $\sum_{m,n\geq1}1/(m^2n^2)=\zeta(2)^2=\pi^4/36$.
3. Par symétrie, la somme sur $m<n$ vaut $\frac12(\zeta(2)^2-\zeta(4))=\pi^4/120$.
4. Écrivons $n=mk$ : $\sum_{m\mid n}m^{-2}n^{-2}=\zeta(4)\zeta(2)=\pi^6/540$.
5. Les termes sont négatifs exactement lorsque $m,n$ sont tous deux impairs. La somme vaut $\zeta(2)^2-2[(1-2^{-2})\zeta(2)]^2=-\pi^4/288$.
6. Par décomposition en pgcd, $\zeta(2)^2=\zeta(4)\sum_{(m,n)=1}m^{-2}n^{-2}$; la somme demandée est $5/2$.

## 25

1. a) Permutation des sommes : $\sum_{n\geq2}\sum_{p\geq2}(-1)^p/n^p=\sum_{n\geq2}1/[n(n+1)]=1/2$. b) $\sum_{p\geq1}\zeta(2p)/4^p=\sum_{n\geq1}1/(4n^2-1)=1/2$ par télescopage.
2. a) $\sum_{n\geq2}[-\ln(1-1/n)-1/n]=1-\gamma$. b) La contribution $n=1$ est $1-\ln2$; pour $n\geq2$, elle vaut $1/n-\ln(1+1/n)$. La somme de ces termes est $\gamma+\ln2-1$; total $\gamma$.

## 26

1. Pour chaque $p$, la somme sur $q\geq0$ télescope : $\sum_q[(p^2+q)^{-1}-(p^2+q+1)^{-1}]=p^{-2}$. La somme totale est $\zeta(2)$.
2. En posant $n=p^2+q$, chaque $n$ est compté $\lfloor\sqrt n\rfloor$ fois. Donc $\sum_{n\geq1}\lfloor\sqrt n\rfloor/[n(n+1)]=\zeta(2)$.

## 27

Le coefficient du pôle $X=-k$ vaut


```math
\frac1{\prod_{0\leq j\leq n,\,j\ne k}(j-k)}
=\frac{(-1)^k}{k!(n-k)!}.
```


Donc


```math
\frac1{X(X+1)\cdots(X+n)}
=\sum_{k=0}^n\frac{(-1)^k}{k!(n-k)!(X+k)}.
```


Fixons $z\notin-\mathbb N$. Alors $M_z=\sup_{k\geq0}|z+k|^{-1}<\infty$ et


```math
\sum_{j,k\geq0}\frac1{j!k!|z+k|}\leq M_ze^2<\infty.
```


On peut donc sommer l'identité précédente en posant $j=n-k$ :


```math
\sum_{n\geq0}\frac1{z(z+1)\cdots(z+n)}
=\left(\sum_{j\geq0}\frac1{j!}\right)
\left(\sum_{k\geq0}\frac{(-1)^k}{k!(z+k)}\right)
=e\sum_{k\geq0}\frac{(-1)^k}{k!(z+k)}.
```



## 28

Pour $\alpha>0$, sur la couronne $\max(m,n)=r$, il y a $2r-1$ couples et $r^\alpha\leq m^\alpha+n^\alpha\leq2r^\alpha$. Sa contribution est comparable à $r^{1-\alpha}$; la série converge exactement si $\alpha>2$. Si $\alpha\leq0$, les termes ne tendent pas vers zéro.

## 29

1. Si $\alpha\leq0$, les termes ne tendent pas vers $0$. Si $\alpha>0$,


```math
\sum_{p\geq2}n^{-\alpha p}=\frac{n^{-2\alpha}}{1-n^{-\alpha}}\asymp n^{-2\alpha}.
```


Sommabilité si et seulement si $\alpha>1/2$.

2. La sous-famille $p=n+1$ a pour valeurs absolues $1/(2n+1)$ : non-sommabilité.

3. Si $|z|\leq1$, $|z|^{pq}/(p!q!)\leq1/(p!q!)$ : sommabilité. Si $r=|z|>1$,


```math
\sum_{p,q\geq0}\frac{r^{pq}}{p!q!}=\sum_{p\geq0}\frac{e^{r^p}}{p!}=+\infty,
```


car $r^p-\ln(p!)\to+\infty$. Condition : $|z|\leq1$.

4. Par positivité et télescopage,


```math
\sum_{n,p\geq1}\frac1{np(n+p)}
=\sum_{n\geq1}\frac{H_n}{n^2}<\infty,
```


car $H_n\leq1+\ln n$. La famille est sommable.

5. Si $a,b>1$,


```math
\frac1{a^p+b^q}\leq\frac12a^{-p/2}b^{-q/2},
```


donc sommabilité. Si $a\leq1$, les termes ne tendent pas vers $0$ quand $p\to\infty$ à $q$ fixé ; de même pour $b\leq1$. Condition : $a>1$ et $b>1$.

6. Une infinité de rationnels de $(1,2)$ donnent chacun un terme au moins $1/4$ : non-sommabilité.

## 30

1. $\sum a_n|x|^n\leq\sum a_n=1$ : convergence absolue pour $|x|<1$.

2. $0\leq b_n\leq1$, donc convergence absolue. Puis


```math
\sum_{n\geq0}b_nx^n
=\sum_{k\geq0}a_k\sum_{n\geq k}x^n=\frac{A(x)}{1-x}.
```



3. (a) $c_0=0$. Si $0\leq c_k\leq1$ pour $k<n$, alors


```math
0\leq c_n=a_n+\sum_{k=1}^{n-1}c_ka_{n-k}
\leq a_n+\sum_{k=1}^{n-1}a_{n-k}\leq1.
```


Conclusion par récurrence.

(b) Ainsi $C(x)=\sum c_nx^n$ converge absolument pour $|x|<1$. Le produit de Cauchy donne $C=A+CA$. Comme $a_0=0$,


```math
|A(x)|\leq\sum_{n\geq1}a_n|x|^n\leq|x|<1,
```


donc $C(x)=A(x)/(1-A(x))$.

## 31

1. Si $(u_n)$ décroît et est positive, pour $2^k\leq n<2^{k+1}$,


```math
2^ku_{2^{k+1}}\leq\sum_{n=2^k}^{2^{k+1}-1}u_n\leq2^ku_{2^k}.
```


Les sommes par blocs sont donc comparables à $2^ku_{2^k}$, d’où le critère de condensation.
2. La condensation transforme $\sum n^{-\alpha}$ en $\sum 2^{k(1-\alpha)}$, convergente exactement pour $\alpha>1$.
3. Appliquer la condensation à $u_n=1/[n(\ln n)^\beta]$ (décroissante à partir d’un rang) donne la série comparable à $\sum k^{-\beta}$; condition $\beta>1$.

## 32

1. $\sum_n|(a*b)_n|\leq\sum_d|a_d|\sum_m|b_m|=\|a\|_1\|b\|_1$. Par convergence absolue,


```math
\sum_n(a*b)_n=\sum_{d,m}a_db_m=(\sum_da_d)(\sum_mb_m).
```


2. a) $d(n)=\sum_{ab=n}1$, donc $\sum d(n)n^{-\alpha}=\sum_{a,b}(ab)^{-\alpha}=\zeta(\alpha)^2$.
b) $\sigma(n)=\sum_{d\mid n}d$, donc $\sum_n\sigma(n)n^{-\alpha}=\sum_{d,m}d/(dm)^\alpha=\zeta(\alpha)\zeta(\alpha-1)$.

## 33

1. Pour correspondre au produit portant sur $p\leq n$, il faut prendre $E_n$ comme l'ensemble des entiers sans facteur premier inférieur ou égal à $n$.
Dans la série absolument convergente $\sum_{m\geq1}m^{-\alpha}$, multiplier par $(1-p^{-\alpha})$ supprime exactement les termes dont l'indice est divisible par $p$.
En procédant pour les nombres premiers $p\leq n$,


```math
\zeta(\alpha)\prod_{p\leq n}(1-p^{-\alpha})=\sum_{m\in E_n}m^{-\alpha}.
```


Avec « strictement inférieur » tel qu'imprimé, l'égalité manque le facteur associé à $n$ lorsque $n$ est premier.

2. $E_n$ contient $1$ et, pour le reste, seulement des entiers $m>n$. Donc


```math
1\leq\sum_{m\in E_n}m^{-\alpha}\leq1+\sum_{m>n}m^{-\alpha}\longrightarrow1.
```


En divisant l'égalité de 1, le produit inverse tend vers $\zeta(\alpha)$.

## 34

1. a) Pour chaque $i\in F$, l’intersection des $I_n$ est vide; il existe donc $N_i$ tel que $i\notin I_{N_i}$. Prendre $N=\max_{i\in F}N_i$.
b) Pour $\varepsilon>0$, choisir un ensemble fini $F$ tel que $\sum_{i\notin F}x_i<\varepsilon$. Pour $n$ assez grand, $F\cap I_n=\varnothing$, donc $\sum_{i\in I_n}x_i\leq\varepsilon$.
2. Choisir un ensemble fini $F$ tel que $\sum_{i\notin F}|z_i|<\varepsilon$. Pour $n$ assez grand, $F\subset I_n$; alors $|\sum_{i\in I}z_i-\sum_{i\in I_n}z_i|\leq\sum_{i\notin I_n}|z_i|\leq\varepsilon$.

## 35

À chaque partie finie $F\subset\mathbb N$ associons $\sum_{k\in F}2^k$. Cette application est injective par unicité de l’écriture binaire; donc $\mathcal P_f(\mathbb N)$ est dénombrable.

## 36

Tout élément de $\langle X\rangle$ est un mot fini en lettres de $X\cup X^{-1}$. L’ensemble des mots de longueur $n$ est au plus dénombrable (produit fini d’ensembles dénombrables); leur réunion sur $n\in\mathbb N$ est dénombrable.

## 37

1. Les rationnels sont algébriques; $i$ annule $X^2+1$, $\sqrt2$ annule $X^2-2$, et $\sqrt2+\sqrt3$ annule le polynôme entier obtenu en éliminant les racines, par exemple $X^4-10X^2+1$.
2. Il existe une réunion dénombrable de polynômes non nuls à coefficients entiers; chaque polynôme a un nombre fini de racines. Ainsi $A$ est dénombrable. Comme $\mathbb R$ est non dénombrable, $\mathbb R\setminus A$ est non dénombrable.

## 38

1. Écrivons $X=\{x_1<\cdots<x_r\}\subset(a,b)$. Par croissance,


```math
f(a)\leq f(x_1^-)\leq f(x_1^+)\leq f(x_2^-)\leq\cdots\leq f(x_r^+)\leq f(b).
```


Donc $\sum_{x\in X}(f(x^+)-f(x^-))\leq f(b)-f(a)$.

2. À l'intérieur de $I$, $f(x^-)\leq f(x)\leq f(x^+)$ ; une discontinuité équivaut donc à un saut strictement positif.
Sur tout segment $[a,b]\subset I$, les sauts de taille au moins $1/m$ dans $(a,b)$ sont en nombre au plus $m(f(b)-f(a))$.
Réunir ces ensembles finis sur $m\geq1$, puis sur une suite dénombrable de segments recouvrant l'intérieur de $I$. Ajouter les éventuelles extrémités de $I$ : l'ensemble des discontinuités est au plus dénombrable.

## 39

Supposons $\mathbb R^2$ réunion dénombrable de droites $(D_n)$. La parabole $\{(x,x^2):x\in\mathbb R\}$ rencontre chaque droite en au plus deux points, sauf si la droite est verticale, auquel cas elle en rencontre un. L’union dénombrable de ces intersections serait dénombrable, alors que la parabole est non dénombrable : contradiction.

## 40

1. La relation est réflexive et symétrique. Si $[x,y]\subset O$ et $[y,z]\subset O$, alors les deux segments unissent $x$ à $z$ sans trou car ils partagent $y$; leur union contient $[x,z]$, donc la relation est transitive. La classe d’un point est l’union des intervalles ouverts contenus dans $O$ qui le contiennent; elle est un intervalle ouvert.
2. a) Des intervalles disjoints de longueur supérieure à $\varepsilon$ inclus dans un intervalle borné sont en nombre fini : pour $r$ tels intervalles, la somme des longueurs est au plus la longueur d’un intervalle contenant $O$, donc $r\varepsilon$ est borné.
b) Pour chaque composante non vide, choisissons un rationnel qu’elle contient. Les composantes disjointes donnent des rationnels distincts; elles sont donc dénombrables et $O$ est leur réunion.
3. Pour $O$ non borné, chaque composante contient un rationnel distinct; le même argument de dénombrabilité s’applique.
