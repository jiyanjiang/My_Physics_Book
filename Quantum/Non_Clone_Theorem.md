# 量子不可克隆原理

量子不可克隆原理说的是：

不存在一个物理过程（幺正变换：U）使得：

$$ U \left| \psi \right\rangle_A \left| X \right\rangle_B  \to \left| \psi \right\rangle_A \left| \psi \right\rangle_B$$

上式的意思是，通过物理过程U, 使得$\psi$被从A复制到了B，初始的时候B处的波函数为任意波函数X。

证明的思路是反证法，假如这样的物理过程存在，会如何？

首先通过U可把$\psi$由A复制B

$$ U \left| \psi \right\rangle_A \left| X \right\rangle_B  = e^{i \alpha} \left| \psi \right\rangle_A \left| \psi \right\rangle_B = \left| \xi \right\rangle$$

其次U当然也可把$\phi$由A复制B

$$ U \left| \phi \right\rangle_A \left| X \right\rangle_B  = e^{i \beta} \left| \phi \right\rangle_A \left| \phi \right\rangle_B = \left| \chi \right\rangle$$

计算：

$$\left\langle \chi \mid \xi \right\rangle = e^{-i \beta} e^{i \alpha} \left\langle \phi \mid \psi \right\rangle_A \left\langle \phi \mid \psi \right\rangle_B   $$

$$= \left\langle X \right|_B \left\langle \phi \right|_A  U^\dagger U \left| \psi \right\rangle_A \left| X \right\rangle_B  =\left\langle \phi \mid \psi \right\rangle_A  \left\langle X \mid X \right\rangle_B = \left\langle \phi \mid \psi \right\rangle_A$$

上式利用了厄米算符的性质：$U^\dagger U = 1$ (反厄米算符对这个证明也成立)

小结一下：

$$e^{i (\alpha - \beta)} \left\langle \phi \mid \psi \right\rangle_A \left\langle \phi \mid \psi \right\rangle_B  =   \left\langle \phi \mid \psi \right\rangle_A $$

假设：$x = \left\langle \phi \mid \psi \right\rangle = \left\langle \phi \mid \psi \right\rangle_A = \left\langle \phi \mid \psi \right\rangle_B $

对等式的左右两边取绝对值。

$$ |x|^2 = |x| $$

$x$的解只有两种情况：

1. $x = 1$，即$\left| \phi \right\rangle= e^{i \gamma} \left| \psi \right\rangle$
2. $x = 0$，即$\left| \psi \right\rangle \perp \left| \phi \right\rangle$

这意味着，假如存在量子态$\left| \psi \right\rangle$可以被复制，那么只有和它垂直的或平行的量子态可以被复制，其他量子态都不可被复制。

## Ref

- [No-Cloning Theorem (Proof)](https://www.youtube.com/watch?v=ydh7Xxh-8lg)
