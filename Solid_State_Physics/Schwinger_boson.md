
# Schwinger玻色子平均场理论

## Heisenberg模型

磁学系统中最简单典型模型就是Heisenberg模型，在自旋晶格系统中，由于交换作用这个系统的基态是磁性离子自旋排列的有序状态。常见的简单磁有序状态是：铁磁序、反铁磁序以及亚铁磁序。铁磁序为各格点上自旋取向一致的状态，反铁磁序和亚铁磁序描述的则是相邻磁离子自旋取向相反的情况，它们在子晶格中自旋取向一致。

Heisenberg模型哈密顿量通常表示为：

$$ H=\sum_{\langle i,j\rangle}J_{ij}\vec{S}_i\cdot\vec{S}_j $$


其中$J_{ij}$称为交换积分，$\vec{S}_i$代表第$i$个格点上磁性离子的向量自旋算符。当$J<0$时，基态为铁磁序，其近邻格点上的自旋趋于平行排列。当$J>0$时可用于描述反铁磁序，其近邻格点上的自旋趋于反平行排列，这时往往可以把晶格分为两个子晶格，在每个子晶格中自旋平行排列和铁磁情况一样，而两个子晶格自旋取向相反，因此总的自发磁化相互抵消，这就是反铁磁体的双子格模型。下面写出双格子模型的哈密顿量：

\begin{align*}
H=&|J|\sum_{i,\delta}\left\{S_{a,i}^zS_{b,i+\delta}+\frac{\varepsilon}{2}(S_{a,i}^+S_{b,i+\delta}^- +S_{a,i}^-S_{b,i+\delta}^+)\right\}\\
+&|J|\sum_{j,\delta}\left\{S_{b,j}^zS_{a,j+\delta}+\frac{\varepsilon}{2}(S_{b,j}^+S_{a,j+\delta}^- +S_{b,j}^-S_{a,j+\delta}^+)\right\}
\end{align*}

其中 $\vec{S}_{a,i}$ 为子格$a$中$i$格点上的算符，$\vec{S}_{b,j}$ 为$b$子格中$j$格点上的自旋；$\delta$代表近邻格点间位矢差；$\varepsilon$为交换各向异性常熟，当$\varepsilon=1$时退化为Heisenberg模型。

**自旋波理论**已经很好的给出了二维，三维Heisenberg模型的基态和低能激发态的性质。Schwinger- boson平均场理论并不依赖于基态性质，把自旋算符表示为玻色子的形式，与Holstein-Primarkov玻色子相比，它并不包括开平方项，已经成功用于一维和二维铁磁、反铁磁、一维亚铁磁以及梯型材料；并且可对二维混合自旋模型在零温时的色散关系进行定量计算。对于整数自旋晶格问题，利用Schwinger- boson平均场理论不仅能够计算得到Haldane激发谱能隙的存在，而且对于二维$T=0$的问题；三维低温情况，还可以得出反铁磁长程序与Schwinger玻色子凝聚有关。

## Schwinger玻色子

下面就来介绍处理Heisenberg模型的Schwinger-boson平均场理论。在Schwinger-boson表象中，自旋算符写作：

\begin{align*}
S_i^+&=b_{i\uparrow}^\dagger b_{i\downarrow}\\
S_i^-&=b_{i\downarrow}^\dagger b_{i\uparrow}\\
S_i^z&=\frac{1}{2}(b_{i\uparrow}^\dagger b_{i\uparrow}- b_{i\downarrow}^\dagger b_{i\downarrow})
\end{align*}

$b_{i\uparrow}^\dagger,b_{i,\downarrow}$为玻色子产生、消灭算符，满足玻色对易关系

$$ \{ b_{i\sigma},b_{j\sigma}^\dagger\}_- =\delta_{ij}\;\;\;,\;\;\;\{ b_{i\sigma}^\dagger,b_{j\sigma}^\dagger \}_- = \{ b_{i\sigma},b_{j\sigma}\}_-=0 $$


做了算符投影变换后，自旋算符应自洽地满足玻色子约束条件：


$$ \sum_{\sigma=\uparrow,\downarrow}b_{i\sigma}^\dagger b_{i\sigma}=2S $$

考虑各向同性反铁磁体晶格，哈密顿量写为：

\begin{align*}
H&=\frac{J}{2}\sum_{\langle ij\rangle}A_{ij}^\dagger A_{ij}+NzJS^2\\
A_{ij}^\dagger&=b_{i\uparrow}^\dagger b_{j\downarrow}^\dagger-b_{i\downarrow}^\dagger b_{j\uparrow}^\dagger\\
A_{ij}&=b_{i\uparrow}b_{j\downarrow}-b_{i\downarrow}b_{j\uparrow}\\
\end{align*}

为了考察反铁磁体双格子问题，对任意$j$格点算符作变换：

$$ b_{j\uparrow}\to -b_{j\downarrow}\;\;\;,\;\;\;b_{j\downarrow}\to -b_{j\uparrow} $$

易证明变换后玻色对易关系保持。下面采用**平均场**近似：

\begin{align*}
A_{ij}^\dagger A_{ij}&\simeq \langle A_{ij}^\dagger\rangle A_{ij}+A_{ij}^\dagger\langle A_{ij}\rangle-\langle A_{ij}^\dagger\rangle\langle A_{ij}\rangle\\
A&= \langle A_{ij}^\dagger\rangle= \langle A_{ij}\rangle
\end{align*}

从而Heisenberg模型哈密顿量可化为

\begin{align*}
H&=-\frac{J}{2}A\sum_{\langle ij\rangle}(A_{ij}^\dagger +A_{ij})+\lambda\sum_{i\sigma}b_{i\sigma}^\dagger b_{i\sigma}+E_0\\
E_0&=\frac{1}{2}zNJS^2+\frac{1}{4}JA^2Nz-2\lambda NS\\
\end{align*}

其中$z$是配位数，$N$是格点数，$\lambda$是引入玻色子约束条件的Lagrange乘子。
接着进行Fourier变换，在动量空间中作Bogoliubov变换或者运动方程对角化方法对哈密顿量进行对角化，得到对角化后的哈密顿量

\begin{align*}
H&=\sum_k\omega_k(\alpha_k^\dagger\alpha_k+\beta_k^\dagger\beta_k+1)+E_0-\lambda N\\
E_0&=\frac{1}{2}zNJS^2+\frac{1}{4}JA^2Nz-2\lambda NS-\lambda A\\
\omega_k&=\sqrt{\lambda^2-(JAZ\gamma_k)^2}\;\;\;,\;\;\;\gamma_k=\frac{1}{z}\sum_\delta e^{i k\cdot\delta}
\end{align*}

于是可得系统的自由能：

$$ F=E_0+\frac{2}{\beta}\sum_k\ln(1-e^{-\beta\omega_k}+\omega_k) $$

## 自洽方程组

利用自由能分别对两个参量$A$和$\lambda$求偏微分来得到**鞍点方程**：

$$ \frac{\partial F}{\partial A}=0\;\;\;,\;\;\;\frac{\partial F}{\partial\lambda}=0 $$

这样就得到两个**自洽方程**，进而通过自洽地数值求解可以得到不同条件下的结果，计算物理上的可观测量。





