# 受迫振动

考虑力学里的受迫振动问题，假设一个弹簧，弹性回复系数是$k$，假设这个弹簧是理想的，没有阻尼，也没有外界的驱动。

这个问题是理想的简谐振子，如果有一个质量为$m$的物体拴在这个弹簧上的话，它收到的力只有：$F=-kx$，再考虑牛顿第二定律：$F=ma=-kx$，即：

$$ m \ddot x = - kx$$

x上面的两个点表示对位置求二阶导数。

这个微分方程的解可表示为：

$$x = A \cos \left( \omega_0 t + \phi_0 \right) $$

$$\omega_0 = \sqrt{\frac{k}{m}} $$

进一步，我们考虑质量为$m$的振子运动起来会受阻力，这个阻力的大小与速度成正比，方向与速度相反，即：$-\gamma v$，这里$\gamma$表示阻尼系数，$v$表示振子的速度。

最后，我们考虑外界的驱动，假设外界的驱动是个周期性的外力$f$，角频率为$\Omega$，

$$f = H \cdot \cos \Omega t$$

这几个要素一起考虑的话，弹簧振子的牛顿第二定律可写为：

$$m \ddot x = - kx - \gamma \dot x + H \cos \Omega t $$

引入新的参数：

$$ \omega_0^2 = \frac{k}{m}, \beta = \frac{\gamma}{2m}, h = \frac{H}{m} $$

微分方程可改写为：

$$\ddot x + 2\beta \dot x + \omega_0^2 x = h \cos \Omega t $$

现在的问题是如何求受迫振动的解：$x(t)$。

现在用复数向量法求解$x(t)$，即把$x$看成是向量，取实部后对应物理的解，复数向量满足的微分方程是：

$$\ddot x + 2\beta \dot x + \omega_0^2 x = h e^{i \Omega t} $$

考虑试探波函数：

$$x(t) = A e^{i \omega t } e^{- \beta t} + B e^{i (\Omega t + \phi)} $$

第一项对应角频率为$\omega$的阻尼振动，第二项对应角频率为$\Omega$的振动解。

分别求出$x$的一阶导数和$x$的二阶导数，

$$\dot x = (i \omega - \beta)A e^{(i \omega - \beta)t} + i \Omega B e^{i (\Omega t + \phi) } $$

$$\ddot x = (i \omega - \beta)^2 A e^{(i \omega - \beta)t} - \Omega^2 B e^{i (\Omega t + \phi)} $$

代入到包含周期驱动力的微分方程中去。

包含$\omega$的复数向量因子应当为0，

$$ (i \omega - \beta)^2 + 2 \beta (i \omega - \beta ) + \omega_0^2 = 0$$

求出：

$$\omega = \sqrt{\omega_0^2 - \beta^2 }$$

考虑微分方程中包含$\Omega$的部分，求出：

$$\cos \phi = \frac{B \left( \omega_0^2 - \Omega^2 \right)}{h}$$

$$\sin \phi = - \frac{2 \beta \Omega B}{h} $$

考虑正弦函数的平方加余弦函数的平方是1，求出：

$$B = \frac{h}{\sqrt{ \left( \omega_0^2 - \Omega^2 \right)^2 + 4 \beta^2 \Omega^2 } }$$

最终我们求出的解是一个频率为$\omega$随时间衰减的振荡，与频率为$\Omega$不随时间衰减的振荡的叠加。时间足够长后，只有后者能存在，其频率就是$\Omega$，振幅是$B$。

由$B$的表达式，我们可以看出当周期性外力的频率$\Omega$等于系统没有阻尼时的固有振荡频率$\omega_0$时，振幅$B$达到最大，此时对应的就是共振。如果与此同时，阻尼β也很小的话，不论周期性外力f多么小，它最终都会驱使受迫振动的振幅变得很大很大。

以上就是共振现象的物理学解释，这里虽然是以力学为例的，但对电路的RCL共振等其他物理现象也适用。
