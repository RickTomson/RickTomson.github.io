---
layout: post
title: Daily questions and thoughts
tags: 
 - questions
 - learning process
 - conclusion
subtitle: 
date: 2020.9.13
author: Rick.T
header-img: img/post-bg-universe.jpg
catalog: true
---

7.20

今天突然想起来个问题，为啥我们想要研究cft呢？

loose掉isometric symmetry然后让他变成conformal symmetry，突然有种距离不重要，之间的夹角才重要的感觉（但是为什么这么要求呢）。另外一点就是在真实世界中存在这种具有conformal symmetry的physical system吗，我的感觉是肯定存在，因为其本身就是对isometric symmetry的loose，这样的话我们可以说后者是前者的特例，那么后者也是一种isometric symmetry，emmm，但是这样想还有一个问题，conformal symmetry除了可以选择等距外还有其他选择，怎么让物理系统有其他选择下的对称性呢？

8.4

1.我们凭什么要求H=\frac{p^2}{2m}+V在量子力学中仍然成立，i.e.，为什么作为算符这种关系仍然满足？

或许我们应该去看H和p实际上指什么，H和p其实是时空平移生成元，因此在考虑经典时空时，其有上述对应的结构。

2.fusion竟然是一个把tensor product变成direct sum的操作，震惊，需要缓一缓想想这两者的区别。还有想问在做fusion的时候应该有什么规则呢？

那个手写的老哥的lectures似乎也很值得听，等之后白天要去听一下。

8.25

又不懂了，state-operator correspondence里面好像还有好多坑，as followings:

https://physics.stackexchange.com/questions/88773/operator-state-correspondence-in-qft

star: https://mathoverflow.net/questions/16584/about-state-field-correspondence

感觉我感兴趣的解决问题的方向可能是VOA。。

9.4

1.tqft为什么是从Bord_n \rightarrow Vect_n的functor？（这里面和tensor product的结构有关）还有我们常说的分类是指什么？（我个人认为是tqft的分类，即有许多的partition functions，一个partition fuction代表了一个tqft，然后partition functions是可以被分类的）

2.量子场对应的是自由度，那么在流形上某一点处的量子场是否就是我们考虑的那一点的Hilbert space呢？

9.9

1.The quantization (or canonical quantization) of tqft? This motivates us to study algebra structure of tqft.

2.今天仍然困惑于correlation functions(or n-point functions)，参考了几个stackexchange，e.g. two-point function

$$
<\phi(x)\phi(y)>
$$

in some (wrong) sense, we can interpret it as the probability amplititude of a particle propagate from point x to point y. However, it is wrong because if we integral it, we will find the probability will divergence. But if the probability is 1, then we can say that interpretation happens to be right. We can treat it as amplititude or transition amplititude indeed, because it is just the inner product of two states. 

There are other treatments.

We can use path integral to calculate it and get following formula:

$$
\langle\mathcal{O}\rangle=\frac{1}{Z} \int \mathcal{D} \Phi \mathcal{O} \mathrm{e}^{-S_E \Phi}
$$

then we replace $\mathcal{O}$ as $\phi(x)\phi(y)$, however, we should prove latter is hermitian.. With gauge symmetry, we get ward identity. (I am doubt with this symmetry and invariant of expectation value)

Another thing is scatting amplititude, where we consider interaction in QFT, however I know nothing about it..

$$
\langle \mathcal{U_a}\mathcal{U_b}\rangle=
$$

为什么在wightman qft中，只需要有n-point functions就可以了

propagator? should the propagator satisfies probability = 1?

为什么没人疑惑$\phi(x)$不是哪个的generator？

9.20

从QFT出发，n-point correlation functions can be given by generating functions, then if we consider CFT, what are the generating functions of n-point correlation functions in CFT?

9.23

in QFT, we always have many kinds of quantum fields, such as scalar field, spinor field, etc. We know those fields represent freedoms (both spin and usual freedoms) and will be corresponding to describing specific particles, thus they have same freedoms (the exact meaning may be rep of lie alg) with particles, we ask what are particles of gauge fields (we can see gauge fields as quantum fields)? Gauge bosons? And does it limit the rep of gauge group?

与常规自由度不同，spinor在mfd会有其他的结构（spinor structure），但是这一点细想起来也有些奇怪，因为按照原始想法，mfd是spacetime，是背景，而spin应为particle (or field)或者说Hilbert space的结构，所以把spinor structure放到spacetime上还是有些奇怪，莫非spin会对spacetime make a difference？

9.28

finite group algebra的定义

首先来看一下algebra的定义，algebra $\mathfrak{g}$是一个向量空间，其上有bilinear map:$[ , ]: \mathfrak{g}\times\mathfrak{g}\rightarrow\mathfrak{g}$ which satisfies:

1.$[v,w]=-[w,v]$

2.jacob identiry



generator，algebra，group algebra和group间的关系



9.29

量子力学是没有背景的，真正的物理需要有背景（时空）.

e.g.很容易看到，在经典量子力学中，考虑一个operator动量p的时候，我们从未考虑过其随空间位置x怎么变化，而只能有其在time evolution中怎么样，因此这是没有背景的理论。



10.9

something about 拓扑简并

如果事先知道tensor product态是一类的话，而且存在简并态，那么纠缠的维度不可能是有限的（我猜的，需要一些分类的知识来解释），所以才要考虑长程纠缠（这里的长程并不是指距离上的长短，而是在lattice model上连接的希尔伯特空间的个数是infinite），问题在于长程纠缠的独特性质是什么？（它的熵是多少）
另外就是取热力学极限是将希尔伯特空间的张量维度（感觉这个维度和普通意义上的维度不同）推向infinite，还有有种把lattice model变成continuous model的感觉。
在tqft里，我们给cobordism安上一个希尔伯特空间，在这里是给一个lattice model安上一个希尔伯特空间，感觉本质上是一致的。



10.12

1.表示和同态的关系

2.我们说对称性的话只关注于时间平移（或者说与Hamilton对易），考虑到energy momentum tensor和计算守恒量时也是只有在时间演化下是守恒的，因此这种对称性是相当不完善的（但是貌似我们也只能关心时间上的守恒量）。我们可以extend symmetry and to consider followings:

i.isometry

ii.conformal

iii.homeomorphism

我们这里的结构基本上都是对于$g_{\mu\nu}$而言，关心的是不变量以及其分类。

感觉tqft也是个bootstrap的方法，就是从构造homeomorphism invariant出发（问题在于tqft给出了怎样的field和quantum state），然后再有lagrangian等。但是仔细想想好像还不太一样，cft中有各种各样的fields，呃，它的field是怎么给出的呢？记不清楚了。。


