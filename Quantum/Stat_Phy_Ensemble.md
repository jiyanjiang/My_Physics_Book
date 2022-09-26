# 统计物理：系综概念介绍


## 宏观和微观

统计物理研究的对象是“大数自由度”的系统在宏观长时间上的平均行为。“宏观”指的是空间，空间的尺度较大，“大尺度”和“长时间”是针对特定物理系统，物理过程而言的。

对原子大小($\sim 10^{-10}m$)大小的物理系统而言，特征能量是$\sim eV$，特征时间按不确定关系估算：$\Delta \tau \Delta E \sim \hbar$，我们可计算出原子大小物理系统的特征时间:

\begin{equation*}
\Delta \tau \sim \frac{\hbar}{1eV} \sim 10^{-15}s,
\end{equation*}

对人（观察者）有意义的时间尺度是：$1s$（脉搏）， 这里$10^{-15}s$就是微观的时间尺度，$1s$就是宏观的时间尺度，其比例是：$10^{15}$。

类似我们可以估计空间的比例，典型的微观，原子大小$\sim 10^{-10}m$，典型的宏观, $1m$, 比例是：$10^{10}$。

“大自由度”，比如考虑$22.4 l$的理想气体，对人（观察者）有意义的物理量仅有P（压强），V（体积），T（温度）几个，或者说自由度很小。但如果采用微观陈述，这个系统就包括$6.02 \times
10^{23}$个粒子，自由度的比例是：$10^{23}$。

涉及大数物理规律的偏差是$\frac{1}{\sqrt N}$，$N$很大保证了统计物理规律是非常准确的[^SquareN]。

[^SquareN]: 参考：薛定谔，《生命是什么》，第一章。

## 密度算符

### 纯系综

统计物理中，我们用系综理论建立“微观——宏观”'的联系。所谓系综就是想象中的集合，对量子力学而言，即便不涉及统计物理，我们也需要系综概念以建立测量理论。

假设量子态$\left| \alpha \right\rangle$，测量力学量A，如果$\left| \alpha \right\rangle$不是A的本征态，我们无法推测测量值是多少，我们只能说可能是多少，算式$\left\langle \alpha \right| A \left| \alpha \right\rangle$给出的是所谓期望值，我们可通过一个假想的操作来得到这个期望值。

* 在想象中把态矢$\left| \alpha \right\rangle$复制N份；

* 取出第一个$\left| \alpha \right\rangle$，测量A，得到$a_1$，但一旦完成测量，物理系统就被改变了，成为$\left| a_1 \right\rangle$，所以我们无法再继续测量了；

* 取出第二个$\left| \alpha \right\rangle$测量A，得到$a_2$，依次得到$a_3, a_4, ...$

* 当N足够大时，$\frac{\sum\limits_{i} a_i}{N}$收敛，这个值就是A的期望值。

这样操作，得到的系综叫纯系综，因为它就对应某个确定的态矢量$\left| \alpha \right\rangle$。

### 混合系综

统计物理需要混合系综，即我们要研究的物理系统处在某个热力学分布中，$w_1$比例处于$\left| \alpha_1 \right\rangle$, $w_2$比例处于$\left| \alpha_2 \right\rangle$，...，并且满足：

\begin{equation}
\sum_n w_n =1.
\end{equation}

对混合系综，力学量$A$的平均值是：

\begin{equation}\label{statistic average}
[A] = \sum\limits_n w_n \left\langle a_n
\right| A \left| a_n \right\rangle.
\end{equation}

这里涉及两次平均，$\left\langle \alpha_n \right| A \left| \alpha_n \right\rangle$是量子力学平均，$\sum\limits_n ... $与系综分布有关，是热力学平均。

如何表达混合系综是个问题，比如我们无法把它表示为传统的波函数按线性迭加因子相加的形式：

\begin{equation*}
\psi = c_1 \psi_1 + c_2 \psi_2
\end{equation*}

因为这样写，暗含着$\psi_1$和$\psi_2$之间的相位差就固定了，或者说$\psi_1$和$\psi_2$是相干的。

我们把上式改写为：

\begin{equation*}
\psi = c_1 \psi_1 + c_2 e^{i \theta} \psi_2
\end{equation*}

这里引入了$\psi_2$和$\psi_1$之间的相位差$\theta$，如果说$\psi_1$, $\psi_2$完全不相干，就意味着$\theta$是个随机数，在$[0, 2\pi]$区间里等几率地随机取值。为了书写的方便，以下我们假设$c_1$, $c_2$都是实数。

