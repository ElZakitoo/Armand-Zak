# corrigé zakito

[Énoncé](https://christophebertault.fr/documents/coursetexercices/Exercices%20-%20Denombrement.pdf)

## 1

21 atouts, 14 cartes par couleur, 1 excuse.

$$\text{1.}\quad\binom{14}2^2\binom{21}3.$$
$$\text{2.}\quad\binom{21}3\binom{14}2\binom{43}2.$$
$$\text{3.}\quad\binom{14}7+63\binom{14}5+\binom{14}6.$$
$$\text{4.}\quad\binom{21}5\left(\binom{43}2+14\cdot43\right)+\binom{21}6(43+14)+\binom{21}7.$$

## 2

$$\text{RIQUIQUI}:\quad(R,I,Q,U)\mapsto(1,3,2,2)\Rightarrow\frac{8!}{3!2!2!}=1680.$$
$$\text{ABRACADABRA}:\quad(A,B,R,C,D)\mapsto(5,2,2,1,1)\Rightarrow\frac{11!}{5!2!2!}=83160.$$

## 3

$$\text{1.}\quad\binom{np}n,\qquad\text{2.}\quad p^n,\qquad\text{3.}\quad\binom p2^n.$$
$$\text{4.}\quad a_{i,\sigma(i)}=1\quad(\sigma\in\mathfrak S_n)\Rightarrow n!.$$

## 4

$$\text{1.}\quad2\times n!\times n!=2(n!)^2.$$
$$\text{2.}\quad\frac{2(n!)^2}{2n}=(n-1)!n!\qquad(n\ge1).$$
Rotations identifiées, sens de rotation conservé.

## 5

$$\text{1.}\quad y=n-x,\quad1\le x\le n-1\Rightarrow n-1.$$
$$\text{2.}\quad\sum_{y=1}^n(y-1)=\binom n2.$$
$$\text{3.}\quad\sum_{x=1}^n(2n-x)=\frac{n(3n-1)}2.$$
$$\text{4.}\quad n+2(n-1)=3n-2.$$

## 6

$$A_i=\{\text{mots de longueur 9 avec le motif commençant en position }i\}.$$
$$\text{1.}\quad|A_i|=26^4,\quad1\le i\le5,\quad A_i\cap A_j=\varnothing\ (i\ne j)\Rightarrow5\cdot26^4.$$
$$\text{2.}\quad|A_i|=26^5,\quad1\le i\le6.$$
$$A_i\cap A_j\ne\varnothing\iff j-i\ge4\quad(i<j),\qquad\#\{(i,j):j-i\ge4\}=3.$$
$$|A_i\cap A_j|=26\Rightarrow\boxed{6\cdot26^5-3\cdot26.}$$
$$\text{3.}\quad A_i\cap A_j\ne\varnothing\iff j-i=3\text{ ou }j-i\ge4.$$
$$j-i=3:\quad3\text{ couples},\quad|A_i\cap A_j|=26^2;\qquad j-i\ge4:\quad3\text{ couples},\quad|A_i\cap A_j|=26.$$
$$\text{Aucune intersection triple}\Rightarrow\boxed{6\cdot26^5-3\cdot26^2-3\cdot26.}$$

## 7

$$\frac{n(n-3)}2=n,\quad n\ge3\iff\boxed{n=5.}$$

## 8

$$N=\prod_{i=1}^rp_i^{\alpha_i},\qquad d\mid N\iff d=\prod_{i=1}^rp_i^{\beta_i},\quad0\le\beta_i\le\alpha_i.$$
$$\boxed{\tau(N)=\prod_{i=1}^r(\alpha_i+1).}$$

## 9

$$\underbrace{\binom mp}_{\text{filles}}\underbrace{\binom np}_{\text{garçons}}\underbrace{(2p)!}_{\text{classement}}.$$

## 10

$$f^2=\operatorname{id}\Rightarrow\{1,\ldots,2n+1\}=\operatorname{Fix}(f)\sqcup\bigsqcup_{j=1}^r\{x_j,f(x_j)\},\qquad f(x_j)\ne x_j.$$
$$2n+1=|\operatorname{Fix}(f)|+2r\Rightarrow|\operatorname{Fix}(f)|\text{ impair}\Rightarrow|\operatorname{Fix}(f)|\ge1.$$

## 11

$$\text{1.}\quad n\ge1:\quad2^n-2;\qquad n=0:\quad0.$$
$$\text{2.}\quad n\ge1:\quad\underbrace{\binom{n+1}2}_{\text{fibre double}}\underbrace{n!}_{\text{images des }n\text{ fibres}};\qquad n=0:\quad0.$$

## 12

$$\text{1.}\quad p\,2^{n-p},\qquad\text{2.}\quad(2^p-1)2^{n-p}=2^n-2^{n-p}.$$

## 13

$$\text{1.}\quad f\longleftrightarrow\{f(1),\ldots,f(p)\}\Rightarrow\binom np.$$
$$\text{2.}\quad1\le f(1)\le\cdots\le f(p)\le n$$
$$\iff1\le f(1)<f(2)+1<\cdots<f(p)+p-1\le n+p-1\Rightarrow\boxed{\binom{n+p-1}p.}$$

## 14

$$\text{1.}\quad R\subset E^2\Rightarrow2^{n^2}.$$
$$\text{2.}\quad\{(x,x):x\in E\}\subset R\Rightarrow2^{n^2-n}.$$
$$\text{3.}\quad x\ne y:\ (x,y)\in R\iff(y,x)\in R\Rightarrow2^{\binom n2}.$$

## 15

$$\text{1.}\quad(\mathbf1_A(x),\mathbf1_B(x))\in\{(1,0),(0,1)\}\Rightarrow2^n.$$
$$\text{2.}\quad(\mathbf1_A(x),\mathbf1_B(x))\in\{(0,0),(1,0),(0,1)\}\Rightarrow3^n.$$
$$\text{3.}\quad(\mathbf1_A(x),\mathbf1_B(x))\in\{(1,1),(1,0),(0,1)\}\Rightarrow3^n.$$

## 16

$$A_1\subseteq\cdots\subseteq A_p,\qquad r(x)=\min\{i:x\in A_i\},\quad r(x)=p+1\text{ si }x\notin A_p.$$
$$r:E\to\{1,\ldots,p+1\},\qquad A_i=\{x:r(x)\le i\}.$$
$$\boxed{(p+1)^{|E|}.}$$

## 17

$$\text{1.}\quad4^n.$$
$$\text{2.}\quad u=x+y,\quad v=x-y,\qquad(\Delta u,\Delta v)\in\{(-1,-1),(-1,1),(1,-1),(1,1)\}.$$
$$\Delta u_{\rm total}=\Delta v_{\rm total}=0\iff\text{chaque coordonnée comporte }n\text{ pas }+1\text{ et }n\text{ pas }-1.$$
$$\boxed{\binom{2n}n^2.}$$

## 18

$$N_{p,n}=\#\{f:\{1,\ldots,p\}\twoheadrightarrow\{1,\ldots,n\}\}.$$
$$N_{p,n}=\sum_{J\subseteq\{1,\ldots,n\}}(-1)^{|J|}(n-|J|)^p=\sum_{k=0}^n(-1)^{n-k}\binom nk k^p.$$
$$\text{1.}\quad N_{n,n}=n!,\qquad\text{2.}\quad N_{p,n}=\begin{cases}0&0\le p<n,\\n!&p=n.\end{cases}$$

## 19

$$A_i=\{\sigma:\sigma(i)=i\},\qquad\left|\bigcap_{i\in J}A_i\right|=(n-|J|)!.$$
$$d_n=\sum_{J\subseteq\{1,\ldots,n\}}(-1)^{|J|}(n-|J|)!=\sum_{k=0}^n(-1)^k\binom nk(n-k)!=\boxed{n!\sum_{k=0}^n\frac{(-1)^k}{k!}.}$$

## 20

$$[X^{2n}](1+X)^n(1+X)^{2n}=\sum_{k=0}^n\binom nk\binom{2n}{2n-k}=\boxed{\binom{3n}{2n}=\binom{3n}n.}$$

## 21

$$\text{1.}\quad\max A\in\{p+1,\ldots,n+p+1\}.$$
$$\text{2.}\quad\#\{A:|A|=p+1,\ \max A=m\}=\binom{m-1}p.$$
$$\boxed{\sum_{m=p+1}^{n+p+1}\binom{m-1}p=\sum_{k=0}^n\binom{p+k}p=\binom{n+p+1}{p+1}.}$$

## 22

### 1

$$\#\{(A,B):A\subseteq B\subseteq E,\ |A|=k,\ |B|=p\}=\binom np\binom pk=\boxed{\binom nk\binom{n-k}{p-k}}.$$

### 2

$$\binom nk\binom kj=\binom nj\binom{n-j}{k-j}.$$
$$S(Tx)_n=\sum_{j=0}^n\binom nj x_j\sum_{k=j}^n(-1)^{k-j}\binom{n-j}{k-j}=x_n.$$
$$T(Sx)_n=\sum_{j=0}^n\binom nj x_j\sum_{k=j}^n(-1)^{n-k}\binom{n-j}{k-j}=x_n.$$
$$\boxed{S\circ T=T\circ S=\operatorname{id}_{\mathbb R^{\mathbb N}}.}$$

## 23

$$\#\{(x,A)\in E\times D:x\in A\}=\sum_{x\in E}n=n^2p=\sum_{A\in D}p=p|D|.$$
$$p\ge1\Rightarrow\boxed{|D|=n^2.}$$

## 24

### 1(a)

$$s_1=1,\qquad s_2=2,\qquad s_3=4.$$
$$\text{Première entrée }j:\quad j=n+1\Rightarrow1\text{ liste};\quad1\le j\le n\Rightarrow s_{n+1-j}\text{ listes}.$$
$$\boxed{s_{n+1}=1+\sum_{k=1}^ns_k.}$$
Le $s_0$ imprimé n'est pas défini ; cette formule lui correspond avec $s_0=0$.

### 1(b)

$$n\ge2:\quad s_{n+1}-s_n=s_n,\qquad s_2=2s_1\Rightarrow\boxed{s_n=2^{n-1}.}$$

### 1(c)

$$\underbrace{1\,1\,\cdots\,1}_{n\text{ unités}},\qquad n-1\text{ interstices},\qquad\text{séparer ou réunir à chaque interstice}\Rightarrow2^{n-1}.$$

### 2(a)

$$s_{1,p}=\mathbf1_{p=1},\qquad s_{2,p}=\mathbf1_{p=1}+\mathbf1_{p=2},\qquad s_{n,1}=1,\qquad s_{n,2}=n-1.$$

### 2(b)

$$a_{p+1}=1\Rightarrow(a_1,\ldots,a_p)\text{ de somme }n;$$
$$a_{p+1}\ge2\Rightarrow(a_1,\ldots,a_p,a_{p+1}-1)\text{ de somme }n.$$
$$\boxed{s_{n+1,p+1}=s_{n,p}+s_{n,p+1}.}$$

### 2(c)

$$\binom{n-1}{p-1}+\binom{n-1}p=\binom np,\qquad s_{n,1}=1,\qquad s_{1,p}=\mathbf1_{p=1}.$$
$$\text{Récurrence sur }n\Rightarrow\boxed{s_{n,p}=\binom{n-1}{p-1}.}$$

### 2(d)

$$p\text{ parts non vides}\longleftrightarrow p-1\text{ séparateurs parmi }n-1\text{ interstices}\Rightarrow\binom{n-1}{p-1}.$$

## 25

Entiers distincts.

$$\text{1.}\quad\{1,\ldots,2n\}=\bigsqcup_{j=1}^n\{2j-1,2j\}.$$
$$n+1\text{ éléments},\ n\text{ paires}\Rightarrow\exists j,\quad2j-1,2j\text{ choisis}.$$
$$\text{2.}\quad m=2^{v_2(m)}u(m),\qquad u(m)\in\{1,3,\ldots,2n-1\}.$$
$$\exists a\ne b,\quad u(a)=u(b)\Rightarrow a=2^ru,\quad b=2^su\Rightarrow a\mid b\text{ ou }b\mid a.$$

## 26

$$v\text{ fixé},\quad5\text{ voisins},\quad2\text{ types de lien}\Rightarrow\exists a,b,c\text{ liés à }v\text{ par le même type }T.$$
$$\exists\text{ lien de type }T\text{ parmi }a,b,c\Rightarrow\text{triangle de type }T\text{ avec }v.$$
$$\text{Sinon, }a,b,c\text{ forment un triangle de l'autre type}.$$

## 27

### 1

$$S_0=0,\qquad S_j=\sum_{k=1}^jx_k.$$
$$n+1\text{ sommes},\ n\text{ résidus}\Rightarrow\exists0\le i<j\le n,\quad S_j\equiv S_i\pmod n.$$
$$I=\{i+1,\ldots,j\}\ne\varnothing,\qquad\sum_{k\in I}x_k\in n\mathbb Z.$$

### 2

$$t_j=S_j-\lfloor S_j\rfloor\in[0,1),\qquad t_{\sigma(0)}\le\cdots\le t_{\sigma(n)}.$$
$$\sum_{r=0}^{n-1}(t_{\sigma(r+1)}-t_{\sigma(r)})+(1+t_{\sigma(0)}-t_{\sigma(n)})=1.$$
$$\min\text{ des }n+1\text{ écarts circulaires}\le\frac1{n+1}.$$
$$\exists0\le i<j\le n,\quad\exists N\in\mathbb Z,\quad|S_j-S_i-N|\le\frac1{n+1}.$$
$$\boxed{I=\{i+1,\ldots,j\}.}$$

## 28

### 1

$$[0,1)=\bigsqcup_{r=0}^{n-1}[r/n,(r+1)/n).$$
$$\delta_0,\ldots,\delta_n\Rightarrow\exists0\le i<j\le n,\quad|\delta_j-\delta_i|<1/n.$$
$$q=j-i,\quad p=\lfloor jx\rfloor-\lfloor ix\rfloor\Rightarrow1\le q\le n,\quad\boxed{\left|x-\frac pq\right|<\frac1{nq}.}$$

### 2(a)

$$Q\ge1,\quad x\notin\mathbb Q\Rightarrow\varepsilon_Q=\min_{1\le q\le Q}\operatorname{dist}(qx,\mathbb Z)>0.$$
$$n>1/\varepsilon_Q\Rightarrow|q_nx-p_n|<1/n<\varepsilon_Q\Rightarrow q_n>Q.$$
$$q_n\le n\Rightarrow\left|x-\frac{p_n}{q_n}\right|<\frac1{nq_n}\le\frac1{q_n^2}.$$
$$q_n\to+\infty\Rightarrow\text{une infinité de couples}.$$

### 2(b)

$$|p_n|\ge|x|q_n-|p_n-q_nx|>|x|q_n-1/q_n\to+\infty.$$

## 29

### 1

$$m=\lfloor kp\rfloor=\lfloor\ell q\rfloor\Rightarrow m<kp<m+1,\quad m<\ell q<m+1.$$
$$m\left(\frac1p+\frac1q\right)<k+\ell<(m+1)\left(\frac1p+\frac1q\right)\Rightarrow m<k+\ell<m+1,\quad\bot.$$

### 2

$$\lfloor kp\rfloor\le n\iff kp<n+1\iff k<\frac{n+1}p\Rightarrow|P\cap\{1,\ldots,n\}|=\left\lfloor\frac{n+1}p\right\rfloor.$$
$$a=\frac{n+1}p\notin\mathbb Z,\quad\frac{n+1}q=n+1-a\Rightarrow\lfloor a\rfloor+\lfloor n+1-a\rfloor=n.$$
$$|(P\cup Q)\cap\{1,\ldots,n\}|=n.$$

### 3

$$\forall n\ge1,\quad(P\cup Q)\cap\{1,\ldots,n\}=\{1,\ldots,n\}\Rightarrow\boxed{\mathbb N^*=P\sqcup Q.}$$
