---
layout: post
title: "Closures and closed sets"
categories: lecture
---

Given a topological space $$X$$ and a set $$A \subseteq X$$, we say that a point $$x_0 \in X$$ is a **limit point** of $$A$$ if for every open neighborhood $$U \ni x_0$$ there is a point $$a \in U \cap A$$ with $$a \neq x_0$$.
We define the **closure** of $$A$$ to be the set $$\overline{A} := A \cup A'$$ where $$A'$$ is the set of limit points of $$A$$.
We note that by definition we always have $$A \subseteq \overline{A}$$ but not every point in $$A$$ is a limit point of $$A$$.

We did some examples:

1. If $$X = \mathbb{R}$$ with the standard topology, and $$A = (0, 1)$$, then the set of limit points of $$A$$ is the set $$[0, 1]$$ and $$\overline{A} = [0, 1]$$.


2. If $$X = \mathbb{R}$$ with the standard topology and $$A = \{\frac{1}{n} \mid n \in \mathbb{Z}^{\ge 1}\}$$ then the only limit point of $$A$$ is 0 and $$\overline{A} = A \cup \{0\}$$.

3. If $$X = \mathbb{R}$$ with the upper topology and $$A = (0, 1)$$ then the set of limit points of $$A$$ is $$[0, \infty)$$ and $$\overline{A} = [0, \infty)$$.

We say $$A \subseteq X$$ is **dense** if $$\overline{A} = X$$.
Equivalently, we say $$A$$ is dense if for every non-empty open set $$U \subseteq X$$ we have $$U \cap A \neq \emptyset$$.

Everyone already knows that $$\mathbb{Q}$$ is dense in $$\mathbb{R}$$ with respect to the standard topology.

We covered three other examples of density when the notion of being dense is equivalent to something very simple.
For each topological space $$X$$ below, describe exactly when a set $$A \subseteq X$$ is dense in $$X$$.

1. $$X = \mathbb{R}$$ with the upper topology. We determined that a set $$A \subseteq X$$ is dense if and only if it doesn't have a lower bound.

2. $$X = \mathbb{R}$$ with the discrete topology. We determined that $$A = X$$ itself is the only dense set.

3. $$X = \mathbb{R}$$ with the cofinite topology. We did not cover this and left it as something to think about for next week.

We defined the closed sets. A set $$A \subseteq X$$ is **closed** if $$\overline{A} = X$$.
We proved that equivalently, $$A$$ is closed if and only if $$X \setminus A$$ is open.

In some final remarks, we mentioned that "closed" does not mean "not open". In particular, a set can be both open and closed (sometimes called "clopen"), and a set can be neither open nor closed.
Note that for any topological space $$X$$, the sets $$\emptyset$$ and $$X$$ are clopen (because they are both defined to be open and are complements of each other).