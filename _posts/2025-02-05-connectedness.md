---
layout: post
title: "Connectedness"
categories: lecture
---

Imagine you remove a point of the real line $$\mathbb{R}$$. How many "pieces" are you left with? Most would say "2". Now imagine you remove a point from the real plane $$\mathbb{R} \times \mathbb{R}$$. Most would say it remains in one piece but with a "hole". Thus suggests a way to formally prove that $$\mathbb{R}$$ and $$\mathbb{R} \times \mathbb{R}$$ with the standard topologies are not the same topological space. Of course, this is intuitively obvious, but if you reflect for a moment you may become convinced that we would need to pursure something along these lines to actually prove it. It's clear that they're different spaces when you consider that $$\mathbb{R}$$ has one dimension while $$\mathbb{R} \times \mathbb{R}$$ has two, but it's not clear that after boiling everything down to just the topology we still have a way of making sense of the "dimension" of a space.

The notion of connectedness allows us to make formal the idea of a topological space having "just one piece". If you're curiuos, the number of "holes" of a topological space is formalized by homotopy and the fundamenal group, which is taught in a course on algebraic topology (which is usually taken directly after a course on topology).

Given a topological space $$X$$, we say that $$X$$ is **connected** if the only clopen sets are $$\emptyset$$ and $$X$$.

It turns out in practice working with the notion of being **disconnected** (i.e. not connected) is a often a bit easier, and there are several equivalent ways to characterize it. In particular, the following are all equivalent:

1. $$X$$ is disconnected;

2. There are non-empty disjoint open $$U_1, U_2 \subseteq X$$ such that $$U_1 \cup U_2 = X$$;

3. There are non-empty disjoint closed $$C_1, C_2 \subseteq X$$ such that $$C_1 \cup C_2 = X$$.

Given a set $$A \subseteq X$$ is connected if it is connected in the relative topology as a subspace of $$X$$. If we recall how the relative topology is defined, we can restate this as saying that $$A \subseteq X$$ is connected if there is no pair of open sets $$U_1, U_2 \subseteq X$$ that both have nonempty intersection with $$A$$ that are disjoint within $$A$$ (i.e. $$U_1 \cap U_2 \cap A = \emptyset$$) and cover $$A$$ (i.e. $$A \subseteq U_1 \cap U_2$$).

We proved that the closed interval $$[0, 1]$$ is connected. This is actually quite important so we labeled it as a theorem. We presented two proofs, the first of which was similar but slightly simpler to the one in the book, which I reproduce here. Considering equivalent statement (3) above and the observation in the previous paragraph, as well as the fact that $$[0, 1]$$ is closed, it is sufficient to show that any two nonempty closed sets $$C_1, C_2 \subseteq [0, 1]$$ with $$C_1 \cup C_2 = [0, 1]$$ must intersect. Indeed, assume without loss of generality $$0 \in C_1$$. Let $$b$ be the infimum of $$C_2$$ (i.e. the greatest lower bound). It's straightforward to check that $$b$$ must be a limit point of $$C_2$$ and thus an element of $$C_2$$. Thus if $$b = 0$$ we have that $$0 \in C_1 \cap C_2$$, so assume that $$b > 0$$. But in order for $$[0, 1]$$ to be a subset of $$C_1 \cap C_2$$ we must then have that $$[0, b) \subseteq C_1$$. But then $$b$$ is also a limit point of $$C_1$$ and thus in $$C_1$$ and so we have $$b \in C_1 \cap C_2$$.

Next, we discussed several examples of topological spaces and decided whether they are connected or disconnected:

1. $$(0, 1) \cup \{2\}$$ with the standard topology

2. $$(0, 1) \cup \{2\}$$ with the upper topology

3. $$\mathbb{R}$$ with the lower limit topology

4. $$\mathbb{R}$$ with the discrete topology

5. $$\mathbb{R}$$ with the cofinite topology

6. $$(\mathbb{R} \times \mathbb{R}) \setminus (\{(x, 0) \mid x \in \mathbb{R}\} \cup \{(0, x) \mid x \in \mathbb{R}\})$$ with the standard product topology

The spaces (1), (3), (4) and (6) are disconnected while (2) and (5) are connected.

Finally, we proved that if $$X$$ is connected and $$f : X \rightarrow Y$$ is continuous then the image $$f(X)$$ is connected. This is also an important result and we labeled it as a theorem.
