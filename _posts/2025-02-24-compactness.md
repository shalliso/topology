---
layout: post
title: "Compactness"
categories: lecture
---

We first observed that given two topological spaces $$X$$ and $$Y$$, if those spaces are actually metric spaces with metrics $$d_X$$ and $$d_Y$$ respectively, then we can characterize a function $$f : X \rightarrow Y$$ being continuous if and only if for every $$x \in X$$ and $$\epsilon > 0$$ there is some $$\delta > 0$$ such that for any $$x' \in X$$, if $$d_X(x, x') < \delta$$ then $$d_y(f(x), f(x')) < \epsilon$$.

We then used this definition to show that given any two continuous functions $$f, g : \mathbb{R} \rightarrow \mathbb{R}$$ and scalars $$c, d \in \mathbb{R}$$ we have the *linear combination* $$cf + dg$$ defined by $$(cf + dg)(x) = cf(x) + dg(x)$$ is continuous. This tells us that the continuous functions from $$\mathbb{R}$$ to $$\mathbb{R}$$

We reviewed the notion of **homemorphism**. Recall that a function $$f : X \rightarrow Y$$ between topological spaces is a homeomorphism iff it is bijective (and thus has an inverse $$f^{-1}$$) and moreover both $$f$$ and $$f^{-1}$$ are continuous.
In this case we say $$X$$ and $$Y$$ are **homeomorphic**, often denoted $$X \cong Y$$. We can view two homeomorphic spaces as being ``the same".
In particular, if $$X$$ is connected and $$X \cong Y$$, then so is $$Y$$. If $$X$$ is Hausdorff then so is $$Y$$, etc.
This allows us conversely to say that two spaces are not homemorphic if there is some topological property that one space exhibits but the other doesn't. For example, $$\mathbb{R}$$ and $$\mathbb{R}\setminus\{0\}$$ are not homeomorphic because $$\mathbb{R}$$ is connected while the other is not.
We can also say $$\mathbb{R}$$ and $$\mathbb{R}^2$$ are not homeomorphic because for the first, removing any one point makes it disconnected, while that is not true for the second.

We started discussing the next main topic: **compactness**.

We say a topological space $$X$$ is **compact** iff every open cover of $$X$$ has a finite subcover. What is an open cover? An **open cover** of $$X$$ is a family $$\{U_{i \in I}\}$$ of open sets in $$X$$ such that the union $$\bigcup_{i \in I} U_i$$ is equal to $$X$$. A subcover is simply a subfamily $$(U_i)_{i \in I_0}$$ for some $$I_0 \subseteq I$$ whose union is still $$X$$. So in other words, $$X$$ is compact if and only if for every collection $$\{U_i\}_{i \in I}$$ of open sets that unions up to $$X$$, there is a finite $$I_0 \subseteq I$$ such that $$\{U_i\}_{i \in I_0}$$ still unions up to $$X$$.

The real line $$\mathbb{R}$$ is not compact, since it has a cover $$\{(z, z+2) \mid z \in \mathbb{Z}\}$$ which does not have a finite subcover.

We started but didn't finish a proof that $$[0, 1]$$ is compact. More generally, we will prove that a subset of $$\mathbb{R}$$ is compact if and only if it is closed and bounded.
