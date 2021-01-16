---
layout: post
title: Daily questions and thoughts
tags: 
 - questions
 - learning process
 - conclusion
 - tqft
subtitle: 
date: 2020.10.13
author: Rick.T
header-img: img/post-bg-universe.jpg
catalog: true
---

<head>
<script id="MathJax-script" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
<script>
 MathJax = {
 tex: {
 inlineMath: [['$', '$'], ['\\(', '\\)']],
 packages: ['base', 'newcommand', 'configMacros']
 },
 svg: {
 fontCache: 'global'
 }
 };
</script>
</head>

7.20

今天突然想起来个问题，为啥我们想要研究cft呢？

loose掉isometric symmetry然后让他变成conformal symmetry，突然有种距离不重要，之间的夹角才重要的感觉（但是为什么这么要求呢）。另外一点就是在真实世界中存在这种具有conformal symmetry的physical system吗，我的感觉是肯定存在，因为其本身就是对isometric symmetry的loose，这样的话我们可以说后者是前者的特例，那么后者也是一种isometric symmetry，emmm，但是这样想还有一个问题，conformal symmetry除了可以选择等距外还有其他选择，怎么让物理系统有其他选择下的对称性呢？

8.4

1.我们凭什么要求$H=\frac{p^2}{2m}+V$在量子力学中仍然成立，i.e.，为什么作为算符这种关系仍然满足？

或许我们应该去看$H$和$p$实际上指什么，$H$和$p$其实是时空平移生成元，因此在考虑经典时空时，其有上述对应的结构。

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
\langle\phi(x)\phi(y)\rangle
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

Exactly，表示就是同态，投影表示只不过是homomorphism up to a central term，应该能想到，表示要干的事就是保持群的乘法结构，因此其自然就是同态，这个定义是well-defined。从category来说，表示可以看成两个范畴间的functor（比如从群到表示空间），而同态就是表示之间的natural transformation。

