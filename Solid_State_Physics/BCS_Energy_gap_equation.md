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

序参量$\Delta$的物理含义是能隙（Energy gap）。

考虑有限温度情形（$T > 0$），能隙方程为：

$$ \Delta(T) = V \sum\limits_k \left\langle  c_{-k}c_k \right\rangle_T $$

把线性变换代入上式中的电子算符$c_{-k} c_k$，得到：

$$ \Delta(T) = \sum\limits_k u_k v_k \left( 1- \left\langle \alpha^\dagger_k \alpha_k \right\rangle_T - \left\langle \alpha^\dagger_{-k} \alpha_{-k} \right\rangle_T \right) $$

