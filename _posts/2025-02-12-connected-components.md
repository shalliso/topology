---
layout: post
title: "Connected components"
categories: lecture
---

We started by recalling results from last lecture that imply that every connected component is closed. Must it be open? 

Yes and no.

We showed that if a topological space is "locally connected", meaning that every point is contained in an open neighborhood that is connected, then connected components are open.
On the other hand, if we give $$\mathbb{R}$$ the standard topology and considered the subspace $$X = \mathbb{Q}$$ with the relative topology, then the connected components of $$X$$ are all singletons, which are not open in that space.

Next, we gave a proof that if $$(A_i)_{i \in I}$$ is an indexed family of connected sets with a common point $$x \in \bigcap_{i \in I} A_i$$ then the union $$\bigcup_{i \in I} A_i$$ is connected.

This allowed us to prove that if $$X$$ and $$Y$$ are connected spaces then the product $$X \times Y$$ is connected.
We spent a lot of time discussing tempting but incorrect proofs before presenting a "correct" proof.
The proof we covered involves fixing a point $$(x_0, y_0)$$ and considering the $$+$$-shaped sets

$$A_{\hat{y}} = \{(x_0, y) \mid y \in Y\} \cup \{(x, \hat{y}) \mid x \in X\}.$$

These sets are connected (because $$X$$ and $$Y$$ are) and they all have the point $$(x_0, y_0)$$ in common, and moreover every point in $$X \times Y$$ lies within one of these sets. Thus the union $$\bigcup_{\hat{y}} A_{\hat{y}}$$ is connected and equal to $$X \times Y$$.

Returning to our exploration of connected components, we can prove that any point $$x$$ in a topological space $$X$$ is contained in a unique connected component. This is good because we wanted our notion of connected component to formalize our intuition of a "piece" of a topological space. There are two parts of our proof: "existence" (every point in contained in at least one connected component) and "uniqueness" every point is contained in at most one connected component. We proved these separately. For existence, we observed that we can simply take all the connnected sets that contain $$x$$ and take their union, which is thus connected by the earlier result. This union is in fact a connected component because if it was contained within a larger connected set then that larger set would have been among the sets we unioned up. For uniqueness, we observed that if $$A$$ and $$B$$ are two connected components containing $$x$$ then by the earlier result $$A \cup B$$ is connected, and thus $$A = A \cup B = B$$.

Because the notion of connected components partitions up a topological space, this produces an equivlence relation. We can write that $$x \sim^c y$$ iff there is a connected set containing both $$x$$ and $$y$$. Then the equivalence classes $$[x]_{\sim^c}$$ are exactly the connected components.

We can also develop the notion of components for path-connectedness. In this case, it's easier to start with the equivalence relation. We write $$x \sim^p y$$ iff there is a path from $$x$$ to $$y$$. Some staraightforward manipulation of paths tells us that this is in fact an equivalence relation, in which case we can define the path-connected components to be the equivlence classes $$[x]_{\sim^p}$$. See if you can answer the following: need path-connected components be closed? open?