In a rather general form, we therefore have a **representation** of a category C in a category D is simply a [functor](https://ncatlab.org/nlab/show/functor)  F:C→D. Similarly, an [homomorphism](https://ncatlab.org/nlab/show/homomorphism) between representations (“[intertwiner](https://ncatlab.org/nlab/show/intertwiner)”) is simply a [natural transformation](https://ncatlab.org/nlab/show/natural+transformation) between functors when they are being thought of as representations. Thus we have a [category of representations](https://ncatlab.org/nlab/show/category+of+representations).

2.我们说对称性的话只关注于时间平移（或者说与Hamilton对易），考虑到energy momentum tensor和计算守恒量时也是只有在时间演化下是守恒的，因此这种对称性是相当不完善的（但是貌似我们也只能关心时间上的守恒量）。我们可以extend symmetry and to consider followings:

i.isometry

ii.conformal

iii.homeomorphism

我们这里的结构基本上都是对于$g_{\mu\nu}$而言，关心的是不变量以及其分类。

感觉tqft也是个bootstrap的方法，就是从构造homeomorphism invariant出发（问题在于tqft给出了怎样的field和quantum state），然后再有lagrangian等。但是仔细想想好像还不太一样，cft中有各种各样的fields，呃，它的field是怎么给出的呢？记不清楚了。。

3.老生常谈的cft中lack lagrangian description是啥？

10.13

1.不依赖于basis的tensor product定义（在category里的定义）是什么？

2.将tensor product space reduce to direct sum space

3.之前的一套理论是有一个complete commute set $\{A,B,C...\}$的话，我们可以写出对应的tensor product space，这个space是将不同的Hilbert space tensor起来的，分别对应了相应的data，然后对这个整个的space，我们可以用

$$
|a,b,c,...\rangle
$$

来表示其中一个vector，这里

$$
|a,b,c,...\rangle\equiv|a\rangle\otimes|b\rangle\otimes|c\rangle\otimes ...
$$

其中$a,b,c,...$代表了相应的data，或者说量子数。而简并的意思就是我们信息太少，只能看到$a\rangle$的情况，因此我们需要更多的信息和其他态来label简并态。这里的一点小问题就是，我们知道不在一个Hilbert space一定commute(e.g.$A \otimes I$and $I \otimes B$一定是commute的)，但是commute是否一定能写成上述形式呢？很明显不一定，比如

$$
\begin{pmatrix}
A & 0 \\\\
0 & I
\end{pmatrix}
$$

和

$I\quad 0$

$0\quad B$

在都表示成矩阵时，这里是direct sum，显然与上面的情况不同，而且似乎将上述所有情况都替换成$\oplus$也成立。。（其实不成立，因为这样的话各个态之间没有分立的关系了，refer to the difference of tensor product & cartesian product）但是怎么解释呢？还有许多情况下人们都喜欢reduce到direct sum space里，联系是什么呢？

4.我喜欢的一种general的对称性的expression，

$$
\mathcal{L}_X Y=0
$$

$X$是单参微分同胚群无穷小变换的所对应的vector，$Y$是任一物理量，这样我们就可以说$Y$具有某种某种连续对称性 (e.g. $Y\equiv g_{\mu\nu}$, $Y\equiv L$, $Y\equiv \Phi$)，这个体现了数学简洁的特点，但是需要注意的是，这里我们还未将discrete symmetry纳入，以及quantum symmetry中一些特有的性质，比如说投影表示，中心扩张等。

5.某种意义上讲，gauge transformation就是coordinate transformation，其都对应了structure group，不同的地方在于，在principal bundle上叫gauge transformation，在tangent vector bundle（或其他？）上叫coordinate transformation，总之就是section之间的微分同胚。。（不太准确，spirit到了）

10.16

1.cs theory note大体思路

chern simons theory从trivial bundle出发，类比yangmills action给出一个F wedge F定义在B（with boundary的mfd）上的的不变量，然后我们去看他的boundary，发现在boundary上是cs action，接着我们想对所有的bundle都定义类似结构，因此去找其universal bundle，构建了一个在closed mfd上的action，再然后是把mfd要求放宽，因此我们让B为n chain，然后其boundary是closed mfd的并，这样我们就对一些mfd定义了cs action。
我还考虑了cs action的物理意义，会发现求其el eqn，是Bianchi identity，因此什么都不会贡献，但是其能够给出partition function，每个Z对应的是一个场论，对每个配边都有一个量子态，而分类其实就描述了量子态的类别。还有一个问题，其对Z的贡献的物理意义是什么？correlation function怎么求？

2.还想学NLσM

12.7

1.统计物理中的自发对称性破缺与场论中的自发对称性破缺相对比，我们可以注意到在统计物理中，一级相变是化学势连续，化学势的一阶导也就是熵不连续，因此在场论中如果我们处在叠加态时，应该有某个东西对应于熵，然后当我们选择一个作为“实在”的态之后，熵就会发生变化，这里的熵对应了什么？其次是在二级相变以及之后的相变时，这些现象对应了场论中的什么？

同样在统计物理中，我们考虑T趋于0时，1/β趋于0，这时候就像取了hbar趋于0，对应了经典极限，而T趋于infinity以及T在其他有限温度等情况下，和场论中的什么现象对应呢？

2.orientation的trans和spin structure的联系是什么？

3.landau ginzburg theory还想要看一下

12.10

1.还是从tqft说吧，首先问题就是我们为啥要用tr(F\wedge F)这个不变量呢？（我们也许可以这么解释，在四维时，其是tr(F\wedge *F)的最小值，但是这个解释非常weak）或者说chern simons class，其他那些equivalent classes用处在什么地方呢？也许正如不同相变对应了对称性一样，其他equivalent classes用来描述了其他的物理过程，然后问题就是我们有没有一个general的方法能够给出equivalent classes的物理意义，而不是一个个去看。

脑洞一下，tqft中有没有例如纠缠这种现象？（长程纠缠和拓扑不变量？？）

感觉还是有些迷惑，学会了tqft之后能干什么呢？虽然我觉得tqft是描述这个世界的正确的理论，但是不知道如何去check，而且能解决什么问题呢？第一个肯定是引力量子化的问题，其次呢？解决量子场论ugly的问题？重整化，excitation啥的？解释一些神奇的现象？比如yang-mills质量问题和夸克禁闭？🤔

2.一级相变的熵是不连续的，如果把这个熵看成纠缠熵的话，那么我们可以考虑一个纯的纠缠的ρ（考虑纯态是方便起见），那么我们也许可以把观察的过程当成一级相变，因为很明显，如果我们观察，那么能够得知A和B处在什么状态，纠缠熵减少。这个过程和自发对称性破缺相吻合，而且最关键的是，能够解释为什么这个破缺的过程是瞬间发生的（所以在量子力学这是什么对称性？？）。当然我们可以考虑二级相变在量子体系下是什么样子的？这里的熵是连续变化的，如果当成纠缠熵的话，连续变化的纠缠熵会是怎样的过程呢？

纠缠是很明显的量子力学的特征。

3.ising model应该算一种比较典型的lattice上的相互作用模型，话说3d ising model的主要困难是什么？（尝试算一下？）然后就是ising model感觉和toric code有点类似，可能相互作用还不是特别像，但是有些类似，那ising model里有anyon啥的吗？然后解决3d ising model可能会对3d toric code有所帮助。感觉好多3d问题都没解决，比如3d tqft的分类啥的。。。

4.ising model是gap的，然后看Hamiltonian像是取离散变量的qft，那么gapless的系统取连续的变量，又有点像qft了。。。（不过这个大体是胡扯了，因为还举得特殊的ising model的例子，还不知道ising model有没有nontrivial topological的性质，因此没啥保证）虽然听说那里是有cft，但是cft的处理方式可能也不算量子场论了

5.想看bpz，moore-seiberg他们的cft，想知道nontrivial的想法是啥
