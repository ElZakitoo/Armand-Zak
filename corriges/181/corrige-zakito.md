# corrigé zakito

[Énoncé](http://christophebertault.fr/documents/dm/DM%20-%20Deux%20ou%20trois%20jolies%20idees%20sur%20les%20nombres%20premiers.pdf)

## 1

### a

$$g(t)=\ln(1-t)+t+\frac{t^2}{2(1-t)},\qquad g(0)=0.$$
$$g'(t)=-\frac1{1-t}+1+\frac{2t-t^2}{2(1-t)^2}=\frac{t^2}{2(1-t)^2}\ge0\qquad(0\le t<1).$$
$$\boxed{\ln(1-t)+t+\frac{t^2}{2(1-t)}\ge0.}$$

### b

$$t=\frac1p\Rightarrow\frac1p\ge-\ln\left(1-\frac1p\right)-\frac1{2p(p-1)}.$$
$$\boxed{\sum_{p\le n}\frac1p\ge\ln\prod_{p\le n}\left(1-\frac1p\right)^{-1}-\frac12\sum_{p\le n}\frac1{p(p-1)}.}$$

## 2

$$\sum_{k=0}^r\frac1{p^k}=\frac{1-p^{-r-1}}{1-p^{-1}}\le\left(1-\frac1p\right)^{-1}.$$
$$R=\left\lfloor\frac{\ln n}{\ln2}\right\rfloor,\qquad1\le m\le n\Rightarrow m=\prod_{p\le n}p^{\alpha_p(m)},\quad0\le\alpha_p(m)\le R.$$
$$\prod_{p\le n}\left(1-\frac1p\right)^{-1}\ge\prod_{p\le n}\sum_{k=0}^Rp^{-k}=\sum_{(\alpha_p)\in\{0,\ldots,R\}^{\{p\le n\}}}\frac1{\prod_{p\le n}p^{\alpha_p}}\ge\boxed{\sum_{m=1}^n\frac1m}.$$

## 3

### a

$$t\in[k,k+1]\Rightarrow\frac1t\le\frac1k\Rightarrow\int_k^{k+1}\frac{dt}t\le\frac1k.$$
$$\sum_{k=1}^n\frac1k\ge\int_1^{n+1}\frac{dt}t=\ln(n+1)\ge\ln n.$$

### b

$$\sum_{p\le n}\frac1{p(p-1)}\le\sum_{k=2}^n\left(\frac1{k-1}-\frac1k\right)=1-\frac1n\le1.$$
$$\sum_{p\le n}\frac1p\ge\ln\left(\sum_{k=1}^n\frac1k\right)-\frac12\ge\boxed{\ln\ln n-\frac12}.$$

## 4

### a

$$Q_n=\prod_{n+1<p\le2n+1}p,\qquad n!\binom{2n+1}{n+1}=(n+2)(n+3)\cdots(2n+1).$$
$$\forall p\mid Q_n,\quad p\mid n!\binom{2n+1}{n+1},\quad p\nmid n!\Rightarrow p\mid\binom{2n+1}{n+1}.$$
$$Q_n\mid\binom{2n+1}{n+1},\qquad2\binom{2n+1}{n+1}=\binom{2n+1}{n}+\binom{2n+1}{n+1}\le\sum_{k=0}^{2n+1}\binom{2n+1}{k}=2^{2n+1}.$$
$$\boxed{Q_n\le4^n.}$$

### b

$$P_N=\prod_{p\le N}p,\qquad P_0=P_1=1,\quad P_2=2.$$
Récurrence forte :
$$N=2m+1\ge3\Rightarrow P_N=P_{m+1}Q_m\le4^{m+1}4^m=4^N.$$
$$N=2m\ge4\Rightarrow N\notin\mathbb P\Rightarrow P_N=P_{N-1}\le4^{N-1}\le4^N.$$
$$\boxed{\forall N\in\mathbb N,\qquad P_N\le4^N.}$$

## 5

### a

$$2\le k\le n,\quad t\in[k-1,k]\Rightarrow\ln t\le\ln k.$$
$$\ln(n!)=\sum_{k=2}^n\ln k\ge\int_1^n\ln t\,dt=n\ln n-n+1\ge n\ln n-n.$$

### b

$$p_k\ge k\Rightarrow n!\le\prod_{k=1}^np_k=P_{p_n}\le4^{p_n}.$$
$$n\ln n-n\le\ln(n!)\le2p_n\ln2\Rightarrow\boxed{p_n\ge\frac{n\ln n-n}{2\ln2}.}$$

## 6

$$\zeta_{n+1}(s)-\zeta_n(s)=(n+1)^{-s}>0.$$
$$\sum_{k=2}^nk^{-s}\le\int_1^nt^{-s}\,dt=\frac{1-n^{1-s}}{s-1}\le\frac1{s-1}.$$
$$\boxed{\zeta_n(s)\uparrow\zeta(s)\le1+\frac1{s-1}.}$$

## 7

### a

$$r=|\{p\in\mathbb P:p\le n\}|,\qquad T=\left\lfloor\frac{\ln n}{\ln2}\right\rfloor.$$
$$1\le m\le n\Rightarrow m=\prod_{i=1}^rp_i^{\alpha_i},\quad2^{\alpha_i}\le p_i^{\alpha_i}\le m\le n\Rightarrow0\le\alpha_i\le T.$$
$$\{1,\ldots,n\}\subset E_{r,T}.$$
$$p_r\le n,\qquad p_r\notin E_{r-1,t}\quad(\forall t)\Rightarrow r\text{ minimal}.$$

### b

$$\prod_{i=1}^r\sum_{j=0}^tp_i^{-sj}=\sum_{\alpha_1,\ldots,\alpha_r=0}^t\left(p_1^{\alpha_1}\cdots p_r^{\alpha_r}\right)^{-s}=\sum_{m\in E_{r,t}}m^{-s}.$$
$$t\ge T\Rightarrow\{1,\ldots,n\}\subset E_{r,t}\subset\mathbb N^*\Rightarrow\boxed{\zeta_n(s)\le\prod_{i=1}^r\sum_{j=0}^tp_i^{-sj}\le\zeta(s).}$$

### c

$$t\to+\infty:\qquad\zeta_n(s)\le\prod_{i=1}^r\frac1{1-p_i^{-s}}=\pi_n(s)\le\zeta(s).$$
$$\zeta_n(s)\to\zeta(s)\Rightarrow\boxed{\pi_n(s)\to\zeta(s).}$$

## 8

$$h(t)=t-\ln(1+t),\qquad h'(t)=\frac t{1+t},\qquad h(0)=0.$$
$$h\text{ décroissante sur }(-1,0],\text{ croissante sur }[0,+\infty)\Rightarrow h(t)\ge0.$$
$$\ln(1-p^{-s})\le-p^{-s}\Rightarrow\sum_{p\le n}p^{-s}\le-\sum_{p\le n}\ln(1-p^{-s})=\ln\pi_n(s)\le\boxed{\ln\zeta(s)}.$$

## 9

### a

$$s=1+\frac{a_n}{\ln n}>1,\qquad p\le n\Rightarrow p^{s-1}\le e^{a_n}.$$
$$\sum_{p\le n}\frac1p=\sum_{p\le n}\frac{p^{s-1}}{p^s}\le e^{a_n}\sum_{p\le n}p^{-s}\le e^{a_n}\ln\zeta(s)\le\boxed{e^{a_n}\ln\left(1+\frac{\ln n}{a_n}\right)}.$$

### b

$$n\ge3,\qquad L_n=\ln\ln n>0,\qquad a_n=\frac1{L_n}\to0.$$
$$\ln(1+L_n\ln n)=L_n+\ln L_n+\ln\left(1+\frac1{L_n\ln n}\right)=L_n+o(L_n).$$
$$1-\frac1{2L_n}\le\frac1{L_n}\sum_{p\le n}\frac1p\le e^{1/L_n}\frac{\ln(1+L_n\ln n)}{L_n}\longrightarrow1.$$
$$\boxed{\sum_{p\le n}\frac1p\sim\ln\ln n.}$$
