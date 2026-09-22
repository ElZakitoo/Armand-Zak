# corrigé zakito

[Énoncé](https://www.bourrigan.fr/data/td01-calcul.pdf)

## Autocorrection A

(i) $\sqrt{xy}$ est défini pour $xy\ge0$; $\sqrt x\sqrt y$ exige $x,y\ge0$. Là où les deux expressions sont définies elles sont égales; le second domaine est inclus dans le premier.

(ii) $\ln(xy)$ exige $xy>0$; $\ln x+\ln y$ exige $x>0$ et $y>0$. Sur leur domaine commun, les deux valent la même chose. Si $x,y<0$, seule la première expression existe.

(iii) $x^2/x$ est défini pour $x\ne0$ et vaut alors $x$.

(iv) $xy/(x+y)$ exige $x+y\ne0$. L’expression $1/(1/x+1/y)$ exige $x,y\ne0$ et $1/x+1/y\ne0$, soit $x,y\ne0$ et $x+y\ne0$. Sur ce domaine commun, elle vaut $xy/(x+y)$.

(v) $x$ et $\sqrt{x^2}=|x|$ sont définis pour tout réel; ils sont égaux exactement lorsque $x\ge0$.

(vi) $\sqrt{x}$ exige $x\ge0$ et $(\sqrt{x})^2=x$ sur tout ce domaine.

## Exercice 1

1. Pour $x\ge0$, $\sqrt x$ est l’unique réel $r\ge0$ tel que $r^2=x$. La quantité n’est pas définie dans $\mathbb R$ si $x<0$.
2. $\sqrt{\sqrt{\sqrt{256}}}=\sqrt{\sqrt{16}}=\sqrt4=2$.
3. $(x-y)(x+y)=x^2-y^2=0$, donc $x=y$ ou $x=-y$, autrement dit $|x|=|y|$.
4. $7+4\sqrt3=(2+\sqrt3)^2$ et $2+\sqrt3>0$, donc $\sqrt{7+4\sqrt3}=2+\sqrt3$.
5. Multiplier par le conjugué donne
   $$\frac1{a+b\sqrt5}=\frac{a-b\sqrt5}{a^2-5b^2}.$$
   Le dénominateur est rationnel et non nul par l’hypothèse de l’énoncé; ainsi $x=a/(a^2-5b^2)$ et $y=-b/(a^2-5b^2)$ conviennent.
6. Pour $x\ge1$,
   $$\sqrt{x+1}-\sqrt{x-1}=\frac2{\sqrt{x+1}+\sqrt{x-1}}\longrightarrow0.$$

## Exercice 2

1. (i) $x^2+18x+81=(x+9)^2$. (ii) $x^4+4x^3-12x^2=x^2(x+6)(x-2)$. (iii) $(x^2+1)^2-4x^2=(x^2-2x+1)(x^2+2x+1)=(x-1)^2(x+1)^2$.

2. (i) La fraction composée exige $x\ne0$, $y\ne0$ et $x\ne\pm3$. Elle se simplifie en
   $$\frac{(x^2-x-6)/(2xy)}{(x^2-9)/(2x^2y)}=\frac{x(x+2)}{x+3}.$$
   Son signe est celui de $x(x+2)/(x+3)$: négatif sur $(-\infty,-3)$ et $(-2,0)$, positif sur $(-3,-2)$ et $(0,+\infty)$; elle s’annule en $x=-2$.
   (ii) Pour $x\ne0$ et $x^4\ne1$,
   $$\frac{x^2+x^{-2}-2}{x^2-x^{-2}}=\frac{(x-x^{-1})^2}{(x-x^{-1})(x+x^{-1})}=\frac{x^2-1}{x^2+1}.$$
   Son signe est positif si $|x|>1$, négatif si $0<|x|<1$.
   (iii) Pour tout réel $x$,
   $$\frac1{2x^2-2x+1}-\frac1{2x^2+2x+1}=\frac{4x}{(2x^2-2x+1)(2x^2+2x+1)}.$$
   Les deux facteurs du dénominateur sont strictement positifs ($2(x\mp\tfrac12)^2+\tfrac12$); le signe est celui de $x$.

3. (a) $91=10^2-3^2=(10-3)(10+3)=7\cdot13$, donc n’est pas premier. (b) $xy+\alpha x+\beta y+\alpha\beta=(x+\beta)(y+\alpha)$. (c) Écrire
   $$3x^2y^2+y^2=27x^2+100\iff(3x^2+1)(y^2-9)=91.$$
   Pour $x,y\in\mathbb N$, si $y\le3$, le membre de gauche est non positif; donc $y\ge4$. Les diviseurs positifs de 91 sont $1,7,13,91$. Le choix $3x^2+1=1$ donne $(x,y)=(0,10)$; le choix $3x^2+1=13$ donne $(2,4)$. Les autres diviseurs ne donnent pas de carré pour $x$. Les solutions sont donc $(0,10)$ et $(2,4)$.

## Exercice 3

Les domaines sont donnés par la non-annulation de chaque dénominateur.

(i) $1/60+1/48= (4+5)/240=3/80$.

(ii) $1/x-1/(x+1)=1/[x(x+1)]$, pour $x\ne0,-1$.

(iii) $\frac{2}{(x+1)^2(x+3)}-\frac{1}{(x+1)(x+2)(x+3)}$; pour $x\ne-1,-2,-3$,
$$\frac{2(x+2)-(x+1)}{(x+1)^2(x+2)(x+3)}=\frac{1}{(x+1)^2(x+2)}.$$

(iv) $1/(x^2-y^2)+1/(x^2+y^2-2xy)$. Les dénominateurs sont $(x-y)(x+y)$ et $(x-y)^2$; pour $x\ne y$ et $x\ne-y$,
$$\frac{(x-y)+(x+y)}{(x-y)^2(x+y)}=\frac{2x}{(x-y)^2(x+y)}.$$

(v) Pour $x\ne1,1/2$, le numérateur de la fraction composée est
$$\frac{x+1}{x-1}-\frac{2x+1}{2x-1}=\frac{2x}{(x-1)(2x-1)},$$
et son dénominateur vaut
$$\frac{2x+1}{x-1}-\frac{x+1}{2x-1}=\frac{3x^2}{(x-1)(2x-1)}.$$
Il faut aussi que ce dénominateur soit non nul, donc $x\ne0$. L’expression initiale vaut alors $2/(3x)$.

## Autocorrection B

On utilise $u\le v\iff v-u\ge0$, la transitivité, et la positivité des sommes et produits de réels positifs.

(i) $(b+d)-(a+c)=(b-a)+(d-c)\ge0$. (ii) la même somme est strictement positive puisque $d-c>0$. (iii) $-a,b\ge0$, donc $(-a)b\ge0$, soit $ab\le0$. (iv) $(-a)(-b)\ge0$, donc $ab\ge0$. (v) $a,b>0$ impliquent $ab>0$: leur produit est non négatif et ne peut être nul puisque les facteurs sont non nuls. (vi) $-a,b>0$, donc $ab<0$. (vii) $-a,-b>0$, donc $ab>0$. (viii) selon le signe de $a$, soit $a^2\ge0$, soit $(-a)^2\ge0$; un carré est donc positif. (ix) $\lambda(b-a)\ge0$. (x) $\lambda(b-a)\le0$. (xi) produit de deux réels strictement positifs: $\lambda(b-a)>0$. (xii) $\lambda(b-a)<0$. (xiii) $bd-ac=(b-a)d+a(d-c)\ge0$. (xiv) cette décomposition est strictement positive car $d>0$, $b-a>0$, $a>0$, $d-c>0$. (xv) Si $1/a\le0$, le produit par $a>0$ donnerait $1\le0$, impossible; ainsi $1/a>0$. (xvi) $1/a-1/b=(b-a)/(ab)\ge0$. (xvii) la même différence est strictement positive.

## Exercice 4

Non: pour $a=-2$ et $b=-1/2$, on a $a/b=4\ge1$, tandis que $(a+1)/(b+1)=-2<1$.

## Exercice 5

1. Des bornes $m_1\le x\le M_1$, $m_2\le y\le M_2$:
(i) si $\lambda\ge0$, $\lambda m_2\le\lambda y\le\lambda M_2$, et l’ordre s’inverse si $\lambda<0$ (égalité $0$ si $\lambda=0$).
(ii) $m_1+m_2\le x+y\le M_1+M_2$.
(iii) $m_1-M_2\le x-y\le M_1-m_2$.
(iv) $|x|\le\max(|m_1|,|M_1|)$; la borne inférieure est $0$ si $0\in[m_1,M_1]$, sinon $\min(|m_1|,|M_1|)$.
Sous $0<m_i$: (v) $\ln m_1\le\ln x\le\ln M_1$; (vi) $1/M_2\le1/y\le1/m_2$; (vii) $m_1m_2\le xy\le M_1M_2$; (viii) $m_1/M_2\le x/y\le M_1/m_2$.

2. $1\le x\le4$ donne $1\le x^2\le16$, donc $3\le x^2+x+1\le21$ et $5\le3x+2\le14$. Les quantités étant positives, $3/14\le (x^2+x+1)/(3x+2)\le21/5$.

3. (a) $-1\le\sin x,\cos x\le1$, donc $-2\le\sin x+\cos x\le2$. (b) $\sin x+\cos x=\sqrt2\cos(x-\pi/4)$; son image est $[-\sqrt2,\sqrt2]$.

4. (a) Pour $x\in[0,2]$, $x\ne1$, la rationalisation fournit
$$\frac{x^2-3x+2}{\sqrt x+x-2}=\frac{(\sqrt x-1)(\sqrt x+1)(x-2)}{(\sqrt x-1)(\sqrt x+2)}=\frac{(\sqrt x+1)(x-2)}{\sqrt x+2}.$$
(b) Cette expression a module inférieur ou égal à $2$: $|x-2|\le2$ et $0\le(\sqrt x+1)/(\sqrt x+2)\le1$, d’où l’expression est même entre $-2$ et $2$; en particulier elle est $\le2$.

## Exercice 6

$$1-\frac{a+b}{1+ab}=\frac{(1-a)(1-b)}{1+ab}>0,\qquad 1+\frac{a+b}{1+ab}=\frac{(1+a)(1+b)}{1+ab}>0.$$
En effet $1\pm a,1\pm b>0$ et $1+ab>0$ (si $ab<0$, $1+ab>1-|a|>0$; sinon c’est immédiat). Ainsi le quotient est strictement entre $-1$ et $1$.

## Autocorrection C

1. $(a-b)^2\ge0$ donne $ab\le(a^2+b^2)/2$, avec égalité exactement si $a=b$.
2. Pour $a,b\ge0$, $(\sqrt a-\sqrt b)^2\ge0$ donne $2\sqrt{ab}\le a+b$, avec égalité exactement si $a=b$.

## Exercice 7

1. (a) $(\sqrt x-1/\sqrt x)^2\ge0$ donne $x+1/x\ge2$. (b) Pour chaque $x>0$, $1/x\ge2-x$. En sommant sur $x,y,z$ et en utilisant $x+y+z=s$, on obtient $1/x+1/y+1/z\ge6-s$.

2. (a) $(x+y)/2\ge\sqrt{xy}$, etc.; en multipliant les trois inégalités, $(x+y)(y+z)(z+x)\ge8xyz$. (b) L’identité
$$(x+y)(y+z)(z+x)=s(xy+yz+zx)-xyz$$
donne, après division par $xyz$, $s(1/x+1/y+1/z)-1\ge8$, donc $1/x+1/y+1/z\ge9/s$.

3. $6-s$ et $9/s$ sont comparées par $9/s-(6-s)=(s-3)^2/s\ge0$; la borne $9/s$ est toujours la meilleure.

## Exercice 8+

1. Par AM-GM, $x^4+y^2\ge2\sqrt{x^4y^2}=2x^2y$, donc $x/(x^4+y^2)\le1/(2xy)$.
2. En appliquant le résultat précédent à $(x,y)$ puis $(y,x)$ et en sommant,
$$\frac{x}{x^4+y^2}+\frac{y}{x^2+y^4}\le\frac1{2xy}+\frac1{2xy}=\frac1{xy}.$$

## Exercice 9++

1. $x/y+y/x-2=(x-y)^2/(xy)\ge0$.
2. Par Cauchy-Schwarz,
$$\sum_{cyc}\frac a{b+c}=\sum_{cyc}\frac{a^2}{a(b+c)}\ge\frac{(a+b+c)^2}{2(ab+bc+ca)}\ge\frac32,$$
car $(a+b+c)^2\ge3(ab+bc+ca)$.

## Autocorrection D

1. $|a+b|^2=a^2+2ab+b^2\le a^2+2|a||b|+b^2=(|a|+|b|)^2$; les deux membres étant positifs, on prend les racines.
2. L’égalité équivaut à $ab=|a||b|$, soit $ab\ge0$, c’est-à-dire que $a,b$ sont de même signe (zéro compris).
3. L’équation est $|x|+|x-1|=1$. Par inégalité triangulaire, $1=|x-(x-1)|\le|x|+|x-1|$, avec égalité exactement lorsque $x$ et $1-x$ sont de même signe, soit $x\in[0,1]$.

## Autocorrection E

1. (a) $\min(a,b)+\max(a,b)=a+b$. (b) Si $a\ge b$, le membre proposé vaut $(a+b+a-b)/2=a$; le cas $b\ge a$ est symétrique. (c) $\min(a,b)=(a+b-|a-b|)/2$, vérifié de même dans les deux cas.

2. (i) $\exists i, x_i\le\alpha$. (ii) $\forall i, x_i\ge\alpha$. (iii) $\forall i, x_i\le\alpha$. (iv) $\exists i, x_i\ge\alpha$.

## Autocorrection F

(i) $[-6,6]$. (ii) $[-2,6]$. (iii) $\varnothing$. (iv) $x^2-4=\pm2$: $\{-\sqrt6,-\sqrt2,\sqrt2,\sqrt6\}$. (v) $x^2-8x+11=\pm4$, soit $x\in\{1,7,3,5\}$. (vi) $|x^2-8x+11|<4$ équivaut à $1<(x-4)^2<9$; l’ensemble est $(1,3)\cup(5,7)$. (vii) $|x+1|=|2x-3|\iff x+1=2x-3$ ou $x+1=-2x+3$, donc $x\in\{4,2/3\}$. (viii) $|1-2x|=x+1$ impose $x\ge-1$; le cas $x\le1/2$ donne $x=0$, le cas $x\ge1/2$ donne $x=2$. Solutions: $\{0,2\}$. (ix) Le cas $x^2-3x-3\ge0$ donne $x^2-4x-5=0$, donc $x=-1$ ou $5$; ces deux valeurs conviennent. Le cas $x^2-3x-3<0$ donne $x^2-2x-1=0$, donc $x=1\pm\sqrt2$, qui conviennent aussi. (x) La condition est $x+2>0$ et $-(x+2)<x^2+5x+3<x+2$. Cela équivaut à $(x+1)(x+5)>0$ et $(x+2-\sqrt3)(x+2+\sqrt3)<0$; l’intersection est $(-1,-2+\sqrt3)$. (xi) $2-x<|x+1|$: pour $x\ge-1$, cela donne $x>1/2$; pour $x<-1$, elle devient $2-x<-x-1$, impossible. Donc $(1/2,+\infty)$. (xii) somme des distances à $0$ et $-1$ égale $2$: sur $[-1,0]$ elle vaut $1$; à l’extérieur elle vaut $-2x-1$ si $x<-1$ ou $2x+1$ si $x>0$. Solutions $x=-3/2$ ou $x=1/2$. (xiii) somme des distances aux points $2$ et $7$ est au moins $5$, donc ne peut être $\le3$: $\varnothing$. (xiv) les zéros sont $-7/4$ (multiplicité 20, signe inchangé) et $-4$ (multiplicité 1); le produit est négatif exactement pour $x<-4$.

## Exercice 10

$\sin x\in[-1,1]$ et $\cos y\in[-1,1]$, donc leur produit appartient à $[-1,1]$, en particulier il est supérieur ou égal à $-1$.

## Exercice 11

1. (a) $|a|=|(a-b)+b|\le|a-b|+|b|$. (b) En échangeant $a,b$, on obtient $|a-b|\ge|b|-|a|$; les deux donnent $|a-b|\ge\big||a|-|b|\big|$.
2. $2|a|=|(a+b)+(a-b)|\le|a+b|+|a-b|$ et $2|b|=|(a+b)-(a-b)|\le|a+b|+|a-b|$. En additionnant puis divisant par $2$, on obtient l’inégalité voulue.

## Exercice 12

1. Poser $u=a-1$, $v=b-1$. Alors $ab-1=u+v+uv$ et $a+b=u+v+2$. Par triangulaire,
$$1+|ab-1|\le1+|u|+|v|+|uv|=(1+|u|)(1+|v|).$$
2. Posons $u=|a|$ et $v=|b|$. La fonction $t\mapsto t/(1+t)$ est croissante sur $[0,+\infty[$, donc
$$\frac{|a+b|}{1+|a+b|}\le\frac{u+v}{1+u+v}\le\frac{u}{1+u}+\frac{v}{1+v}.$$
La seconde inégalité résulte de $\frac{u}{1+u}+\frac{v}{1+v}-\frac{u+v}{1+u+v}=\frac{uv(2+u+v)}{(1+u)(1+v)(1+u+v)}\ge0$.

## Exercice 13+

L’expression est inchangée par permutation des variables et par changement simultané de leurs signes. S’il n’y a pas de signes opposés, elle vaut $0$. Sinon, après permutation et éventuellement changement de signe, prenons $a,b\ge0$ et $c=-t\le0$. Elle devient
$$t-|a-t|-|b-t|+|a+b-t|.$$
Supposons $a\ge b$. Si $t\le b$, cette quantité vaut $2t$; si $b\le t\le a$, elle vaut $2b$; si $t\ge a$, elle vaut $a+b-t+|a+b-t|\ge0$.

## Exercice 14+

1. La moyenne des deux nombres $a^2+b$ et $b^2+a$ vaut
$$\frac{a^2+b^2+a+b}{2}=\frac{a^2+a}{2}+\frac{b^2+b}{2}\ge-\frac14,$$
car $t^2+t=(t+1/2)^2-1/4$. Leur maximum est au moins leur moyenne, donc il est supérieur ou égal à $-1/4$.
2. L’assertion, telle qu’écrite, est fausse: pour $a=b=c=0$, le maximum vaut $0<1/4$ (et pour $a=b=c=2/3$, il vaut $2/9<1/4$).

## Exercice 15

$A=(0,0,0)$, $B=(a,a,a)$, $a>0$.

$$F_- = \{x=0\}\cup\{y=0\}\cup\{z=0\},\qquad F_+=\{x=a\}\cup\{y=a\}\cup\{z=a\}$$
Sur la surface du cube, tout chemin de $A$ à $B$ rencontre $F_-\cap F_+$.
$$P\in F_-\cap F_+\Rightarrow P=(0,a,t),\quad0\le t\le a\quad\text{à permutation des coordonnées près}.$$
$$L\ge AP+PB=\sqrt{a^2+t^2}+\sqrt{a^2+(a-t)^2}\ge\sqrt{(2a)^2+(t+a-t)^2}=a\sqrt5.$$
$$\text{Égalité}\iff t=a/2\text{ et le chemin suit les segments }[A,P]\text{ et }[P,B].$$
$$P\in\{(0,a,a/2),(a,0,a/2),(0,a/2,a),(a,a/2,0),(a/2,0,a),(a/2,a,0)\}.$$
$$\boxed{6\text{ chemins minimaux, de longueur }a\sqrt5.}$$

## Exercice 16

$$\sum_{k=1}^{99}\frac1{k(k+1)}=\sum_{k=1}^{99}\left(\frac1k-\frac1{k+1}\right)=1-\frac1{100}=0{,}99.$$

## Exercice 17+

La première page du premier volume et la dernière page du second se trouvent sur les faces qui se font face entre les deux livres. Le ver ne traverse donc que les deux couvertures intérieures, soit $2+2=4$ mm.

## Exercice 18+

Si l’angle droit est en $A$, alors $AB^2+AC^2=BC^2=100$. La hauteur sur l’hypoténuse vaut $h=AB\,AC/BC=6$, donc $AB\,AC=60$. Or $(AB^2+AC^2)\ge2AB\,AC=120$, contradiction avec $100$. Aucun tel triangle n’existe; l’aire $30$ vient d’une configuration impossible. Les données minimales de $BC$ pour une hauteur $6$ seraient $BC\ge12$.
