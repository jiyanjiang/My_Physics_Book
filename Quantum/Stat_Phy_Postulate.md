# 统计力学的基本假设



## 经典统计

经典动力学系统可用相空间中点的运动表示。一个粒子就是$(q, p)$，$q$是广义坐标，$p = \frac{\partial L}{\partial \dot q}$（$L = T -V$是拉格朗日量），粒子的运动用相空间中$(q,p)$的轨迹来表示。

$N$个粒子组成的系统可用高维相空间中一个点$(q_i, p_i)$表示，这里$i = 1, ..., N$，对三维物理空间而言，每一个$q_i$对应三个独立的分量$q_i^x, q_i^y, q_i^z$，所以$N$个粒子的运动状态要用$6N$维相空间中的一个点来表示。

随着时间的变化，这个代表点会在相空间中运动，满足正则方程：

\begin{eqnarray}
\dot q_i & = & \frac{\partial H (q_i, p_i)}{\partial p_i} \\
\dot p_i & = & - \frac{\partial H (q_i, p_i) }{\partial q_i}
\end{eqnarray}


这里$i = 1, 2, ..., 3N$，对应每个粒子都有三个物理的维度($x, y, z$)。

现在，我们考虑这个系统大量思维复本（mental copies）的集合，即一个系综（ensemble）。系综中每个元素对应相空间中的一个代表点。我们期望系综中各元素在任意时刻$t$处在所有可能（允许）的（微观）状态，并假定宏观状态（人通过宏观仪器记录到的态）是全体系综元素所规定的态。

我们规定$\rho (q, p; t)$是$t$时刻系综代表点在$(q, p)$附近的“几率密度”。由于给定系综既不接受新元素，也不驱除老元素，即代表点的总数守恒，得到代表点的连续性方程：

\begin{equation}
\frac{\partial \rho}{\partial t } + \nabla \cdot j = 0
\end{equation}

相空间中“几率流”($j$)的散度是：

\begin{equation}
\nabla \cdot j = \nabla \cdot ( \rho v) = \sum\limits_i \frac{\partial }{\partial q_i} (\rho \dot q_i ) + \frac{\partial }{\partial p_i }(\rho \dot p_i) 
\end{equation}

几率密度$\rho(q, p ; t)$不随时间变化（对应系统的宏观陈述，如$P, V, T$不随时间变化）：

\begin{equation}
\frac{d \rho }{dt } = \frac{\partial \rho }{\partial t } + \sum\limits_i \left( \frac{\partial \rho}{ \partial q_i } \dot q_i + \frac{\partial \rho }{\partial p_i} \dot p_i \right) = 0
\end{equation}

考虑正则方程，

\begin{equation}
\sum\limits_i \frac{\partial \rho}{ \partial q_i } \dot q_i + \frac{\partial \rho }{\partial p_i} \dot p_i = \sum\limits_i \frac{\partial \rho}{ \partial q_i } \frac{\partial H }{\partial p_i}  - \frac{\partial \rho }{\partial p_i} \frac{\partial H}{\partial q_i} = \left\{ \rho , H  \right\}
\end{equation}

上式，最后一步利用了泊松括号（Poisson bracket）的定义：

\begin{equation}
\left\{ f, g \right\} = \sum\limits_i \left( \frac{\partial f}{\partial q_i} \frac{\partial g}{\partial p_i} -  \frac{\partial f}{\partial p_i} \frac{\partial g}{\partial q_i} \right)
\end{equation}

得到“几率密度”在相空间中运动所满足的方程：

\begin{equation}
\frac{\partial \rho }{\partial t } = - \left\{ \rho, H  \right\}
\end{equation}

上式就是刘维定理（Liouville's theorem）。刘维定理意味着代表点的密度不随时间变化，这表明代表点在相空间中的运动与不可压缩流体的运动相同。

如果$\left\{ \rho , H  \right\} = 0$，则$\rho(q, p) = \text{const}$，这就是“等几率假设”，即$\rho$在相空间所允许的各个地方都相同，对应的系综叫微正则系综（Microcanonical ensemble）。

物理量$f(q,p)$的系综平均（对应宏观观测量）是：

\begin{equation}
\left\langle f \right\rangle =  \int dq dp \rho(q,p) f(q,p)
\end{equation}

