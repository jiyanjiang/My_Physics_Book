# 超导能隙方程

假设费米面附近动量和自旋都相反的电子通过有效吸引形成库帕对。

有效哈密顿量为：

$$ H = \sum\limits_k E_k \left( c^\dagger_{k \uparrow} c_{k \uparrow} + c^\dagger_{ -k \downarrow} c_{ -k \downarrow} \right) - V \sum\limits_{k k'} \left( c^\dagger_{ k' \uparrow } c^\dagger_{  -k' \downarrow } c_{ -k \downarrow }   c_{k \uparrow}   \right) $$

引入记号的简化：用$k$表示$k \uparrow$，$-k$表示$-k \downarrow$

费米面附近电子的能量：

$$ \epsilon_k = E_k - \mu  $$

这里$\mu$是化学势，或费米能($E_F$)。

有效哈密顿量为：

$$ H = \sum\limits_k \epsilon_k (c^\dagger_k c_k + c^\dagger_{-k} c_{-k}  ) - V \sum\limits_{k k'} c^\dagger_{k'} c^\dagger_{-k'} c_{-k} c_k $$

假设发生“库帕对”凝聚的态是上述哈密顿量的本征态

$$ \left| \psi \right\rangle = \sum\limits_{k > k_F}  a(k)  c^\dagger_{k} c^\dagger_{-k} \left| FS \right\rangle  $$

这里FS表示费米球（无相互作用时电子系的基态）。

利用自洽的平均场方法，可以将有效哈密顿量简化为二算子的哈密顿量，进而我们可通过线性变换（u-v变换）把它对角化。

定义库帕对发生凝聚的序参量为：

$$ \Delta = V \sum\limits_k \left\langle c_{-k}c_k  \right\rangle  $$

线性变换：

$$ \alpha_k = u_k c_k - v_k c^\dagger_{-k} $$

$$ \alpha^\dagger_k = u_k c^\dagger_k - v_k c_{-k} $$

对角化后，有效哈密顿量的形式为：

$$ H = \sum\limits_k \xi_k \left( \alpha^\dagger \alpha + \beta^\dagger \beta  \right) + \sum\limits_k (\epsilon_k - \xi_k ) + \frac{\Delta^2 }{V}$$

这里：

$$ \xi_k = \sqrt{ \epsilon_k + \Delta^2 } $$

序参量$\Delta$是能隙（Energy gap）的一半。

$$Gap = 2 \Delta$$

考虑有限温度情形（$T > 0$），能隙方程为：

$$ \Delta(T) = V \sum\limits_k \left\langle  c_{-k}c_k \right\rangle_T $$

把线性变换代入上式中的电子算符$c_{-k} c_k$，得到：

$$ \Delta(T) = \sum\limits_k u_k v_k \left( 1- \left\langle \alpha^\dagger_k \alpha_k \right\rangle_T - \left\langle \alpha^\dagger_{-k} \alpha_{-k} \right\rangle_T \right) $$

超导元激发满足费米统计

$$ \Delta(T) = V \sum\limits_k u_k v_k \left[ 1 - 2 f(\xi_k) \right] $$

把$u_k, v_k$的表达式代入上式，得到：

$$ 1 = \frac{1}{2}V \sum\limits_k \frac{ \tanh \left(\frac{1}{2} \beta \xi_k \right)  }{ \xi_k } $$

$T = T_c$ 时，$\Delta(T_c)=0$，能隙方程为：

$$ 1 = g(0) V \int_0^{\hbar \omega_D} d \epsilon \frac{ \tanh \frac{\epsilon \beta_c }{2} }{\epsilon} $$

这里$g(0)$是费米面附近的态密度。

考虑$\hbar \omega_D \ll k_B T$, 积分上限取$+ \infty$，积分化简可得：

$$ 1 = g(0) V \ln \left[  \left(  \frac{\hbar \omega_D}{k_B T_c} \right) \left( \frac{ 2 e^\gamma }{ \pi }  \right) \right] $$

这里$\gamma \approx 0.5772$，是欧拉常数。

$$ \frac{2 e^\gamma}{\pi } \approx 1.13 $$

从而

$$ k_B T_c = \frac{2 e^\gamma }{\pi } \hbar \omega_D \exp \left( - \frac{1}{ g(0)V } \right) $$

即

$$k_B T_c \approx 1.13 \hbar \omega_D \exp \left(-\frac{1}{g(0) V}\right) $$

考虑$T=0 K$时的超导能隙$\Delta(0)$：

$$ \Delta(0) \approx 2 \hbar \omega_D \exp \left( - \frac{1}{g(0)V} \right)  $$

因此，能隙($2\Delta(0)$)与$T_c$之比为：

$$ \frac{2 \Delta(0) }{ k_B T_c } = \frac{4}{1.13} \approx 3.54$$
