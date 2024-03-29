# 为什么不能达到绝对零度？


绝对零度，指的是热力学温标中的零度，相当于摄氏温标中的零下273.15°C。根据热力学定律，绝对零度在自然界中永远没法达到。

考虑一台理想的制冷机（冰箱），制冷机的效率被定义为：制冷机从低温热源的吸热（$Q_C$）除以制冷机在热力学循环中做的功（$W$），

$$\eta = \frac{Q_C}{W}$$

<img width="483" alt="截屏2022-07-22 08 53 25" src="https://user-images.githubusercontent.com/6512579/180339605-4f8023b7-ace0-4848-a657-548dc6a30486.png">

根据**热力学第二定律**：不可能存在一个制冷机，能够把从低温物体吸收来的热量全部传输到高温物体中而不产生任何其他效果。这意味着我们必须做功（$W$），才能使系统从低温吸热（$Q_C$），到高温放热（$Q_H$），

$$\eta = \frac{Q_C}{W} = \frac{Q_C}{Q_H - Q_C} = \frac{T_C}{T_H - T_C}\to 0$$

假设低温温度无限接近零温（$T_C \to 0$），这意味着制冷机的效率此时也趋于0，换句话说当低温温度无限接近零温时，我们需要做无穷大的功，才能继续从低温吸收有限的热量。

$$W = \frac{Q_C}{\eta} \to \infty$$

小结一下：热量无法自发地从低温传到高温，如果我们要使热量从低温物体传到高温物体，我们就必须对系统做功。如果我们要使一个有限温度的物体降温降到绝对零度，就需要我们不断地从低温物体上把热量传到高温物体中。随着低温物体的不断降温，趋于绝对零度，继续从低温物体吸取热量所需做的功将趋于无穷大。

这意味着，我们永远无法把一个物体从有限温度通过有限过程（有限做功）降温降到绝对零度。这个洞见最早是德国物理化学家——能斯特（Nernst，1864-1941）——在1912年提出的。

虽然绝对零度我们永远无法达到，但在实验室里我们可以无限逼近绝对零度。随着低温技术的发展，人类在实验室能够达到的最低温度一直在刷新中。目前我查到的最低记录是100pK，或$1 \times 10^{-10} K$。

下图是实验装置示意图：

![image](https://user-images.githubusercontent.com/6512579/180339814-8e75c2df-d7fc-4cfd-acd1-d518bca70173.png)

如图偏上方中央有个小黑点，这里样品温度可达到低于1nK ($1 \times 10^{-9}K$)。