实际测量中，我们测量的是物理量对时间的平均，

\begin{equation}
\left\langle f \right\rangle_\tau = \lim\limits_{\tau \to \infty }\frac{1}{\tau} \int_0^{\tau} dt f(q, p, t)
\end{equation}

测量时间（人的反应时间是$10^{-1}$秒数量级）$\tau$应远大于系统微观碰撞的特征时间（小于$10^{-10}$秒[^1]，超快过程对应的时间是小于$10^{-9}$秒），这意味着我们在使用宏观测量仪器完成测量时系统已经完成了无穷多个碰撞过程，经历了无穷多可能的微观状态。

[^1]: 想象一个宏观小，微观大的探针放在气体里，探针将受到周围气体分子非常密集的撞击。

我们把这些微观状态用相空间中的代表点表示，并假设这些代表点均匀地分布在相空间允许区域的每个部分，这就是所谓“各态历经定理”或“各态历经假说”（ergodic hypothesis）。

各态历经假说最早是由玻尔兹曼在1871年提出的，可表述为：

> 一个代表点的轨迹随着时间的推移将通过相空间允许区域的任何点的任何邻域。

以上表述与玻尔兹曼的原始叙述稍有不同，称为“准各态历经假说”。这样我们就可通过计算物理量的系综平均来得到物理量的宏观测量值了（这里就是长时间的平均值）。

对于微正则系综（能量$E$保持不变），系综并不是完全孤立的，而是与环境保持着“热接触”，环境可看作是除系统外的全部宇宙，环境的运动状态我们是无法完全确定的。系统由于与环境的相互作用，将以完全随机的方式演化，因此只要时间足够长，代表点将均匀地充满整个相空间允许的区域。这样，我们就把描述宏观现象的统计物理与描述微观现象的动力学理论联系起来了。

## 量子统计

类似于对经典统计的讨论，我们认为系统与环境处在“热平衡”状态。在量子力学中，我们使用波函数（或态矢量）$\left| \psi \right\rangle$来表示系统微观运动状态。假设系统的哈密顿量是$H$，存在能量本征态$\left| n \right\rangle$，

\begin{equation}
H \left| n \right\rangle = E_n \left| n \right\rangle
\end{equation}

这里$\left\{ \left| n \right\rangle  \right\}$组成完全集，因此$\left| \psi \right\rangle$可表示为：

\begin{equation}
\left| \psi \right\rangle = \sum\limits_n \left| n \right\rangle \left\langle n | \psi \right\rangle = \sum\limits_n c_n \left| n \right\rangle
\end{equation}

假设系统对应的力学量是$x$，

\begin{equation}
\left\langle x | \psi \right\rangle = \sum\limits_n \left\langle  x \mid n \right\rangle \left\langle n \mid \psi \right\rangle= \sum\limits_n c_n \left\langle x | n \right\rangle
\end{equation}

如果考虑量子态可以随时间演化，即$\left| \psi , t \right\rangle$

\begin{equation}
\psi(x, t) = \left\langle x | \psi, t \right\rangle = \sum\limits_n c_n(t) \left\langle x | n \right\rangle = \sum\limits_n c_n(t) \varphi_n(x) 
\end{equation}

假设系统的每一个能量本征函数$\varphi_n(x) $都对应一个环境的量子态，用波函数$c_n (y,t)$表示，总波函数（$\Psi(x,y,t)$，考虑了系统和环境）可写成系统与环境的直接乘积的形式（猫态）：

\begin{equation}
\Psi(x,y,t) = \sum\limits_n c_n(y,t) \varphi_n (x)
\end{equation}

或：

\begin{equation}
\left| \Psi \right\rangle = \sum\limits_n \left| c_n \right\rangle \left| \varphi_n \right\rangle
\end{equation}


这里我们用$x$表示系统的变量，$y$表示环境的变量，迭加系数$c_n(t)$在形式上归入环境波函数。对系统计算力学量$A$（只作用于系统波函数）的量子力学平均：

\begin{equation}
\left\langle A \right\rangle = \frac{ \left\langle \Psi \right| A \left| \Psi \right\rangle }{\left\langle \Psi | \Psi \right\rangle } =  \frac{ \sum\limits_{n,m} \left\langle c_n | c_m \right\rangle \left\langle \varphi_n \right| A \left| \varphi_m \right\rangle  }{ \sum\limits_n \left\langle c_n | c_n \right\rangle }
\end{equation}

