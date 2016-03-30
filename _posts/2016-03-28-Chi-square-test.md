---
published: true
author: Charles
layout: post
title:  "卡方检验"
date:   2016-03-27 9:30
categories: 机器学习 统计学
---

![此处输入图片的描述][1]

#### $\chi^2$ 统计量

我们前面提到过，各种检验方法的差别在于计算的**检验统计量**不同。

我们先来关注下 $\chi^2$ 统计量，

$$\chi^2 = \sum \frac{(A – E)^2}{E} \tag{1}$$

其中 $A$ 表示实际观察次数， $E$ 表示理论观察次数（对比一下 $\chi^2$ 分布）。

> $\chi^2$ 是度量实际观察次数与理论次数偏离程度的一个统计量。

 - $\chi^2$ 越小，表明实际观察次数与理论次数越接近
 - $\chi^2=0$ 表示两者完全吻合
 - $\chi^2$ 越大，表示两者相差越大


----------


#### 适合性检验

 


  [1]: http://7xjbdi.com1.z0.glb.clouddn.com/Chi_square_test.png