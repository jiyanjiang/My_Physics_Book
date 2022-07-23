# 超交换机制


考虑两个电子，分别位于格点1和格点2。电子可以在格点间跳来跳去，用$H_t$项表示：

$$H_t = - t \sum\limits_{\sigma} c_{1 \sigma}^\dagger c_{2 \sigma} + c_{2 \sigma}^\dagger c_{1 \sigma} $$

当两个电子位于相同格点时，具有“库仑能”：

$$ \mathscr{U} = U \sum\limits_i n_{i \uparrow} n_{i \downarrow} $$

假设$U \gg t$，$\mathscr{U}$看做是0级贡献，$H_t$看做是微扰。

基态是两个格点上各占据一个电子，共有4个:

$$\left| \uparrow, \uparrow \right\rangle$$

$$\left| \uparrow, \downarrow \right\rangle$$

$$\left| \downarrow, \uparrow \right\rangle$$

$$\left| \downarrow, \downarrow \right\rangle$$

构成一个集合，记作：$GS$。基态能是0。

回忆二阶微扰的公式：

$$E_n^{(2)} = E_n^{(0)} + H'_{nn} + \sum\limits_{m \neq n} \frac{|H'_{mn}|^2}{E_n^{(0)} - E_m^{(0)}}$$

这里$n \in GS$, $m$是中间态。

能量的1阶修正，对应$H'_{nn}$，这里是：

$$\left\langle n \right| H_t \left| n \right\rangle $$

由于$H_t$的作用使得$H_t \left| n \right\rangle $不再属于基矢$\{ 0 \}$，因此：

$$ \left\langle n \right| H_t \left| n \right\rangle = 0 $$

现在计算能量的2阶修正，

首先由于泡利不相容原理，需要排斥这样的态：

$$ \left| \uparrow, \uparrow \right\rangle  \to  \left| \uparrow \uparrow, 0 \right\rangle$$

除此之外需考虑：

（1）

$$\left| \uparrow, \downarrow  \right\rangle \to \left| \uparrow \downarrow, 0 \right\rangle \to \left| \downarrow, \uparrow \right\rangle $$

$$\left| \uparrow, \downarrow \right\rangle \to \left| 0,  \uparrow \downarrow \right\rangle \to \left| \downarrow, \uparrow \right\rangle $$

这两个过程的特点是：1格点的自旋降1，2格点的自旋升1，可记作：

$$S_1^- S_2^+ \left| \uparrow, \downarrow \right\rangle = \left| \downarrow, \uparrow \right\rangle $$

同时对这两个中间态进行2阶微扰计算：

$$ - \frac{2 t^2}{U} S_1^- S_2^+$$

（2）

$$\left| \downarrow, \uparrow \right\rangle \to \left| \uparrow \downarrow, 0 \right\rangle \to \left| \uparrow, \downarrow \right\rangle $$

$$\left| \downarrow, \uparrow \right\rangle \to \left| 0,  \uparrow \downarrow \right\rangle \to \left| \uparrow, \downarrow \right\rangle $$

这两个过程的特点是：1格点的自旋升1，2格点的自旋降1，可记作：

$$ S_1^+ S_2^- \left| \downarrow, \uparrow \right\rangle = \left| \uparrow, \downarrow \right\rangle $$

同时对这两个中间态进行2阶微扰计算：

$$ - \frac{2 t^2}{U} S_1^+ S_2^-$$

（3）

最后还有4个过程，两格点上自旋取向没有变化：

$$ \left| \uparrow, \downarrow \right\rangle = \left| \uparrow \downarrow, 0 \right\rangle = \left| \uparrow, \downarrow \right\rangle$$

$$ \left| \uparrow, \downarrow \right\rangle = \left| 0, \uparrow \downarrow \right\rangle = \left| \uparrow, \downarrow \right\rangle$$

和

$$ \left| \downarrow, \uparrow \right\rangle = \left| \uparrow \downarrow, 0 \right\rangle = \left| \downarrow, \uparrow   \right\rangle$$

$$ \left| \downarrow, \uparrow \right\rangle = \left| 0, \uparrow \downarrow \right\rangle = \left| \downarrow, \uparrow   \right\rangle$$

可记作：

$$ S_1^z S_2^z \left| \uparrow, \downarrow \right\rangle = - \frac{1}{4} \left| \uparrow, \downarrow \right\rangle $$

或

$$ S_1^z S_2^z \left| \downarrow, \uparrow \right\rangle = - \frac{1}{4} \left| \downarrow, \uparrow \right\rangle $$

考虑二阶微扰：

$$ - \frac{4t^2}{U} S_1^z S_2^z $$

综合以上（1）（2）（3）过程，考虑2阶微扰后，有效哈密顿量是：

$$ H_{eff} = \frac{4t^2}{U} \hat S_1 \cdot \hat S_2 $$

展开：

$$H_{eff} = \frac{2t^2}{U}\left( S_1^- S_2^+ + S_1^+ S_2^- \right) + \frac{4t^2}{U} S_1^z S_2^z $$


## Reference

- Assa Auerbach, Interacting electrons and quantum magnetism, pp16