由于$c_n(y,t)$不一定是环境的本征函数，所以不能进一步化简。对系统测量物理量$A$的宏观取值，即对应求物理量$A$的长时平均，这个对$c_n(y,t)$的平均是第二次求平均，第一次是对$\varphi_n(x)$求的量子力学平均。

第二次平均（对时间的平均）用横线表示$\overline{ \left\langle A \right\rangle}$，

\begin{equation}
\overline{ \left\langle A \right\rangle} = \frac{ \sum\limits_{n,m} \overline{ \left\langle c_n | c_m \right\rangle }  \left\langle \varphi_n \right| A \left| \varphi_m \right\rangle  }{ \sum\limits_n \overline{ \left\langle c_n | c_n \right\rangle } } 
\end{equation}

假设$\Psi$保持守恒（没有粒子的产生和湮灭过程），即$\left\langle \Psi | \Psi \right\rangle = 1$，那么$\sum\limits_n \overline{ \left\langle c_n | c_n \right\rangle } = \sum\limits_n \left\langle c_n | c_n \right\rangle = 1 $是不含时的。

现在，我们做如下假设：

* 先验等几率假设（Postulate of equal a-Priori probabilities）：

如果$E \le E_n \le E + \delta$（$\delta \to 0$），$\left\langle c_n | c_n \right\rangle = \text{const}$，否则$\left\langle c_n | c_n \right\rangle = 0 $（对应微正则系综）。

* 无规相假设（Postulate of random phases）：假设环境也存在能量本征态$\left\{ \left| \theta_j (y) \right\rangle  \right\}$，对$m \neq n$，$\left\langle c_n, t | c_m,t  \right\rangle$可表示为：

\begin{eqnarray*}
\left\langle c_n, t | c_m,t  \right\rangle & = & \sum\limits_{j,k} c_{nj}^*(t) c_{mk}(t ) \left\langle \theta_j | \theta_k \right\rangle    \\
{} & = & \sum\limits_j c_{nj}^*(t) c_{mj}(t ) \\
{} & = & \sum\limits_j |c_{nj} c_{mj}| e^{i (\theta_{mj} - \theta_{nj})}
\end{eqnarray*}

假设不同时刻$t$计算出来的相位$(\theta_{mj} - \theta_{nj}) $完全随机（非相干的），则：

\begin{equation}
\overline{ \left\langle c_n, t | c_m,t  \right\rangle } = \sum\limits_j \left| c_{nj} c_{mj} \right| \overline{  e^{i ( \theta_{mj} - \theta_{nj} ) } } = 0 
\end{equation}

这意味着由于系统与环境的相互作用，系统波函数$\psi$是完全集$\varphi_n$的非相干迭加。量子相干性以及系统与环境间是否存在去相干（decoherence）是宏观物理学（量子统计）与微观物理学（解薛定谔方程）间区分的判据。



最终得到：

\begin{equation}
\overline{ \left\langle A \right\rangle} = \sum\limits_n |c_n|^2 \left\langle \varphi_n \right| A \left| \varphi_n \right\rangle
\end{equation}

对量子统计，我们可以引入密度算符(density operator)：

\begin{equation}
\rho = \sum\limits_n \left| \varphi_n \right\rangle \rho_n \left\langle \varphi_n \right|
\end{equation}

$\rho_n$是系统处于态$\left| \varphi_n \right\rangle$的几率，满足：

\begin{equation}
\sum\limits_n \rho_n = 1
\end{equation}

力学量$A$的系综平均：

\begin{equation}
\left\langle A \right\rangle = \text{Tr} \rho A
\end{equation}

对密度算符$\rho$求时间偏导，并利用薛定谔方程$i \hbar \frac{\partial }{\partial t } \left|   \right\rangle = H \left|   \right\rangle  $，可以得到量子刘维定理：

\begin{equation}
i \hbar \frac{\partial \rho }{\partial t } = \left[ H, \rho  \right]
\end{equation}

## 参考

* 帕斯利亚《统计力学·上册》（中译本），pp49；

* K. Huang, Statistical Mechanics, 2nd Edition, John Wiley & Sons, pp171; 

* Michael W. Noel, etc., PRL 77, 1913 (1996)
