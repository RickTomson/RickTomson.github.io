---
layout: post
title: Daily questions
tags: 
 - 1.02137
subtitle: Problems of state-operator correspondence
date: 2020.9.13
author: Rick.T
header-img: img/post-bg-universe.jpg
catalog: true
---

8.4

1.我们凭什么要求H=\frac{p^2}{2m}+V在量子力学中仍然成立，i.e.，为什么作为算符这种关系仍然满足？

或许我们应该去看H和p实际上指什么，H和p其实是时空平移生成元，因此在考虑经典时空时，其有上述对应的结构。

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


