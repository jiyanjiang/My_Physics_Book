# 相干干涉光的透射率




等比数列求和：

$$ 1 + e^{i \delta } + e^{i 2 \delta } + ... + e^{i N \delta } $$

Transmission

$$\left| \frac{1-e^{iN\delta}}{1-e^{i \delta}} \right|^2=\left| \frac{1- \cos N \delta - i \sin N \delta }{1 -  \cos \delta - i \sin \delta } \right|^2 = \frac{ (1- \cos N\delta)^2 + \sin^2 N \delta }{(1-\cos \delta)^2 + \sin^2 \delta  } $$

use:

$$ \cos \delta = \cos^2 \frac{\delta}{2} - \sin^2 \frac{\delta}{2} $$

$$ 1-\cos\delta = \cos^2 \frac{\delta}{2}+ \sin^2 \frac{\delta}{2} - \cos^2 \frac{\delta}{2}+ \sin^2 \frac{\delta}{2} = 2 \sin^2 \frac{\delta}{2}$$

Then

$$ (1-\cos\delta)^2 = 4 \sin^4 \frac{\delta}{2} $$

$$ \sin^2 \delta = 4 \sin^2 \frac{\delta}{2} \cos^2 \frac{\delta}{2} $$

$$ (1- \cos\delta )^2+ \sin^2 \delta = 4 \sin^2 \frac{\delta}{2} \left(\sin^2 \frac{\delta}{2} + \cos^2 \frac{\delta}{2}\right) = 4 \sin^2 \frac{\delta}{2} $$

Hence

$$ \left| \frac{1-e^{iN\delta}}{1-e^{i \delta}} \right|^2 = \frac{\sin^2 \frac{N \delta}{2}}{\sin^2 
\frac{\delta}{2}} $$


![截屏2020-02-17下午8.59.24.png-49.8kB][1]


phase factor gained in transmission

$$e^{i k x} = e^{i \frac{2 \pi x}{\lambda}} = e^{i \frac{2 \pi n l}{\lambda}}$$


$$ a_1 = e^{i \frac{2\pi n l }{\lambda}} \sqrt{(1- R)^2 e^{- \alpha l}}   $$

$$ q = e^{ i \frac{4 \pi n l }{\lambda} } \sqrt{R^2 e^{- 2 \alpha l}} $$

define: $\Phi = \frac{4 \pi n l }{\lambda} $

$$\frac{(1-R)e^{- \alpha l /2}e^{i\Phi/2} } {1 - R e^{- \alpha l } e^{i \Phi}} = \frac{(1-R)e^{- \alpha l /2} (\cos \Phi/2 + i \sin \Phi/2)}{1 - R e^{- \alpha l }(\cos \Phi + i \sin \Phi)} $$


$$\left| \frac{a_1}{1 - q} \right|^2 = ?$$

numerator: $(1-R)^2 e^{- \alpha l }$

denominator:

$\left| 1 - R e^{- \alpha l }\cos \Phi - i R e^{- \alpha l }\sin \Phi \right|^2 \\ = (1 - R e^{- \alpha l }\cos \Phi)^2 + (R e^{- \alpha l }\sin \Phi)^2 \\ = 1 - 2 R e^{-\alpha l }\cos \Phi  + R^2 e^{- 2 \alpha l }$

Transmission:

$$T = \frac{(1-R)^2 e^{- \alpha l }}{ 1 - 2 R e^{-\alpha l }\cos \Phi  + R^2 e^{- 2 \alpha l } } $$





  [1]: http://static.zybuluo.com/jiyanjiang/fwjtdv44s9sir5y6pee04res/%E6%88%AA%E5%B1%8F2020-02-17%E4%B8%8B%E5%8D%888.59.24.png