计算力学量$A$的期望值：

\begin{equation*}
[A] = c_1^2 A_1 + c_2^2 A_2 + c_1 c_2 e^{i \theta} \left\langle \psi_1 | A | \psi_2 \right\rangle + c.c. 
\end{equation*}

这里$c.c.$表示复共轭，$e^{i \theta}$平均而言为0，因此：

\begin{equation*}
[A] = c_1^2 A_1 + c_2^2 A_2
\end{equation*}

我们令$c_1^2 = w_1$, $c_2^2 = w_2$，就得到混合系综平均的定义式(\ref{statistic average})。

密度算符（Density operator）是朗道引入以描述统计物理的，

\begin{equation}\label{statistic operator}
\rho = \sum\limits_n \left| a_n \right\rangle w_n \left\langle a_n \right|
\end{equation}

平均值(\ref{statistic average})可改写为：

\begin{equation}
[A] = \text{Tr} (\rho A)
\end{equation}

对统计算符$\rho$求偏导$i\hbar \frac{\partial}{\partial t}$，可推出$\rho$满足的运动方程，“量子刘维方程”（Quantum Liouville Equation），

\begin{equation}\label{quantum Liouville eqs}
i\hbar \frac{\partial}{\partial t} \rho = H \rho - \rho H = [H,
\rho].
\end{equation}

注意：和海森堡运动方程比较$i\hbar \dot a = [a, H]$，量子刘维方程在形式上差一个“负号”。

## 正则分布

对平衡态而言，$\rho$不随时间改变，因此$[H, \rho]=0$。这意味着如果$\rho$是$H$的幂函数，则$\rho$表示的态一定是平衡态。

正则分布，

\begin{equation}\label{canonical distribution}
\rho = \frac{e^{-\beta H}}{Z} = Z^{-1} e^{-\beta H}
\end{equation}

这里，$\beta = \frac{1}{k_B T}$，$Z^{-1}$是归一化因子，

\begin{equation*}
Z = \text{Tr} e^{-\beta H}
\end{equation*}

$Z$是个数，

\begin{equation*}
Z = \text{Tr} e^{-\beta H} = \sum_i \left\langle i \right| e^{-\beta H}
\left| i \right\rangle = \sum\limits_i e^{-\beta E_i}
\end{equation*}

正则系综的能量$E$，

\begin{equation*}
E = \text{Tr} (H \rho) = Z^{-1} \text{Tr} (H e^{-\beta H}),
\end{equation*}

因为$Z^{-1}$是个数，所以可提出$Tr$之前。

现在考虑正则系综的熵（entropy），

熵是不确定（或信息缺乏）的度量，假设等几率分布，几率$p$，状态数$\Gamma = \frac{1}{p}$，熵被定义为: $S = k_B \ln \Gamma = - k_B \ln p$。把这个定义推广为非等几率${p_{\lambda}}, \sum_{\lambda}
p_{\lambda}=1$分布，$S = -k_B \sum\limits_{\lambda} p_{\lambda}\ln
p_{\lambda}$。如果用密度算符表示的话，就是:

\begin{equation}\label{definition of entropy}
S = - k_B \text{Tr} (\rho \ln \rho)
\end{equation}

这里，

\begin{equation*}
\ln \rho = \ln ( Z^{-1} e^{-\beta H} ) = \ln e^{-\beta H} - \ln Z =
-\beta H - \ln Z,
\end{equation*}

那么，

\begin{equation*}
S = - k_B \text{Tr} (\rho \ln \rho) = k_B \text{Tr} [ \rho (\beta H + \ln Z) ].
\end{equation*}

第一项: $k_B \beta \text{Tr} (\rho H) = \frac{1}{T} E$,

第二项: $k_B \text{Tr} [ \rho \ln Z  ]$, 考虑到$\text{Tr} (\rho) = 1$, 这一项是: $k_B \ln Z$.

因此,

\begin{equation*}
S = \frac{E}{T} + k_B \ln Z
\end{equation*}

定义自由能（Free energy），

\begin{equation}\label{definition of free energy}
F = - k_B T \ln Z = - \beta^{-1} \ln Z,
\end{equation}

对正则系综，$E$，$S$，$F$存在关系:

\begin{equation}\label{relation ESF}
F = E - TS
\end{equation}

正则系综代表与热库接触，允许能量交换，保持温度固定而达到的平衡态。

