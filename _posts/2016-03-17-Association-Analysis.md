---
published: true
author: Charles
layout: post
title:  "关联分析"
date:   2016-03-17 9:30
categories: 数据挖掘
---

**关联规则**反映一个事物与其它事物之间的相互依存性和关联性。如果两个或者多个事物之间存在一定的关联关系，那么，其中一个事物发生就能够预测与它相关联的其它事物的发生。比如经典的购物篮事务(market basket transaction)，通过顾客放入购物篮中商品之间的**同现关系**(co-occurrence)来分析顾客的购买习惯，实现商品的交叉销售和推荐。 

![此处输入图片的描述][1]

从上面的数据中我们可以提取如下的规则：

$$\{ \text{尿布} \} \rightarrow \{ \text{啤酒} \} $$

这表明尿布和啤酒的销售关系存在很强的联系，因为许多购买尿布的顾客也购买了啤酒，零售商可以利用这类规则，帮助他们发现新的商机。

那我们如何提取出这样的关联规则呢？

#### 基本概念
- 项集，支持度计数，频繁项集

![此处输入图片的描述][2]

- 关联规则，支持度，置信度

![此处输入图片的描述][3]

举个简单例子，熟悉下公式。

考虑关联规则： $\{Milk,Diaper\} \Rightarrow Beer$，

$$\begin{align*}
s & = \frac{\sigma(Milk,Diaper,Beer)}{|T|} = \frac{2}{5} = 0.4\\
c & = \frac{\sigma(Milk,Diaper,Beer)}{\sigma(Milk,Diaper)} = \frac{2}{3} = 0.67
\end{align*}$$

![此处输入图片的描述][4]


  [1]: http://7xjbdi.com1.z0.glb.clouddn.com/2016-03-21_195111.png?imageView2/2/w/400
  [2]: http://7xjbdi.com1.z0.glb.clouddn.com/2016-03-21_212028.png
  [3]: http://7xjbdi.com1.z0.glb.clouddn.com/2016-03-21_212722.png
  [4]: http://7xjbdi.com1.z0.glb.clouddn.com/2016-03-21_213839.png