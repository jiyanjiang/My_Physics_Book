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

$$ \frac{M_0 - M_T }{M_0} = \frac{0.0587 }{Z_c} \left( \frac{k_B T}{2Js} \right)^{3/2} $$

$Z_c = 1, 2, 4$ for SC, BCC, or FCC lattice.

The best way to derive $A_{ex}$ (exchange stiffness) is from $D_{sw}$,

$$A_{ex}(T) =  \frac{M_s(T) D_{sw} }{2 g \mu_B} $$

typical A value for cobalt is $31 pJ m^{-1}$

For $T=0$ case:

$$A(0) \approx \frac{J S^2 Z_c }{a_0}  $$

$Z_c$ is the number of atoms per unit cell

unit cell | $Z_c$ | A
--- | --- | ---
sc | 1 | $J S^2/a$
bcc | 2 | $2 J S^2/a$
fcc | 4 | $4 J S^2/a$
hcp |  | $2 \sqrt{2} J S^2/a$ 

the exchange length $l_{ex}$

$$l_{ex} = \sqrt{\frac{A}{\mu_0 M_s^2}}$$

## Magnetization

$$ \left\langle n_k \right\rangle_T = \frac{1}{e^{\hbar \omega_k / kT} - 1} $$

$$\frac{1}{N} \sum\limits_k \left\langle n_k \right\rangle_T = \alpha \left( \frac{k_B T }{2SJ} \right)^{3/2}  $$

$$ M(T) = g \mu_B \sum\limits_l \left( S - \left\langle n_l \right\rangle_T \right) $$


$$ = N g \mu_B S - g \mu_B \sum\limits_k \left\langle n_k \right\rangle_T  $$

$$ = M(0) \left( 1  - \frac{\alpha}{S} \left( \frac{k_B T}{ 2 SJ }  \right)^{3/2} \right) $$

$$ M(0) = N g \mu_B S $$


$$ M_S(0) = \frac{Q}{a^3} g \mu_B S$$


spin quantum number:

$$ S = \frac{M_S(0) a^3}{ Q g \mu_B } $$

https://journals.aps.org/prb/pdf/10.1103/PhysRevB.66.144426

unit cell   | $\alpha$ | Q | 
--- | --- | --- | ---
sc | 0.117/2 | 1 | 0.0587
bcc | 0.117/4 | 2 | 0.0587/2
fcc | 0.117/8 | 4 | 0.0587/4
