# 从函数到微分

## 函数

最简单的函数

$$y = x$$

$x$: 自变量；$y$: 因变量(因之而变的量)。

如何理解函数？

1.列表

N | x | y
--- | --- | ---
1 | 0 | 0
2 | 1 | 1
3 | 2 | 2
4 | 3 | 3
... | ... | ...

第一个点是(0,0)；第二个点是(1,1)；第三个点是(2,2)……可以一直这么罗列下去。 

2.画图

横轴是$x$轴，与之垂直是$y$轴；$x$轴与$y$轴相交，交点是原点O(0,0)。

$x$轴，自左向右，是有个方向的。原点的左边是负数，原点的右边是正数。

$y$轴，自下向上，也是有方向的。原点之上是正数，原点之下是负数。

在这个$x-y$平面上，任何一个点P都有$x$的取值和$y$的取值，点P用($x,y$)表示；

经过点P($x,y$)，平行于$y$轴做一条平行线，与$x$轴交于点A，A的坐标是($x,0$)。

经过点P，平行于$x$轴做一条平行线，与$y$轴交于点B，B的坐标是($0,y$)

<img width="298" alt="O-xy坐标系和点P" src="https://user-images.githubusercontent.com/6512579/180114650-c0bdc9e1-b776-4aec-ac70-ee80ba5415c7.png">


现在$y=x$可表示为下图：

<img width="255" alt="y=x 是一条直线" src="https://user-images.githubusercontent.com/6512579/180114785-5081935a-1a8f-4c8c-a7f3-0ac8211f1d5c.png">


我们发现$y=x$在平面上可表示为一条直线。

对直线而言，两个点，比如O(0,0)和A(1,1)就可以确定一条直线。

更进一步的例子，是函数: 

$$y=2x$$

模仿以上研究步骤，我们先列表：

N | $x$ | $y$
--- | --- | ---
1 | 0 | 0
2 | 1 | 2
3 | 2 | 4
…… | …… | ……

然后作图，$y=2x$也是一条直线，两个点就可以画出这条直线。

<img width="289" alt="y=2x，也是一条直线" src="https://user-images.githubusercontent.com/6512579/180114903-d809fad4-639c-4c74-9324-37f26202c261.png">


比较$y=x$和$y=2x$，我们发现$y=2x$比$y=x$“陡峭”。

更一般意义下，我们研究

$$y=kx$$

这也是一条直线。

假设$k>0$，我们发现$k$越大，这个直线就越陡峭，因此我们称$k$为斜率。

<img width="279" alt="y=kx, k越大越陡峭" src="https://user-images.githubusercontent.com/6512579/180115129-7ff16965-aa83-4b69-81fc-ddf7040da969.png">


两点可以确定一条直线，我们选原点O(0,0)为其中一点，另一点是如图的A点，假设A点的坐标是($b,a$)；经过A点平行于$y$轴做到$x$轴的垂线，与$x$轴交于B，B点的坐标是($b,0$)。

现在我们得到了一个直角三角形$OBA$

假设$\angle AOB = \alpha$，$\alpha$相对的边AB叫“对边”，对边的长度是$AB=a$，另外一条直角边OB叫“邻边”，邻边的长度是$OB=b$。

那么斜率$k$等于什么呢？

回到函数

$$y=kx$$

A：$(b,a)$是$y=kx$上的一点，因此

$$a = k b$$

斜率是：

$$k = a \div b = \frac{a}{b}$$

我们单独看$\triangle AOB$

<img width="192" alt="直角三角形AOB" src="https://user-images.githubusercontent.com/6512579/180115248-f76f66e5-c512-4c4f-a65c-a5d8f2ebd11c.png">


这是一个直角三角形；

$\angle ABO = 90^\circ $，假设$\angle AOB = \alpha$

对边AB长度为$a$，邻边OB长度为$b$，斜边$OA$长度为$c$

对直角三角形，我们有勾股定理（或毕达哥拉斯定理）

