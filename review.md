# $\textbf{Review}$

## $1.$ $\textbf{Group}$

规定 $G$ 为群，$H$ 为其子群，$N$ 为其正规子群，即 $H\leqslant G,\ N\vartriangleleft G$

### $1.1$ $\textbf{Proposition}$

$\textbf{Prop.1}$ 群必定满足消去律. 事实上，若有 $a,\ b,\ c\in G,\ ab = ac$，则 $a^{-1}ab = a^{-1}ac$，所以 $b = c$

$\textbf{Prop.2}$ 加群 $\mathbb{Z}$ 的每个子群都是循环群，并且有 $H = \left\langle 0\right\rangle,\ H = \left\langle m\right\rangle = m\mathbb{Z}$，前者为有限群，后者为无限群

$\textbf{Prop.3}$ 陪集 $aH$ 与子群 $H$ 的元素个数相同

$\textbf{Prop.4}$ 循环群同构于整数加群，无限循环群同构于 $\mathbb{Z}$，$m$ 阶循环群同构于 $\mathbb{Z}/m\mathbb{Z}$

$\textbf{Prop.5}$ 循环群的子群还是循环群

### $1.2$ $\textbf{Theorem}$

$\textbf{Desc.}\ H\leqslant G\Leftrightarrow \forall a,\ b\in H,\ ab^{-1}\in H$ （子群判定定理）

$\textbf{Desc.}\ N\vartriangleleft G\Leftrightarrow \forall a\in G,\ aNa^{-1}\subset N$ （正规子群判定定理）

$\textbf{Desc.}\ a,\ b\in G,\ aH = bH\Leftrightarrow b^{-1}a\in H$ （判定陪集相等）

$\textbf{Desc.}$ 子群的阶是群本身阶的因数，即 $|H|\mid|G|$ （拉格朗日定理）

$\textbf{Desc.}$ 考虑==满同态映射== $f: G\rightarrow G'$，有 $G/kerf\cong G'$ （同态基本定理）

### $1.3$ $\textbf{Exercise}$

$\textbf{Prob.1}$ 考虑同态映射 $f: G\rightarrow G'$，$kerf = \left\{a\mid a\in G,\ f(a) = e'\right\}$，其中 $e'$ 是 $G'$ 单位元，证明 $kerf$ 是 $G$ 的正规子群

$\textbf{Proof}$ 先证明 $kerf\leqslant G$，再证明 $kerf\vartriangleleft G$

- 任取 $a,\ b\in kerf$，有 $f(a) = f(b) = f(b^{-1}) = e'$，所以 $f(ab^{-1}) = f(a)f(b)^{-1} = e'$，所以 $kerf$ 是子群
- 任取 $a\in G,\ b\in kerf$，有 $f(aba^{-1}) = f(a)f(b)f(a)^{-1} = f(a)f(a)^{-1} = e'$，所以 $aba^{-1}\in kerf$，所以 $kerf$ 是正规子群

$\textbf{Prob.2}$ 设 $a\in G$，证明：映射 $\sigma: x\mapsto axa^{-1}$ 是 $G$ 到自身的自同构

$\textbf{Proof}$ 分别证明单射，满射和自同态

- $\forall x,\ y\in G,\ \sigma(x) = \sigma(y)$，则 $axa^{-1} = aya^{-1}$，易得 $x = y$，单射得证
- $\forall y\in G,\ \exists x = a^{-1}ya,\ s.t.\ \sigma(x) = a(a^{-1}ya)a^{-1} = y$，满射得证
- 设 $\sigma: G\rightarrow G'$，首先证明映射是同态，其次证明 $G = G'$
  - $\forall x,\ y\in G,\ \sigma(xy) = a(xy)a^{-1} = axa^{-1}\cdot aya^{-1} = \sigma(x)\cdot \sigma(y)$，同态得证
  - 首先，$\forall x\in G,\ \sigma(x) = axa^{-1}\in G'$，取 $x = a,\ a^{-1}$，得到 $a,\ a^{-1}\in G'$，所以 $a(axa^{-1})a^{-1} = x\in G'$，所以 $G\subset G'$，反过来，$\forall y\in G',\ y = axa^{-1}\in G$，所以 $G'\subset G$，所以 $G = G'$

