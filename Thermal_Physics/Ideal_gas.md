# 理想气体的压力

考虑：

$$\frac{mv_x^2}{2} = \frac{mv_y^2}{2} = \frac{mv_z^2}{2} = \frac{k T}{2}$$

即：

$$\frac{mv^2}{2} = \frac{3kT}{2}$$

对给定体积的气体，气体分子会像下雨一样冲击容器的器壁，考虑时间$\Delta t$，有：$\frac{n V}{6} = \frac{n S v \Delta t}{6}$个的气体分子撞向了器壁，这里$v$是气体分子的速度，$n$是气体分子的数密度，因子1/6是说大致只有1/6分子会撞到某方向的器壁上。

假设气体分子与器壁碰撞后，其速度就变为$-v$。

现在可以计算所有气体分子的总的$\Delta \vec p$为（以下只考虑大小）：

$$\frac{nV}{6} (2mv) = \frac{n V mv}{3}$$

考虑[冲量定理](https://github.com/jiyanjiang/My_Physics_Book/blob/main/Mechanics/Impulse.md)：

$$F \Delta t = \frac{nS v \Delta t (mv)}{3}$$

压强 $P$ 为

$$P = \frac{F}{S} =\frac{n mv^2}{ 3 }$$

这里$n = \frac{N_A}{V_{m}}$是数密度，$N_A$是阿佛加德罗常数，$V_m$是摩尔体积，

$$P = \frac{N_A mv^2 }{3 V_m}$$

考虑气体分子动能与温度之间的关系：

$$\frac{mv^2}{2} = \frac{3 k_B T}{2}$$

得到：

$$P V_m = \frac{2 }{3} N_A \frac{mv^2}{2} = \frac{2 }{3} N_A  \frac{3 k_B T}{2} = N_A k_B T$$

这里：$N_A k_B = R$，即普遍适气体常数。

假设有$\mu$摩尔气体，$V = \mu V_m$

$$PV = \mu RT$$

上式就是著名的玻意耳定律。