$$a^2 + b^2 = c^2$$ 

口诀：“斜边平方等于两直角边平方之和。”

对直角三角形AOB，我们可引入一系列三角函数：

### “正弦函数”是“对边比斜边”

$$\sin \alpha = \frac{a}{c}$$

### “余弦函数”是“邻边比斜边”

$$\cos \alpha = \frac{b}{c}$$

### 正切函数就是斜率

$$\tan \alpha = \frac{a}{b} = k$$

简单的性质：$\tan \alpha = \frac{\sin \alpha}{\cos \alpha}$

### 余切函数是正切函数的倒数

$$\cot \alpha = \frac{1}{\tan \alpha} = \frac{b}{a}$$

也可表示为：$\cot \alpha = \frac{\cos \alpha}{\sin \alpha}$

三角函数很有用，它有好多性质。比如：

$$\sin^2 \alpha + \cos^2 \alpha = 1$$

这个证明很简单，由勾股定理$a^2 + b^2 = c^2$很容易证出来。

## 幂函数

我们现在来研究更复杂点的函数，比如

$$y = x^2$$

首先列表

N | $x$ | $y$
--- | --- | ---
1 | 0 | 0
2 | 1 | $1^2 = 1$
3 | 2 | $2^2 = 4$
4 | 3 | $3^2 = 9$
…… | …… | ……

然后画图，

<img width="310" alt="这是一条曲线" src="https://user-images.githubusercontent.com/6512579/180115437-6d35112f-5d0d-4cd3-b5d6-f30495ee2d1b.png">


我们发现$y=x^2$不是一条直线，这是一条曲线，在这条曲线上每一点的斜率都不一样。

这里斜率可以理解为在每一点($x,x^2$)附近曲线的陡峭程度。

我们有没有办法把$y=x^2$的斜率随x变化的规律表达出来？

我们想了这么一个办法

<img width="315" alt="在某一点附近的陡峭程度" src="https://user-images.githubusercontent.com/6512579/180115539-80fcddc3-ac45-4631-ad0e-4c55175799a7.png">


假设A、B是$y=x^2$曲线上的两个点，这个点挨的非常近，但又没有重合。

假设A点的坐标是($x,x^2$)

B点的坐标是($x+\Delta, (x+\Delta)^2$)

这里$\Delta$是个很小很小的量，但又不为零。

经过A、B我们引一条直线，这条直线的斜率是$k$，我们就用这个$k$值来表示曲线$y=x^2$在$x$时候的斜率。

为了看清楚一些，我们把图中的直角三角形ABC放大

<img width="304" alt="把小三角形放大" src="https://user-images.githubusercontent.com/6512579/180115635-30515907-b767-412a-82b9-524d96fdb150.png">

斜率的取值是“对边除以邻边”

$$k = \frac{BC}{AC}$$

这里AC的长度是$\Delta$，$BC$的长度是

$$(x+ \Delta)^2 - x^2$$

我们首先来计算$(x+ \Delta)^2$

回忆公式$(a+b)^2 = a^2+b^2+2ab$

$$(a+b)\times(a+b) = a^2 + b^2 + ba + ab$$

口诀：“前前、后后、内内、外外”

如此算出来共4项，其中$ba=ab$（乘法的“交换律”）

因此

$$(x+ \Delta)^2 = x^2 + \Delta^2 + 2x \Delta$$

$$(x+ \Delta)^2 - x^2 = 2x \Delta + \Delta^2$$

考虑到$\Delta$很小，那么$\Delta^2$就更小了，相比于$2x\Delta$，我们忽略$\Delta^2$，现在：

$$(x+ \Delta)^2 - x^2 = 2x \Delta$$

斜率是

$$k = \frac{2x\Delta}{\Delta} =2x$$

我们现在就求出了$y=x^2$在$x$处的斜率，它是$2x$，确实是在变化的。

在微积分的语言里，我们记作

$$k = \frac{dy }{dx} = 2x$$

类似地，我们来研究函数$y=x^3$，它的斜率是多少？

