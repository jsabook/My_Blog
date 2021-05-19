---
title: research
date: 2021-03-08 23:23:15

---

------



# CVPR2020

[CVPR论文获奖名单](http://cvpr2020.thecvf.com/node/817)



#### 1.最佳论文奖

- 论文链接：https://arxiv.org/abs/1911.11130
- 代码地址：https://github.com/elliottwu/unsup3d
- demo 地址：http://www.robots.ox.ac.uk/~vgg/blog/unsupervised-learning-of-probably-symmetric-deformable-3d-objects-from-images-in-the-wild.html

​	来自牛津大学的吴尚哲、Christian Rupprecht、Andera Vedaldi 获得了最佳论文奖，获奖论文是《Unsupervised Learning of Probably Symmetric Deformable 3D Objects from Images in the Wild》

​	这项研究提出了一种基于原始单目图像学习 3D 可变形物体类别的新方法，且无需外部监督。

![](https://image.jiqizhixin.com/uploads/editor/311e2326-377a-4f25-be10-ae42c25af887/640.jpeg)

​	该方法基于一个自编码器，它将每张输入图像分解为深度、反射率、视点和光照（将这四个组件结合起来即可重建输入图像）。该模型在训练过程中仅利用重建损失，未使用任何外部监督。

​	为了在不使用监督信号的前提下将这些组件分解开，研究人员利用了很多物体类别所具备的属性——对称结构。该研究表明，对光照进行推理可以帮助我们利用物体的底层对称性，即便由于阴影等因素造成物体外观看起来并不对称也没有关系。

​	此外，该研究还使用模型其他组件以端到端的方式学得对称概率图，并借助对该概率图的预测对可能并不对称的物体进行建模。

![](https://image.jiqizhixin.com/uploads/editor/289ee2f0-4160-46c2-a445-17c8ff6a20a8/640.gif)

​	实验表明，该方法可以准确恢复单目图像中人脸、猫脸和车辆的 3D 形状，且无需任何监督或先验形状模型。相比于利用 2D 图像对应监督的另一种方法，该方法在基准数据集上的性能更加优越。



{% pdf https://arxiv.org/pdf/1911.11130.pdf %}

#### 2.最佳学生论文奖

- 论文链接：https://arxiv.org/pdf/1911.06971.pdf

- 代码地址：https://github.com/czq142857/BSP-NET-original

  

​    来自加拿大西蒙弗雷泽大学和谷歌的 Zhiqin Chen 等人获得了最佳学生论文奖，获奖论文是《BSP-Net: Generating Compact Meshes via Binary Space Partitioning》。

​	多边形网格在数字 3D 领域中无处不在，但它们在深度学习革命中仅扮演了次要角色。学习形状生成模型的领先方法依赖于隐函数，并且只能在经过昂贵的等值曲面处理过程后才能生成网格。为了克服这些挑战，该研究受计算机图形学中经典空间数据结构 Binary Space Partitioning（BSP）的启发，来促进 3D 学习。

![](https://image.jiqizhixin.com/uploads/editor/614428b1-e3c7-44a5-8b57-9280882b5be2/640.png)

​	BSP 的核心部分是对空间进行递归细分以获得凸集。利用这一属性，研究者设计了 BSP-Net，该网络可以通过凸分解来学习表示 3D 形状。重要的是，BSPNet 以无监督方式学得，因为训练过程中不需要凸形分解。

![](https://image.jiqizhixin.com/uploads/editor/1c21b26b-9cfa-4a51-9aeb-6e5c7e63a9b4/640.png)

​	该网络的训练目的是，为使用基于一组平面构建的 BSPtree 获得的一组凸面重构形状。经过 BSPNet 推断的凸面可被轻松提取以形成多边形网格，而无需进行等值曲面处理。生成的网格是紧凑的（即低多边形），非常适合表示尖锐的几何形状。此外，它们一定是水密网格，并且可以轻松参数化。该研究还表明，BSP-Net 的重构质量和 SOTA 方法相比具备竞争力，且它使用的原语要少得多。

{% pdf https://arxiv.org/pdf/1911.06971.pdf %}

#### 3.最佳学生论文荣誉提名奖

- 论文链接：https://arxiv.org/pdf/2003.08325.pdf



​	本次获得最佳学生论文荣誉提名的是德国马普所和 Facebook Reality Labs 合作的文章《DeepCap: Monocular Human Performance Capture Using Weak Supervision》，第一作者为马普所的 Marc Habermann。

​	在这篇论文中，研究者提出了一种新颖的单目密集人体表现捕捉深度学习方法。该方法采用一种基于多视图监督的弱监督方法进行训练，并且完全不需要利用 3D ground truth 标注来训练数据。此外，网络架构基于的两个独立网络将任务分解为姿态估计和非刚性表面变形步骤。大量的定性和定量评估表明，研究者提出的方法在质量和鲁棒性两方面优于当前 SOTA 方法。

​	该方法的流程图如下所示，其中以单个分割图像作为输入。首先，通过将稀疏多视图 2D 关节检测作为弱监督，研究者训练姿态网络 PoseNet 来预测关节角度和相机相对旋转；其次，研究者训练变形网络 DefNet 来返回嵌入图旋转和平移参数，从而考虑到非刚性变形。此外，为了训练变形网络 DefNet，研究者将多视图 2D 关节检测和剪影用于监督。

![](https://image.jiqizhixin.com/uploads/editor/d8367866-f3e2-489b-aa76-62a1cd73dd94/640.png)


​	下图展示了该方法在各种服装款式、姿态和环境的野外测试序列（in-the-wild sequence）上的定性结果。由效果图可见，研究者的重建不仅能够精准地与输入图像重合，而且在任意 3D 视图下也有不错的效果。

![](https://image.jiqizhixin.com/uploads/editor/1a05b612-e546-4529-bfd5-d77b15fe23d6/640.png)

{% pdf https://arxiv.org/pdf/2003.08325.pdf %}





#### 参考：

[1]   机器之心文章  [CVPR 2020华人一作包揽最佳论文、最佳学生论文，中国作者占39%，清华高居第一](https://www.jiqizhixin.com/articles/2020-06-17)