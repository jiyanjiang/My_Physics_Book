# 量子计算 QUANTUM COMPUTING Read Log

@ianwest

## 重点

1. 量子计算要想大规模走向应用，必须解决量子纠错的问题。
2. 量子纠错太难了，短期实现很难。
3. 短期，我们必须学会与错误共存。

短期，量子计算走向应用的突破点在：

1. 错误缓解技术，[Quantum Error Mitigation](https://arxiv.org/abs/2210.00921)
2. 中等有噪声的量子计算（NISQ, Noisy Intermediate-Scale Quantum Computing），[Quantum Computing in the NISQ era and beyond
](https://arxiv.org/abs/1801.00862)


## 量子计算的由来

1984, [Quantum Mechanical Computers](https://opn-web-afd-d3bfbkd5bcc5asbs.z02.azurefd.net/opn/media/images/pdfs/11557/11557_23417_110730.pdf)




## 量子计算机的硬件实现

1. 超导量子计算: Transmon 超导传输子量子比特
2. 光量子计算：光子
3. 离子阱量子计算：带电离子中的两个能级
4. 中性原子计算：里德堡原子中的两个能级
5. 拓扑量子计算：超导纳米线中的马约拉纳零能模（MZM）
6. 量子退火机：严格说不算量子计算机，超导磁通量子比特 Fluxon

### 光量子计算

- [Universal photonic quantum processor sets new size record
](https://physicsworld.com/a/universal-photonic-quantum-processor-sets-new-size-record/)

- Company: [QuiX](https://www.quixquantum.com/), Photonic Quantum Computing

- 光量子计算机DIY: [DIY Quantum Computing: How I Got Started Building Quantum Circuits](https://turbofuture.com/computers/build-quantum-computer)

Comments: 根据不确定关系，具有单一频率，且具有确切光子数的量子态是不可能存在的。

> The Heisenberg uncertainty principle dictates that a state with an exact number of photons of a single frequency cannot be created.

$$\Delta E \Delta t \ge h $$

我们平时说的单光子源指的是一个有效的“单光子”态。

> a single-photon source gives rise to an effectively one-photon number state.



### 中性原子量子计算

- 光镊（optical tweezer）使中性原子通过激光聚焦被束缚在空间指定位置；
- 中性原子一般使用里德堡原子，里德堡原子钟的两个能级构成量子比特；
- 光镊移动中性原子使不同量子比特发生耦合，耦合机制为电偶极矩相互作用(dipole-dipole interaction)；
- 如此实现的双量子比特门保真度高，能实现更多连接数。

是实现规模化量子纠错的最新选择，大有后来居上的趋势。

2022-01: [](https://www.mittrchina.com/news/detail/10251), [Vibrating atoms make robust qubits](https://news.mit.edu/2022/vibrating-atoms-qubits-0126)

> 该研究团队利用激光干涉形成二维网状势阱，捕获了大约 400 对中性钾-40 冷原子，制造了一种光学晶格结构，并成功地在每个原子对中观测到了两种不同量子振动行为的叠加态，发现了全新的量子比特


## 评价一台量子计算机的指标

量子体积, [Quantum Volume: A Yardstick To Measure The Performance Of Quantum Computers](https://www.forbes.com/sites/moorinsights/2019/11/23/quantum-volume-a-yardstick-to-measure-the-power-of-quantum-computers/
)

量子体积与如下因素有关：

1. 量子比特数
2. 量子比特的连接性，假设各个量子比特互相充分连接，就有更强的处理信息的能力
3. 量子线路的深度


## 量子优越性（Quantum supremacy）

2012, Preskill

2019, 谷歌，量子随机线路采样

- Google

2019, [Quantum supremacy using a programmable superconducting processor](https://www.nature.com/articles/s41586-019-1666-5)

2022, 普通计算机也能打败谷歌的量子计算机

- [Ordinary computers can beat Google’s quantum computer after all](https://www.science.org/content/article/ordinary-computers-can-beat-google-s-quantum-computer-after-all) 

arXiv [Solving the sampling problem of the Sycamore quantum circuits](https://arxiv.org/abs/2111.03011)

- [Google’s ‘quantum supremacy’ usurped by researchers using ordinary supercomputer](https://techcrunch.com/2022/08/05/googles-quantum-supremacy-usurped-by-researchers-using-ordinary-supercomputer/)

1. 随机线路采样
2. 玻色采样

## 量子应用 Application

大概三个层次

1. 模拟：量子化学，催化，材料设计，磁性，量子多体……

- [Quantum Chemistry in the Age of Quantum Computing](https://arxiv.org/abs/1812.09976)

目前的量子计算机可以被认为是粒子数$\sim 10^2 - 10^3$的量子多体系统，如果类比的话，目前的神经网络是基于经典伊辛模型的，而量子计算机是可以基于量子海森堡模型的。



2. 设计：蛋白质折叠，药物设计



3. 优化：


4. 大数据/机器学习


## 量子纠错（Quantum Error Correction）

## 人物 People

Stephen Wiesner (1942 – August 12, 2021),
https://en.wikipedia.org/wiki/Stephen_Wiesner

Charles H. Bennett, (1943- )
https://en.wikipedia.org/wiki/Charles_H._Bennett_%28physicist%29

Dr. Chetan Nayak
https://www.microsoft.com/en-us/research/people/cnayak/


### 信息与熵 Information and Entropy

- Maxwell's demon

- Landauer's Theorem

- Feynman’s Lecture on Computing
[Three Papers Related to Quantum Computing](https://jackkrupansky.medium.com/feynmans-three-papers-related-to-quantum-computing-dd6f9847e6ad)





Thermodynamics of information
https://www.nature.com/articles/nphys3230

### 统计物理传承

玻尔兹曼/艾伦菲斯特
海森堡/Hans Bethe/David J. Thouless

### IBM

- Quantum Error suppression 错误抑制
- Quantum Error Mitigation 错误缓解
- Quantum Error Correction 量子纠错

[What’s the difference between error suppression, error mitigation, and error correction?](https://www.ibm.com/quantum/blog/quantum-error-suppression-mitigation-correction)

[Quantum Error Mitigation](https://arxiv.org/abs/2210.00921)


### Google


### 微软


马约拉纳零能模（MZM）

马约拉纳零能模的非阿贝尔统计及其在拓扑量子计算的应用
https://www.researching.cn/ArticlePdf/m30001/2020/69/11/20200812.pdf


## 行业/公司 Companies

https://www.riverlane.com/

Riverlane was founded in 2016 by Steve Brierley, a senior research fellow in computational mathematics at the University of Cambridge. At that time, the majority view in the global quantum computing community was that 'useful' quantum computing was more than 20 years away - or might never happen.

## 一般参考

https://qubit.guide/index

## Tools 工具

1. Colab, https://colab.research.google.com/
2. Jupyter Notebook, https://jupyter.org/
[Quantum mechanics lectures with QuTiP](https://qutip.org/qutip-tutorials/#lectures)

