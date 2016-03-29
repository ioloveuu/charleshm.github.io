---
published: true
author: Charles
layout: post
title:  "漫谈行列式"
date:   2016-03-27 9:30
categories: 线性代数
---

因为不少公司的机器学习（数据挖掘）的笔试题中都涉及到行列式的求解，一时心血来潮，深挖了下。

#### 几何意义
一个解释是行列式就是矩阵的行（列）向量所构成的**超平行多面体**的有向面积或有向体积[^1]；

另一个解释是矩阵A的行列式就是**线性变换** A 下的图形面积或体积的**伸缩因子**。

这两个几何解释一个是**静态**的体积概念，一个是**动态**的变换比例概念。但具有相同的几何本质，因为矩阵 A 表示的（矩阵向量所构成的）几何图形相对于单位矩阵 E 的所表示的单位面积或体积而言，伸缩因子本身就是矩阵A表示的几何图形的面积或体积。

比如，一个 $3\times 3$ 阶的行列式就是其行向量或列向量所张成的平行六面体的有向体积。

![此处输入图片的描述][1]


  [1]: http://7xjbdi.com1.z0.glb.clouddn.com/3_det.png
  
  [^1]: [行列式的几何意义](http://www.cnblogs.com/AndyJee/p/3491487.html)