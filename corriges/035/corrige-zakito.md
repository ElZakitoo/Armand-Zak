# corrigé zakito
[Énoncé](https://www.bourrigan.fr/data/td35-deux-variables.pdf)

## Autocorrection A

$$
\begin{aligned}
&\text{(i)}&&p\in\mathbb R^2\Rightarrow B(p,1)\subset\mathbb R^2.\\
&\text{(ii)}&&p\ne0,\quad r=\|p\|/2>0,\quad \|z-p\|<r\Rightarrow\|z\|>\|p\|/2.\\
&\text{(iii)}&&p=(a,b)\in(0,1)^2,\quad r=\tfrac12\min(a,1-a,b,1-b)>0\\
&&&\Rightarrow B(p,r)\subset(0,1)^2.\\
&\text{(iv)}&&U=h^{-1}((0,+\infty)),\quad h(x,y)=y-\cos x\in C^0(\mathbb R^2).
\end{aligned}
$$

## Autocorrection B

$$q=p+(r,0),\qquad q\in D(p,r),\qquad q+(\varepsilon/2,0)\in B(q,\varepsilon)\setminus D(p,r).$$
$$\forall\varepsilon>0,\quad B(q,\varepsilon)\not\subset D(p,r).$$

## Exercice 1

### 1

$$p\in\bigcup_iU_i\Rightarrow\exists i,\ p\in U_i\Rightarrow\exists r>0,\ B(p,r)\subset U_i\subset\bigcup_iU_i.$$

### 2

$$p\in U\cap V,\quad B(p,r)\subset U,\quad B(p,s)\subset V\Rightarrow B(p,\min(r,s))\subset U\cap V.$$

### 3

$$U_n=\pi_2^{-1}((-1/n,1/n)),\qquad\pi_2(x,y)=y\in C^0.$$
$$\bigcap_{n\ge1}U_n=\mathbb R\times\{0\},\qquad (a,\varepsilon/2)\in B((a,0),\varepsilon)\setminus\bigcap_nU_n.$$

## Exercice 2

$$B(p,r)\subset U,\qquad g(t)=f(p+\tfrac r2(\cos t,\sin t))-f(p-\tfrac r2(\cos t,\sin t)).$$
$$g\in C^0([0,\pi]),\quad g(\pi)=-g(0)\Rightarrow\exists t_0\in[0,\pi],\ g(t_0)=0.$$
$$p+\tfrac r2(\cos t_0,\sin t_0)\ne p-\tfrac r2(\cos t_0,\sin t_0)\Rightarrow f\text{ non injective}.$$

## Exercice 3

### 1(a)

$$K=S\times T,\quad p_n=(x_n,y_n)\in K\Rightarrow\exists(n_k),\quad x_{n_k}\to x\in S,\quad y_{n_k}\to y\in T.$$
$$|f(p_n)|\ge n\Rightarrow |f(p_{n_k})|\to+\infty,\qquad f(p_{n_k})\to f(x,y),\quad\bot.$$
$$M=\sup_Kf\in\mathbb R,\quad M-1/n<f(p_n)\le M.$$
$$p_{n_k}\to p\in K\Rightarrow f(p)=\lim_kf(p_{n_k})=M.$$
$$m=\inf_Kf\in\mathbb R,\quad m\le f(q_n)<m+1/n,\quad q_{n_k}\to q\in K\Rightarrow f(q)=m.$$

### 1(b)

$$\neg\text{continuité uniforme}\Rightarrow\exists\varepsilon>0,\ (p_n),(q_n)\in K^{\mathbb N},\quad\|p_n-q_n\|\to0,\quad|f(p_n)-f(q_n)|\ge\varepsilon.$$
$$p_{n_k}\to p\in K\Rightarrow q_{n_k}\to p\Rightarrow |f(p_{n_k})-f(q_{n_k})|\to0,\quad\bot.$$

### 2

$$|F(x)-F(a)|\le\sup_{t\in[0,1]}|f(x,t)-f(a,t)|\xrightarrow[x\to a]{}0$$
par continuité uniforme sur $[a-1,a+1]\times[0,1]$.

## Autocorrection C

$$
\begin{array}{c|cc}
&\partial_x&\partial_y\\\hline
f_1&1/y&-x/y^2\\
f_2&-1/(x^2y^2)&-2/(xy^3)\\
f_3&\ln(xy)+1&x/y\\
f_4&e^{-x}(2x\cos(x^2+y^2)-\sin(x^2+y^2))&2ye^{-x}\cos(x^2+y^2)
\end{array}
$$

## Autocorrection D

$$\frac{N(h,0)-N(0,0)}h=\frac{|h|}h,\qquad\frac{N(0,h)-N(0,0)}h=\frac{|h|}h.$$
$$\partial_xN(x,y)=\frac{x}{\sqrt{x^2+y^2}},\quad\partial_yN(x,y)=\frac{y}{\sqrt{x^2+y^2}}\qquad((x,y)\ne0).$$
Ces deux fonctions sont continues sur $\mathbb R^2\setminus\{0\}$.

## Autocorrection E

$$\theta\in C^1(\mathbb R),\qquad\theta'(t)=2t\,\partial_1f(t^2,t^3)+3t^2\,\partial_2f(t^2,t^3).$$

## Autocorrection F

$$
\begin{aligned}
\partial_xu_1(x,y)&=\partial_2f(y,x),&\partial_yu_1(x,y)&=\partial_1f(y,x),\\
u_2'(x)&=\partial_1f(x,x)+\partial_2f(x,x),\\
\partial_xu_3(x,y)&=\partial_2f(y,f(x,x))[\partial_1f(x,x)+\partial_2f(x,x)],\\
\partial_yu_3(x,y)&=\partial_1f(y,f(x,x)),\\
u_4'(x)&=\partial_1f(x,f(x,x))+\partial_2f(x,f(x,x))[\partial_1f(x,x)+\partial_2f(x,x)].
\end{aligned}
$$
Les compositions et les dérivées affichées sont continues.

## Exercice 4

$$H(t)=\int_0^tf(s)\,ds\in C^1,\qquad\varphi(x,y)=H(y)-H(x).$$
$$\partial_x\varphi=-f(x),\qquad\partial_y\varphi=f(y),\qquad\varphi\in C^1(\mathbb R^2).$$

## Exercice 5

### 1

$$p\ne0\Rightarrow f\text{ de classe }C^1\text{ au voisinage de }p\Rightarrow D_vf(p)=\nabla f(p)\cdot v.$$
$$v=(a,b),\quad b\ne0:\qquad\frac{f(ta,tb)}t=\frac{a^2b}{t^2a^4+b^2}\to\frac{a^2}{b}.$$
$$b=0\Rightarrow f(ta,0)=0\Rightarrow D_{(a,0)}f(0)=0.$$

### 2

$$t\ne0\Rightarrow f(t,t^2)=\frac12\not\to f(0,0)=0.$$

## Exercice 6

$$\partial_x(f+ig)=P'(x+iy),\qquad\partial_y(f+ig)=iP'(x+iy).$$
$$P'(x+iy)=u+iv\Rightarrow f_x=u=g_y,\qquad f_y=-v=-g_x.$$

## Exercice 7

### 1

$$h(t)=f(p+t(q-p)),\qquad h'(t)=\nabla f(p+t(q-p))\cdot(q-p)=0.$$
$$f(q)=h(1)=h(0)=f(p).$$

### 2

$$U=\{(x,y):x\ne0\},\qquad f(x,y)=\begin{cases}0&x<0,\\1&x>0.\end{cases}$$
$$f\in C^1(U),\qquad\nabla f=0,\qquad f(-1,0)\ne f(1,0).$$

## Exercice 8

$$f_y=0\Rightarrow\forall x,y,\quad f(x,y)=f(x,0)=h(x),\quad h\in C^1,\quad h'(x)=f_x(x,0).$$
$$f(x,y)=h(x)\Rightarrow f_y(x,y)=0.$$

## Exercice 9

Définition corrigée : $g(r,\theta)=f(r\cos\theta,r\sin\theta)$.

### 1

$$g_r=\cos\theta\,f_x(r\cos\theta,r\sin\theta)+\sin\theta\,f_y(r\cos\theta,r\sin\theta),$$
$$g_\theta=-r\sin\theta\,f_x(r\cos\theta,r\sin\theta)+r\cos\theta\,f_y(r\cos\theta,r\sin\theta).$$

### 2

$$f\text{ radiale}\iff\forall r\ge0,\ g(r,\cdot)\text{ constante}\iff g_\theta=0\iff xf_y-yf_x=0.$$

## Exercice 10

$$f(tp)=t^kf(p)\Rightarrow \left.\frac d{dt}f(tp)\right|_{t=1}=p\cdot\nabla f(p)=kf(p).$$
Réciproquement, pour $p\ne0$ et $t>0$,
$$\frac d{dt}\left(t^{-k}f(tp)\right)=t^{-k-1}\bigl((tp)\cdot\nabla f(tp)-kf(tp)\bigr)=0.$$
$$t^{-k}f(tp)=f(p).$$

## Exercice 11

### 1

$$F(u,v)=f(u,v-2u),\qquad F_u=f_x(u,v-2u)-2f_y(u,v-2u).$$
$$f_x-2f_y=0\iff F(u,v)=h(v)\iff f(x,y)=h(2x+y),\quad h\in C^1(\mathbb R).$$

### 2

$$\left(\partial_x-2\partial_y\right)\frac{x^2}{2}=x,$$
$$\boxed{f(x,y)=\frac{x^2}{2}+h(2x+y),\qquad h\in C^1(\mathbb R).}$$

## Exercice 12

### 1

$$\frac{f(a+h,t)-f(a,t)}h=\int_0^1f_x(a+sh,t)\,ds.$$
$$\left|\frac{F(a+h)-F(a)}h-\int_0^1f_x(a,t)\,dt\right|\le\sup_{\substack{0\le s,t\le1}}|f_x(a+sh,t)-f_x(a,t)|\to0.$$
$$F'(a)=\int_0^1f_x(a,t)\,dt,\qquad F'\in C^0$$
par l'exercice 3 appliqué à $f_x$.

### 2(a)

$$\gamma'(x)=e^{-x^2},\qquad F'(x)=-2xe^{-x^2}\int_0^1e^{-x^2t^2}\,dt=-2e^{-x^2}\gamma(x).$$
La formule vaut aussi pour $x=0$.

### 2(b)

$$\bigl(F+\gamma^2\bigr)'=0,\qquad F(0)=\int_0^1\frac{dt}{1+t^2}=\frac\pi4,\qquad\gamma(0)=0.$$
$$F(x)=\frac\pi4-\gamma(x)^2.$$

### 2(c)

$$0\le F(x)\le e^{-x^2}\int_0^1\frac{dt}{1+t^2}=\frac\pi4e^{-x^2}\to0.$$
$$x\ge0\Rightarrow\gamma(x)\ge0,\qquad\boxed{\int_0^{+\infty}e^{-t^2}\,dt=\frac{\sqrt\pi}{2}.}$$

## Autocorrection G

### 1

$$\nabla f_1=(-\sin x,2y)=0\iff(x,y)=(k\pi,0).$$
$$f_1\ge-1,\qquad f_1((2k+1)\pi,0)=-1.$$
Les $((2k+1)\pi,0)$ sont des minima globaux stricts localement.
$$f_1(2k\pi+t,0)<1<f_1(2k\pi,t)\quad(0<|t|<\pi).$$
Aucun maximum local ou global.

### 2

$$\partial_yf_2=2e^{3x}y+e^x=0\Rightarrow y=-\tfrac12e^{-2x},$$
$$\partial_xf_2=3e^{3x}y^2+e^xy=\tfrac14e^{-x}>0.$$
Aucun point critique, donc aucun extremum local ou global.

### 3

$$X=x-1,\quad Y=y+1,\qquad f_3(x,y)=-8+3X^2-2XY+3Y^2=-8+2(X^2+Y^2)+(X-Y)^2.$$
Minimum global unique : $f_3(1,-1)=-8$. Aucun maximum.

### 4

$$\nabla f_4=f_4\left(\arctan y,\frac{x}{1+y^2}\right)=0\iff(x,y)=(0,0).$$
$$t\ne0:\quad f_4(t,t)>1>f_4(t,-t).$$
Aucun extremum local ou global.

## Exercice 13

### 1

$$f\in C^\infty,\qquad \nabla f=(e^y+ye^x,xe^y+e^x).$$
$$\nabla f=0\Rightarrow x<0,\ y<0,\ xy=1.$$
$$a=-x>0,\ y=-1/a,\qquad 1/a-a=\ln a.$$
$$H(a)=1/a-a-\ln a,\quad H'(a)=-1/a^2-1-1/a<0,\quad H(1)=0.$$
$$\nabla f=0\iff(x,y)=(-1,-1).$$

### 2

$$\operatorname{Hess}f(-1,-1)=e^{-1}\begin{pmatrix}-1&2\\2&-1\end{pmatrix}.$$
$$f(-1+t,-1+t)=-2/e+t^2/e+o(t^2),$$
$$f(-1+t,-1-t)=-2/e-3t^2/e+o(t^2).$$
Aucun extremum local.

## Exercice 14

$$\nabla f(p)=0,\quad v=q-p,\quad h(t)=f(p+tv).$$
$$t>0:\qquad t h'(t)=\langle\nabla f(p+tv)-\nabla f(p),tv\rangle\ge0.$$
$$f(q)-f(p)=\int_0^1h'(t)\,dt\ge0.$$

## Exercice 15

### 1

$$f=y^2-3x^2y+2x^4,\qquad\nabla f=(-6xy+8x^3,2y-3x^2).$$
$$\nabla f=0\Rightarrow y=\tfrac32x^2,\quad -x^3=0\Rightarrow(x,y)=(0,0).$$
$$f(0,t)=t^2>0=f(0,0)\quad(t\ne0).$$

### 2

$$v=(a,b),\qquad f(tv)=t^2(b-ta^2)(b-2ta^2).$$
$$b\ne0\Rightarrow (b-ta^2)(b-2ta^2)\to b^2>0;\qquad b=0\Rightarrow f(tv)=2a^4t^4\ge0.$$

### 3

$$f(t,\tfrac32t^2)=-\tfrac14t^4<0\quad(t\ne0).$$
Aucun extremum local en $(0,0)$.

## Exercice 16

Énoncé impossible tel qu'imprimé.
$$\varphi:\mathbb R^2\to(-1,1),\quad\psi=\varphi^{-1},\quad\psi\circ\varphi=\operatorname{id}_{\mathbb R^2}$$
$$\Rightarrow D\psi(\varphi(p))D\varphi(p)=I_2\Rightarrow 2=\operatorname{rg}I_2\le1,\quad\bot.$$

## Exercice 17

### 1

$$f(f(x,y),z)=f(x,f(y,z)).$$
Dérivation en $z=e$ :
$$\partial_2f(x*y,e)=\partial_2f(x,y)\partial_2f(y,e).$$

### 2

$$a(y)=\partial_2f(y,e),\qquad a(e)=1.$$
$$x=y^{-1}\Rightarrow 1=\partial_2f(y^{-1},y)a(y)\Rightarrow a(y)\ne0.$$
$$a\in C^0(\mathbb R),\quad a(e)>0\Rightarrow\forall y,\ a(y)>0.$$

### 3

$$\varphi(e)=0,\qquad \varphi(f(x,y))=\varphi(x)+\varphi(y).$$
Dérivation en $y=e$ :
$$\varphi'(x)a(x)=\varphi'(e)=c\Rightarrow\boxed{\varphi(x)=c\int_e^x\frac{dt}{a(t)}.}$$

### 4

$$c\ne0,\qquad\varphi'(x)=c/a(x)\ne0.$$
$$\frac d{dy}\bigl(\varphi(f(x,y))-\varphi(y)\bigr)=\frac{c\,\partial_2f(x,y)}{a(x*y)}-\frac c{a(y)}=0.$$
$$y=e\Rightarrow\varphi(x*y)=\varphi(x)+\varphi(y).$$
$$J=\varphi(\mathbb R)\text{ intervalle ouvert contenant }0,\qquad J+J\subset J,\quad-J=J.$$
$$(-\delta,\delta)\subset J\Rightarrow\forall n\ge1,\ (-n\delta,n\delta)\subset J\Rightarrow J=\mathbb R.$$
$$\varphi\text{ strictement monotone, surjective},\qquad(\varphi^{-1})'(u)=\frac{a(\varphi^{-1}(u))}{c}\in C^0.$$
$$\varphi:(\mathbb R,*)\simeq(\mathbb R,+),\qquad x*y=y*x.$$
Le sens de l'isomorphisme imprimé dans l'énoncé est inversé.

### 5

$$ (u,v)*(s,t)=(u+s,v+e^ut).$$
$$((u,v)*(s,t))*(a,b)=(u+s+a,v+e^ut+e^{u+s}b)=(u,v)*((s,t)*(a,b)).$$
$$e=(0,0),\qquad(u,v)^{-1}=(-u,-e^{-u}v).$$
$$(1,0)*(0,1)=(1,e)\ne(1,1)=(0,1)*(1,0).$$
