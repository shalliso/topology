---
layout: post
title: "Closed and bounded"
categories: lecture
---

We started off reviewing the definition of compactness and the properties we proved of it.
Then we proved that in $$\mathbb{R}$$, a set is compact if and only if it is closed and bounded.
As an application of this, we proved that any continuous function $$f : [0, 1] \rightarrow \mathbb{R}$$ has a maximum, i.e. a point $$a \in [0, 1]$$ such that $$f(x) \le f(a)$$ for every $$x \in [0, 1]$$.
Students pointed out that this result still holds as long as the domain is any compact set, and the co-domain is any linearly-ordered set with the order topology (we aren't covering order topologies in this course).

We spent the second half proving a subtle but useful fact which says that compactness can be verified by only considering open covers coming from some basis.
More specifically, let $$X$$ be a topological space with basis $$\mathcal{B}$$. 
Then a set $$K \subseteq X$$ is compact if an only if for every open cover $$\mathcal{O}$$ consisting of open sets in $$\mathcal{B}$$, there exists a finite subcover.
The forward direction is immediate, but the backwards direction required careful argument.