综上得到，$\sigma$ 是 $G$ 到自身的同构

$\textbf{Prob.3}$ 素数阶群一定是循环群

$\textbf{Proof}$ 设 $G$ 为素数阶群，设 $a\in G$，设 $\left \langle a \right \rangle$ 为 $a$ 生成的循环子群，根据拉格朗日定理，有 $|\left \langle a \right \rangle|\mid |G|$，而 $|G|$ 为素数，所以 $|\left \langle a \right \rangle| = |G|$ 或者 $|\left \langle a \right \rangle| = 1$，前者对应 $G$ 本身，后者对应单位元生成的循环子群 $\left \langle a \right \rangle = \left \{ e \right \}$，因此素数阶群一定是循环群

$\textbf{Prob.4}$ 设同态映射 $f: G\rightarrow G'$，若 $a,\ b\in G,\ f(a) = f(b)$，证明 $akerf = bkerf$

$\textbf{Proof}$ 由 $f(a) = f(b)$，得到 $f(b)^{-1}f(a) = f(b^{-1}a) = e'$，所以 $b^{-1}a\in kerf$，所以 $akerf = bkerf$

$\textbf{Prob.5}$ 列出循环加群 $\left\langle Z_{8},\ +\right\rangle$ 和循环乘群 $\left\langle Z_{15}^{*},\ \cdot\right\rangle$ 的所有非平凡循环子群

$\textbf{Sol.}$ 由拉格朗日定理知道，$\left\langle Z_{8},\ +\right\rangle$ 的所有非平凡循环子群分别为 $4$ 阶和 $2$ 阶. $4$ 阶循环子群为 $\left\{0,\ 2,\ 4,\ 6\right\}$，$2$ 阶为 $\left\{0,\ 4\right\}$. 同理，$\left\langle Z_{15}^{*},\ \cdot\right\rangle$ 的所有非平凡循环子群分别为 $2$ 阶和 $4$ 阶，分别为 $\left\{1,\ 4\right\},\ \left\{1,\ 2,\ 4,\ 8\right\}$

$\textbf{Prob.6}$ 证明模 $m$ 的所有剩余类构成的集合关于剩余类的加法构成 $m$ 阶循环群

$\textbf{Proof}$ 设循环群 $G = \left\langle a\right\rangle = \left\{g^n\mid n\in \mathbb{Z}\right\}$，构造映射 $f: \mathbb{Z}\rightarrow G,\ n\mapsto a^n$，因为 $f(x + y) = a^{x + y} = a^xb^y = f(x)f(y)$，且对于 $\forall a^n\in G,\ \exists n\in \mathbb{Z}$，所以 $f$ 是满同态映射，根据同态基本定理，$\mathbb{Z}/kerf\cong G$，且 $kerf = \left\{0\right\}$ 或者 $kerf = m\mathbb{Z}$，前者对应无限循环群，后者对应 $m$ 阶循环群，所以 $\mathbb{Z}/m\mathbb{Z}\cong G$

$\textbf{Prob.7}$ 证明 $\mathbb{Z}/m\mathbb{Z}\cong \mathbb{Z_{m}}$

$\textbf{Proof}$ 构造映射 $f: \mathbb{Z}\rightarrow \mathbb{Z_{m}},\ n\mapsto n\ mod\ m$，由 $f(ab) = (ab)\ mod\ m = f(a)f(b)$，且容易证明 $f$ 是满射，所以 $f$ 是满同态映射，又 $kerf = m\mathbb{Z}$，所以根据同态基本定理，得到 $\mathbb{Z}/m\mathbb{Z}\cong \mathbb{Z_{m}}$

$\textbf{Prob.8}$ 设 $p$ 是奇素数，证明乘法群 $F_{p}^{*} = \mathbb{Z}/p\mathbb{Z}\backslash \left\{0\right\}$ 关于乘法 $a\cdot b = a\cdot b\ mod\ p$ 构成循环群，且与加群 $\mathbb{Z}/(p - 1)\mathbb{Z}$ 同构