假如不仅允许能量交换，还允许系统和热库交换粒子，保持温度$T$和化学势$\mu$固定，这样达到的平衡态，就是巨正则分布（Grand
canonical distribution）了，密度算符是:

\begin{equation}\label{density operator: GCE}
\rho_G = Z_G^{-1} e^{-\beta (H - \mu N)}
\end{equation}

这里$H, N$是算符, $Z_G^{-1}$是巨配分函数:

\begin{equation*}
Z_G = Tr e^{-\beta (H - \mu N)}
\end{equation*}

利用: $E = Tr (\rho H)$, $N = Tr (\rho N)$, 可证明:

\begin{equation*}
-k_B T \ln Z_G = \Omega = E- TS - \mu N
\end{equation*}

这里$\Omega(T,V,\mu)$是“广势函数”。由$\Omega$，我们可求出$S$, $P$, $N$:

\begin{eqnarray*}
% \nonumber to remove numbering (before each equation)
  S &=& -\left( \frac{\partial \Omega}{\partial T}\right)_{V, \mu} \\
  P &=& -\left( \frac{\partial \Omega}{\partial V} \right)_{T, \mu} \\
  N &=& -\left( \frac{\partial \Omega}{\partial \mu} \right)_{T, V}
\end{eqnarray*}

## 热力学关系

$T$, $P$, $\mu$这样的物理量叫强度量, $S$, $V$, $N$这样的量叫广延量。能量的变化$dE$可表示为,

\begin{equation}\label{dE relation}
dE = TdS - P dV + \mu dN,
\end{equation}

$-PdV$项中的负号意味着，体积增大，系统对外作功，系统内能E是减小的。公式(\ref{dE relation})表示，$E$是$S$, $V$, $N$的函数，即$E(S, V, N)$，由公式(\ref{dE relation}), 我们还可得到:

\begin{eqnarray*}
% \nonumber to remove numbering (before each equation)
  T &=& \left( \frac{\partial E}{\partial S} \right)_{V,N}  \\
  P &=& - \left(\frac{\partial E}{\partial V} \right)_{S,N} \\
  \mu &=& \left(\frac{\partial E}{\partial N} \right)_{S,V}
\end{eqnarray*}

现在我们作勒让德变换, 努力把$S$, $V$, $N$宗量变为, 比如$T$, $V$, $N$宗量.

\begin{equation*}
F = E - TS
\end{equation*}

则, $d F = d E - T dS - S dT = -S dT - P dV + \mu dN$, $F$是$T$, $V$, $N$的函数, 记为: $F(T, V, N)$, 求偏微分可得:

\begin{eqnarray*}
% \nonumber to remove numbering (before each equation)
  S &=& - \left( \frac{\partial F}{\partial T} \right)_{V,N} \\
  P &=& - \left( \frac{\partial F}{\partial V} \right)_{T,N} \\
  \mu &=& \left( \frac{\partial F}{\partial N} \right)_{T,V}
\end{eqnarray*}

继续作勒让德变换, 变成$T$, $V$, $\mu$宗量的,

\begin{equation*}
\Omega(T,V,\mu) = F - \mu N = E - TS - \mu N.
\end{equation*}

则, $d \Omega = -S dT - P dV - N d\mu$, 由此式求偏微分就得到$S$, $P$, $N$.

## 练习

* 证明：$[A] = \text{Tr} \rho A$

证：

\begin{equation}
\text{Tr} \rho A = \sum_i (\rho A)_{ii} = \sum_{ij} \rho_{ij} A_{ji} 
\end{equation}

这里：

\begin{equation}
A_{ji} = \left\langle j | A | i \right\rangle
\end{equation}

代入可得：

\begin{equation}
\text{Tr} \rho A = \sum_{ij} \sum_n   \left\langle i  | n \right\rangle w_n \left\langle n | j \right\rangle \left\langle j | A | i \right\rangle
\end{equation}

即：

\begin{equation}
\text{Tr} \rho A =  \sum_n   w_n \left\langle n | A | n \right\rangle
\end{equation}

QED

* 证明：$\text{Tr} \rho =1$


* 推导密度算符随时间的演化，即量子刘维方程（Quantum Liouville equation），

\begin{equation}
i \hbar \frac{\partial }{\partial t } \rho = [H, \rho]
\end{equation}

提示：利用薛定谔方程和，$d (uv) = (du) v + u dv$

## 阅读

* J. J. Sakurai, Modern Quantum Mechanics, $\S$ 3.4;
