---
layout: post
title: "Countability Properties"
categories: lecture
---

We proved some results relating the different countability properties we introduced in the previous lecture for general topological spaces and metrizable spaces.

First, we showed that being second-countable always implies being first-countable. 
In particular, if $$\mathcal{B}$$ is a countable basis for a topological space $$X$$, then for any point $$x \in X$$, we have that $$\mathcal{B}_x = \{U \in \mathcal{B} \mid x \in U\}$$ is a countable local basis at $$x$$.

Next, we showed that being first-countable imples being separable.
In particular, if $$\mathcal{B}$$ is a countable basis for a topological space $$X$$, assuming without loss of generalith that every $$U \in \mathcal{B}$$ is nonempty, we can select a point $$x_U \in U$$ for each such $$U$$ where $$\{x_U \mid U \in \mathcal{B}\}$$ is a countable dense subset of $$X$$.

Moving on to metrizable spaces, recall that a topological space $$X$$ is metrizable if and only if there is a metric $$d$$ on $$X$$ generating the topology. This means the collection of open balls $$\{B_d(x, r) \mid x \in X, \; r > 0\}$$ forms a basis for the topology.

We showed that every metrizable space is first-countable.
In particular, let $$d$$ be a metric on $$X$$ generating the topology for any point $$x \in X$$, consider $$\mathcal{B}_x = \{B_d(x, \frac{1}{n} \mid n \in \mathbb{Z}^{> 0}\)$$.
This forms a countable local basis at $$x$$.

Finally, we showed that every separable metrizable space is second-countable.
Suppose $$A \subseteq X$$ is a countable dense set and consider $$\mathcal{B} = \{B_d(x, \frac{1}{n}) \mid n \in \mathbb{Z}^{>0}\}$$.
This forms a countable basis for the topology.