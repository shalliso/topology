---
layout: post
title: "Putting things together"
categories: lecture
---

We started off by showing that if $$X$$ is the real line with the cofinite topology, then a set $$A \subseteq X$$ is dense if and only if it is infinite.

Given a topological space $$X$$ and a set $$A \subseteq X$$ we showed that if $$\mathcal{B}$$ is a basis for the topology on $$X$$ then to check that $$A$$ is dense it suffices to check that any non-empty *basic open* set $$U \in \mathcal{B}$$ intersects $$A$$.
We applied this to show that if $$X$$ and $$Y$$ are both the real line with the standard topology, then the set $$\mathbb{Q} \times \mathbb{Q}$$ is dense in $$X \times Y$$ when given the product topology.

Next, we showed that in any topological space $$X$$, the class of closed sets contains $$\emptyset$$ and $$X$$ and is closed under arbitrary intersections and finite unions.

I asked the class to determine under what assumtions we can conclude that all singleton sets are closed. We proved that being Hausdorff is sufficient but in fact T1 is enough.

We discussed two examples of topological spaces in which singletons are not closed, namely:

- $$X = \{0, 1\}$$ with the trivial topology (the only open sets are $$X$$ and $$\emptyset$$)

- $$\mathbb{R}$$ with the upper topology

Given a topological space $$X$$, we call the **diagonal** of $$X$$ the set $$\{(x, x) \mid x \in X\}$$. We proved that $$X$$ is Hausdorff if and only if the diagonal is closed.

Today, we studied several different definitions we've seen and drew some connections. Next lecture, we will add continuous functions and sequences (and their limits) into the mix.