$\textbf{Proof}$ 因为 $p$ 是素数，所以模 $p$ 的原根存在，设为 $g$，于是 $\left\{g^0,\ g^1,\ g^2,\ ...,\ g^{\phi(p) - 1}\right\}$ 组成模 $p$ 的简化剩余系，所以 $F_{p}^{*}$ 是一个 $p - 1$ 阶的循环乘法群，故而与 $\mathbb{Z}/(p - 1)\mathbb{Z}$ 同构

$\textbf{Prob.9}$ 设 $p$ 是奇素数，证明 $\mathbb{Z}/p^2\mathbb{Z}$ 中的可逆元对于模 $p^2$ 乘法构成循环群，并且求其阶

$\textbf{Proof}$ 设 $g$ 是模 $p$ 的原根，由于 $p$ 是奇素数，因此 $g$ 也是模 $p^2$ 原根，因此 $\mathbb{Z_{p^2}}^{*}$ 可以由 $g$ 生成，所以 $\mathbb{Z_{p^2}}^{*}$ 是一个循环群，阶数为 $\phi(p^2) = p(p - 1)$，根据同构，$\mathbb{Z}/p^2\mathbb{Z}$ 中的可逆元对于模 $p^2$ 乘法构成循环群，阶数为 $p(p - 1)$

$\textbf{Prob.10}$ 设 $G$ 是群，证明 $(xy)^{-1} = y^{-1}x^{-1}$

$\textbf{Proof}$ $(xy)\cdot (xy)^{-1} = e = xy\cdot y^{-1}{x}^{-1}$，所以 $(xy)^{-1} = y^{-1}x^{-1}$

$\textbf{Prob.11}$ 设 $G$ 是群，$\forall x\in G,\ x^2 = e$，证明 $G$ 可交换

$\textbf{Proof}$ 由 $x^2 = e$，得到 $x^{-1}x^2 = x^{-1}e$，即 $x = x^{-1}$. 由 $(xy)^2 = e$，得到 $xy = (xy)^{-1} = y^{-1}x^{-1} = yx$，所以 $G$ 可交换

## $2.\ \textbf{Ring and Field}$

设环为 $R$，域为 $K$

### $2.1\ \textbf{Proposition}$

$\textbf{Prop.1}$ $R$ 为整环满足三个条件：==交换环，无零因子，有乘法单位元==

$\textbf{Prop.2}$ $K$ 为域满足三个条件：==交换环，有乘法单位元，每个非零元都是可逆元.== 进而推出，==域一定无零因子，以及域是整环==

$\textbf{Prop.3}$ 主理想环是每个理想均为主理想 $\textbf{(Principal Ideal)}$ 的环，常见的有整环 $\mathbb{Z}$，以及域 $K$ 上的多项式环 $K[x]$

$\textbf{Prop.4}$ 环 $R$ 首先是个交换加群，其次是个乘法半群（满足乘法结合律），同时满足乘法分配律

$\textbf{Prop.5}$ 域 $K$ 对加法和乘法均构成交换群

$\textbf{Prop.6}$ 环 $R$ 中的可逆元无零因子. 事实上，假设非零元 $a,\ b\in R,\ ab = 0$，则 $abb^{-1} = a = 0$，矛盾.

$\textbf{Prop.7}$ 环的特征 $p$ 指的是环中所有元素的共同阶数，即 $\forall a\in R,\ pa = 0$，若不存在 $p$，特征为 $0$

### $2.2\ \textbf{Theorem}$

### $2.3\ \textbf{Exercise}$

$\textbf{Prob.1}$ 证明整环 $\mathbb{Z}$ 是主理想环

$\textbf{Proof}$ 只需要证明 $\mathbb{Z}$ 的每一个理想 $I$ 都是 $(a)$ 的形式，即证明 $I = (a)$

