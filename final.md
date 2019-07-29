## 布朗运动与 DNA 随机行走

#### 摘要

参考文献《布朗运动100年》，本文首先简要介绍一下布朗运动与随机行走在数学上的联系。接着采用数值模拟的方法来详细说明这一点。然后就文献中提到的 DNA Walker 现象进行数值计算。

### 扩散方程与随机行走

以下内容来自参考文献[]，这里只是做一下简要回顾。著名的扩散方程具有以下形式，
$$
\frac{\partial \rho}{\partial t}=D \frac{\partial^{2} \rho}{\partial x^{2}}
$$
假定在 $t =0$ 时刻粒子位于 $x =0$ 处，即 $\rho(x , 0) = \delta ( x )$，扩散方程的解是：
$$
\rho(x, t)=\frac{1}{\sqrt{4 \pi D t}} e^{\frac{x^{2}}{4 D t}},
$$
即粒子的密度遵从高斯分布。对于固定的时刻 $t$ ，有，
$$
\langle x\rangle= 0, \quad\left\langle x^{2}\right\rangle= 2 D t,
$$
可以验证 $\displaystyle{\int_{-\infty}^{\infty}\rho(x,t) \mathrm{d}\,t=1}$。这样就得到了扩散长度公式，
$$
\sqrt{\left\langle x^{2}\right\rangle}=\sqrt{2 D t},
$$
这里出现了著名的爱因斯坦的 $\frac{1} {2} $ 指数。