# 线性自旋波理论

## 海森堡模型

$$H = - J \sum\limits_{ij} s_i \cdot s_j   $$


$J>0$, FM, 平行排列

## 量子海森堡模型

$$ H = -J \sum\limits_{l, \delta}\frac{S_{l}^+S_{l+\delta}^- + S_{l}^-S_{l+\delta}^+}{2} + S_l^z S_{l+\delta}^z $$ 

## H-P 变换(线性自旋波)

引入自旋偏离：$n = S - m$, $m = 0, \pm 1, ... \pm S$

$$ n = 0, 1, 2, ..., 2S $$


$$ S^+ = \sqrt{2S -a^\dagger a} a$$


$$ S^- = a^\dagger \sqrt{2S -a^\dagger a}$$

$$ S_z = S - a^\dagger a $$

考虑低能激发：$\left\langle n \right\rangle \ll 2S$

$$ \hbar \omega_k = 2 z JS (1 - \cos ka) $$

长波极限(k small)下：

$$\hbar \omega_k = zJS k^2a^2 = D_{sw} k^2 $$

$D_{sw}$ is the spin-wave stiffness

$$D_{sw} = z J S a^2$$

For cobalt, $D_{sw} = 8.0 \times 10^{-40 } J m^2$ (500 meV \AA^2)

## Bloch-3/2 law

Exchange stiffness ($A_ex$) was obtained from the best-fit based on the Bloch-3/2 law:

$$ \frac{M_0 - M_T }{M_0} = \frac{0.0587 }{\nu} \left( \frac{k_B T}{2Js} \right)^{3/2} $$

$\nu = 1, 2, 4$ for SC, BCC, or FCC lattice.

The best way to derive $A_{ex}$ (exchange stiffness) is from $D_{sw}$,

$$A_{ex}(T) =  \frac{M_s(T) D_{sw} }{2 g \mu_B} $$

typical A value for cobalt is $31 pJ m^{-1}$

For $T=0$ case:

$$A(0) \approx \frac{J S^2 Z_c }{a_0}  $$

$Z_c$ is the number of atoms per unit cell

unit cell | $Z_c$
--- | ---
sc | 1
bcc | 2 
fcc | 4