- 先证明 $I\subset (a)$. 对于非零理想 $I$，$I$ 保有子环性质，若 $b\in I$，则 $0,\ -b\in I$，所以 $I$ 中存在正整数. 设 $a$ 是 $I$ 中最小正整数，那么 $\forall b\in I,\ b = qa + r,\ 0\leq r < a,\ q\in \mathbb{Z}$，根据封闭性有 $r = b + (-q)a\in I$，由于 $a$ 的最小性，$r$ 只能为 $0$，所以 $b = qa\in (a)$，所以 $I\subset (a)$
- 再证明 $(a)\subset I$. 根据 $I$ 的性质, $\forall k\in \mathbb{Z},\ ka\in I,$ 所以 $(a)\subset I$

所以 $I = (a)$，即 $\mathbb{Z}$ 是主理想环

$\textbf{Prob.2}$ 计算环 $\mathbb{Z_{8}}$ 的所有零因子

$\textbf{Sol.}$ 计算环 $\mathbb{Z_{8}}$ 中所有不可逆元，即 $2,\ 4,\ 6$

## $3.$ $\textbf{Polynomial Ring}$

记整环为 $R$，有限域为 $F_{p}$，环上多项式集合为 $R[x]$，域上多项式集合为 $F_{p}[x]$，关于多项式加法和多项式乘法，前者构成整环，后者构成主理想环

### $3.1\ \textbf{Proposition}$

$\textbf{Prop.1}$ $F_{p}[x]$ 上的不可约多项式 $f(x)$ 指的是，除了平凡因式 $1$ 和 $f(x)$ 外，不存在非常数因式的多项式

$\textbf{Prop.2}$ $F_{p}[x]$ 上的本原多项式 $f(x)$ 指的是满足 $ord_{p}(f(x)) = p^n - 1$ 的多项式，其中指数 $ord_{p}(f(x))$ 指的是使得 $x^e\equiv 1\ (mod\ f(x))$ 的最小整数 $e$

### $3.2\ \textbf{Theorem}$

$\textbf{Desc.}$ 证明 $f(x) = \sum\limits_{i = 0}^{n}a_{i}x^i$ 是 $F_{p}[x]$ 上的不可约多项式，等价于验证，对于 $F_{p}[x]$ 上所有次数不超过 $\frac{1}{2}degf$ 的不可约多项式 $p(x)$，都有 $p(x)\nmid f(x)$ （不可约多项式判定定理）

$\textbf{Desc.}$ 证明 $f(x) = \sum\limits_{i = 0}^{n}a_{i}x^i$ 是 $F_{p}[x]$ 上的本原多项式，等价于验证，$x^{p^{n} - 1}\equiv 1\ (mod\ f(x))$，并且对于 $p^n - 1$ 的所有因数 $d$，都有 $x^{\frac{p^{n} - 1}{d}}\not\equiv 1\ (mod\ f(x))$ （本原多项式判断定定理）

### $3.3\ \textbf{Exercise}$

$\textbf{Prob.1}$ 证明 $f(x) = x^4 + x + 1$ 是 $F_{2}[x]$ 上的不可约多项式

$\textbf{Proof}$ 找到 $F_{2}[x]$ 上所有次数不超过 $2$ 的不可约多项式，即 $x,\ x + 1,\ x^2 + x + 1$，依次对 $f(x)$ 做带余除法，得到 $f(x) = (x^3 + 1)\cdot x + 1,\ f(x) = (x^3 + x^2 +x)\cdot (x + 1) + 1,\ f(x) = (x^2 + x)\cdot (x^2 + x + 1) + 1$，所以 $x\nmid f(x),\ x + 1\nmid f(x),\ x^2 + x + 1\nmid f(x)$，所以 $f(x)$ 是 $F_{2}[x]$ 上的不可约多项式

$\textbf{Prob.2}$ 证明 $f(x) = x^8 + x^4 + x^3 + x^2 + 1$ 是 $F_{2}[x]$ 上的本原多项式

$\textbf{Proof}$ $n = 8$，则 $p^n - 1= 2 ^ 8 - 1 = 255 = 3\cdot 5\cdot 17$，只需要验证 $x^{255}\equiv 1,\ x^{15}\not\equiv 1,\ x^{51}\not\equiv 1,\ x^{85}\not\equiv 1\ (mod\ f(x))$，验证成立，所以 $f(x)$ 是 $F_{2}[x]$ 上的本原多项式

## $4.$ 椭圆曲线