<img width="332" alt="一个更进一步的例子" src="https://user-images.githubusercontent.com/6512579/180115880-3d22c273-eb4f-420a-8435-0b885bf78f46.png">


我们可类似地考虑小直角三角形ABC

<img width="314" alt="小直角三角形ABC" src="https://user-images.githubusercontent.com/6512579/180115977-a20ba38e-291f-45a3-9b12-d38cd0eb3c3d.png">

如图我们需要计算

$$(x+\Delta)^3 = ?$$

### 计算：$(a+b)^3=?$

$$(a+b)^3 = (a+b)\times (a+b)\times (a+b)$$

这本质上是一个“排列组合”的问题。

从第一个括号里随便拿出一项来，有两种可能性$a$，或$b$；

从第二个括号里随便拿出一项，也是两种可能性；

从第三个括号里随便拿出一项，还是两种可能性；

三个括号相乘，会有$2 \times 2 \times 2 = 8$项；

1：三个括号都出$a$，$a \times a \times a = a^3$，这只有一种可能。

2：三个括号中有两个$a$，一个$b$，取$a^2b$，有三种可能性，因为b可能从三个括号里的任何一个里被挑选出来。

3：三个括号里有一个$a$，两个$b$，取$ab^2$，有三种排列组合的方式。

4：三个括号都出$b$，对应$b^3$，只有一种可能。

综合以上4点，我们得到$1+3+3+1=8$项

$$(a+b)^3 = a^3 + 3a^3b + 3ab^2 + b^3$$

利用上面这个关系

$$(x+\Delta)^3 = x^3 + 3 x^2 \Delta + 3 x \Delta^2 + \Delta^3$$

$$(x+\Delta)^3 - x^3 = 3 x^2 \Delta + 3 x \Delta^2 + \Delta^3$$

上式中，考虑到$\Delta \to 0$，第二项、第三项相比于第一项是可以忽略不计的。

因此：$(x+\Delta)^3 - x^3 = 3 x^2 \Delta$

$$\frac{(x+\Delta)^3 - x^3}{\Delta} = \frac{3x^2 \Delta}{\Delta} = 3x^2$$

这意味着$y=x^3 $的导数是$3x^2$

### 计算

$(a+b)^3 = ?$

$(a+b)^n = ?$

## 形式记号

函数(function) $f(x)$ 把定义域中某个数$x$映射为值域中的某个数$f(x)$

其导数记为：

$$f'(x) =\frac{d}{d x} f(x) $$

$f'(x)$也是个函数，可称之为导函数。

## 排列组合

排列数公式(n个人中挑出m个人排队，次序有关)：

$$ A_n^m = \frac{n!}{(n-m)!} = n(n-1)(n-2)...(n-m+1) $$

组合数公式(n个人中挑出m个人的组合数，次序无关)：

$$ C_n^m = \frac{n!}{(n-m)! m!}=\frac{n(n-1)(n-2)...(n-m+1)}{m !} $$

分母中的$m!$是由于重复计算引起的，固定m个人排队，排列数是$m!$，即排列数$A_n^m$相对于组合数$C_n^m$，在选定m个人后都重复计算了$m!$种可能性。

### 排列组合练习

1. A、B、C、D、E、F六名同学，A、B二人必须排在一起的不同排法有多少种？
2. 要排一张有6个歌唱节目和4个舞蹈节目的演出节目单，任何两个舞蹈节目不得相邻，有多少不同的排法？
3. 信号兵把红旗与白旗从上到下挂在旗杆上表示信号。现有3面红旗、2面白旗，把这5面旗都挂上去，可表示不同信号的种数是多少？
4. 同室4人各写一张贺年卡，先集中起来，然后每人从中拿一张别人送来的贺年卡，则四张贺年卡的分配方式有多少种？
5. 有甲、乙、丙三项任务，甲需由2人承担，乙、丙各需由1人承担，从10人中选派4人承担这三项任务，不同的选法共有多少种？
