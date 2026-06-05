# 为什么需要引入 $q_t$？

论文想解释两个典型事实：

$$
p^e_t \downarrow,
\qquad
\frac{i^e_t}{Y_t}\uparrow
$$


**标准增长模型无法同时解释这两个现象。**

---

# 1. 不加入 $q_t$：无法解释什么？

在标准增长模型中，设备投资和其他投资一样，都是由最终品一比一转化而来：

$$
Y_t = C_t + I_t
$$

设备资本积累方程为：

$$
K_{t+1} = (1-\delta)K_{t}+I_t
$$

因此，设备相对于消费品的价格是固定的：

$$
p^i_t = p^{c}_t
$$



在平衡增长路径上，设备资本和产出以同一速度 $g$ 增长：

$$
K_{t+1}=gK_{t}= (1-\delta_e)K_{t}+I_t
$$

代入资本积累方程，由于平衡增长路径中 $K_t/Y_t$ 是常数：




$$
\frac{I_t}{Y_t}
=
(g-1+\delta_e)\frac{K_{t}}{Y_t} =
\text{constant}
$$



---

# 3. 加入 $q_t$：为什么可以解释？

论文引入投资品特定技术进步：

$$
K_{t+1}
=

(1-\delta)K_{t}
+
q_t I_t
$$

其中，$q_t$ 表示一单位最终品可以转化为多少有效设备：

$$
p^i_t = \dfrac{p^{c}_t}{q_t}, \qquad \frac{I_t}{Y_t} = (g-1+\delta)\frac{q_t K_{t}}{Y_t}
$$

---

# 设备价格与设备投资负相关：为什么需要 (q_t)？

原文中的高频事实是：

$$
p^e_t \downarrow
\quad \text{时，通常有} \quad
i^e_t \uparrow
$$

即：

$$
\operatorname{corr}(p^e_t,i^e_t)<0
$$

问题是：标准模型如果不加入 (q_t)，很难解释这种负相关。

---

# 1. 不加入 (q_t)：为什么解释不了？

在不加入 (q_t) 的标准模型中，设备投资由最终品一比一转化而来：

$$
K_{e,t+1}
=========

(1-\delta_e)K_{e,t}
+
i^e_t
$$

资源约束为：

$$
Y_t=C_t+i^e_t+i^s_t
$$

这意味着设备相对价格固定为：

$$
p^e_t=1
$$

因此，模型本身没有设备相对价格波动：

$$
\Delta p^e_t=0
$$

既然 (p^e_t) 不变，就无法解释：

$$
\operatorname{corr}(p^e_t,i^e_t)<0
$$

也就是说，不加入 (q_t) 时，模型里根本没有一个机制让设备价格下降。

如果强行用“投资需求上升”解释设备投资增加，那么通常得到的是价格和投资正相关。设设备需求为 (D)，供给为 (S)。当投资需求增强时，需求曲线右移：

$$
D \uparrow
$$

均衡结果通常是：

$$
p^e_t \uparrow,
\qquad
i^e_t \uparrow
$$

所以需求侧解释对应的是：

$$
\operatorname{corr}(p^e_t,i^e_t)>0
$$

这和原文事实相反。

因此，不加入 (q_t) 时，标准模型无法解释：

$$
p^e_t \downarrow,
\qquad
i^e_t \uparrow
$$

也就无法解释设备价格和设备投资的负相关。

---

# 2. 加入 (q_t)：为什么能解释？

加入投资品特定技术进步后，设备资本积累方程变为：

$$
K_{e,t+1}
=========

(1-\delta_e)K_{e,t}
+
q_t i^e_t
$$

其中，(q_t) 表示一单位最终品可以转化为多少有效设备：

$$
1 \text{ unit final good}
\longrightarrow
q_t \text{ units effective equipment}
$$

因此，设备相对价格为：

$$
p^e_t=\frac{1}{q_t}
$$

当投资品技术进步提高时：

$$
q_t \uparrow
$$

设备相对价格下降：

$$
p^e_t=\frac{1}{q_t}\downarrow
$$

同时，同样一单位设备投资支出可以形成更多有效设备：

$$
q_t i^e_t \uparrow
$$

这会刺激企业增加设备投资。因此可以得到：

$$
q_t \uparrow
\quad \Rightarrow \quad
p^e_t \downarrow,
\qquad
i^e_t \uparrow
$$

于是：

$$
\operatorname{corr}(p^e_t,i^e_t)<0
$$

所以，引入 (q_t) 后，设备价格和设备投资负相关可以被解释为：

$$
\text{投资品技术进步}
\Rightarrow
\text{设备更便宜}
\Rightarrow
\text{设备投资增加}
$$

核心直觉是：

**不加入 (q_t) 时，设备价格没有变化机制；加入 (q_t) 后，设备技术进步同时带来价格下降和投资上升，因此可以解释负相关。**
