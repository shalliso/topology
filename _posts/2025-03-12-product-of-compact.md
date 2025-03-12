---
layout: post
title: "Products of compact spaces"
categories: lecture
---

The first half of this lecture addressed a single result: that the product of two compact spaces is compact.
We briefly used this result to prove a corollary: a subset of $$\mathbb{R} \times \mathbb{R}$$ which is closed and bounded is compact (the other direction is also true and requires a proof similar to the proof we saw for subsets of $$\mathbb{R}$$).
The proof in the textbook is quite different from the one we did in lecture, so I sketch it here.

Let $$X$$ and $$Y$$ be two compact spaces.
Let $$\mathcal{O}$$ be an open cover of $$X \times Y$$.
By the result from the previous lecture, since the set $$\{U \times V \mid U \subseteq X \text{ open}, V \subseteq Y \text{ open}\}$$ forms a basis for the topology on $$X \times Y$$, we can assume $$\mathcal{O}$$ is of the form $$\{U_i \times V_i \mid i \in I\}$$.
For each $$y \in Y$$, define $$I^y := \{i \in I \mid y \in V_i\}$$ and $$\mathcal{O}^y := \{U_i \mid i \in I^y.\}$$.
We argued that $$\mathcal{O}^y$$ is an open cover of $$X$$, thus by compactness of $$X$$, there is a finite $$I^y_0 \subseteq I^y$$ such that $$\mathcal{O}^y_0 := \{U_i \mid i \in I^y_0\}$$ is a cover of $$X$$.
For each $$y \in Y$$, define $$V^y := \bigcap \{V_i \mid i \in I^y_0\}$$, which is open since $$I^y_0$$ is finite, and moreover contains $$y$$.
Thus $$\mathcal{O}^* := \{V^y \mid y \in Y\}$$ is an open cover of $$Y$$.
Thus there is finite $$Y_0 \subseteq Y$$ such that $$\mathcal{O}^*_0 := \{V_y \mid y \in Y_0\}$$ is a cover of $$Y$$.
Now let $$I_0 = \bigcup_{y \in Y_0} I^y_0$$ and $$\mathcal{O}_0 := \{U_i \times V_i \mid i \in I_0\}$$.
We claim that $$\mathcal{O}_0$$ is a finite cover of $$X \times Y$$.
It's immediate that $$\mathcal{O}$$ is a finite collection of open sets in $$X \times Y$$, so we show that it is a cover.

To this end, let $$(\hat{x}, \hat{y}) \in X \times Y$$ be arbitrary.
Since $$\mathcal{O}^*_0$$ is a cover of $$Y$$, there is some $$y^* \in Y_0$$ such that $$\hat{y} \in V_{y^*}$$.
Since $$\mathcal{O}^{y^*}_0$$ is a cover of $$X$$, there is some $$\hat{i} \in I^{y^*}_0$$ with $$\hat{x} \in U_{\hat{i}}$$.
Then $$(\hat{x}, \hat{y}) \in U_{\hat{i}} \times V_{\hat{i}}$$ and $$\hat{i} \in I_0$$ so indeed the point $$(\hat{x}, \hat{y})$$ is covered by $$\mathcal{O}_0$$.

It's a difficult proof! It will take some time to fully digest.

In the second half, we started to set up a deeper discussion of sequences.
We defined three properties of a topological space $$X$$:

1. $$X$$ is **second-countable** if the topology on $$X$$ has a countable basis;

2. $$X$$ is **first-countable** if every point in $$X$$ has a countable local basis; and

3. $$X$$ is **separable** if there is a countable dense subset.

Recall that given $$x \in X$$ a local basis of $$x$$ is a collection $$\mathcal{B}_x$$ of open neighborhoods of $$x$$ with the property that for any open neighborhood $$U \ni x$$ of $$x$$, there exists some $$V \in \mathcal{B}_x$$ with $$V \subseteq U$$.

For $$\mathbb{R}$$ with the standard topology, and $$\mathbb{R}$$ with the discrete topology, I asked the class to determine if these properties hold.
The standard topology, is second-countable, first-countable, and separable.
The discrete topology is not secound-countable, nor is it separable, but it is first-countable.

We will discuss implications between these properties and additional examples in the next lecture.