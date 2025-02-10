---
layout: post
title: "Path connectedness"
categories: lecture
---

Last time we isolated what it means for a topology to be "in one piece", so today...

Wait, did we? Not everyone would necessarily feel like the definition we gave is the one they would first have thought of.
Does that mean they would be wrong? Let's consider another possible formulation.
Often times in math, there are multiple ways to formalize an informal idea like this, and they often reveal different perspectives.

We call a topological space $$X$$ **path-connected** if for any two points $$x_0, x_1 \in X$$ there is a continuous function $$\gamma : [0, 1] \rightarrow X$$ with $$\gamma(0) = x_0$$ and $$\gamma(1) = x_1$$. We call such $$\gamma$$ a **path from $$x_0$$ to $$x_1$$**.

Given a topological space $$X$$ and a set $$A \subseteq X$$, we say $$A$$ is **path-connected** if $$A$$ is path-connected in the relative topology, or equivalently, for any two points $$x_0, x_1 \in A$$ there is a continuous $$\gamma : [0, 1] \rightarrow X$$ with $$\gamma(0) = x_0$$ and $$\gamma(1) = x_1$$ such that the image of $$\gamma$$ is contained in $$A$$.

We didn't discuss any examples of path-connectedness (perhaps we should -- maybe next lecture).

We proved that if $$X$$ is a topological space and $$A, B \subseteq X$$ are path-connected and furthermore satisfy $$A \cap B \neq \emptyset$$ then $$A \cuo B$$ is path-connected.

Next, we proved that if a topological space $$X$$ is path-connected then it is connected. This follows from the fact that the "paths" in the definition of path-connectedness are continuous, and moreover we proved last time that the closed interval $$[0, 1]$$ is connected.

We gave an example of a topological space that is connected but not path-connected. We will revisit it along with a proof in a future lecture.

Thus, we have two notions of a space being "in one piece".
Now, suppose we are given a topological space that is not "in one piece". How do we define what the "pieces" are? How can we determine how many "pieces" make up the space?
This is a bit deeper of a question that will take some time to answer.

Let's return to the original definition of connectedness. As you may hope, the following can also be developed in the context of path-connectedness, if you wish.

Let $$X$$ be a topological space. We call a set $$A \subseteq X$$ a **connected component** if the following two properties are satisfied:

1. $$A$$ is connected

2. For any $$Y \subseteq X$$ if $$A \subseteq Y$$ and $$Y$$ is connected then $$A = Y$$.

The second statement amounts to saying that $$A$$ is "maximally connected" meaning that we can't add anything new to $$A$$ without making it disconnected.

We discussed what are the connected components of the real plane with the axes subtracted (which you saw on the test and we discussed last lecture.)
There are four of them and they consist of the four quadrants. As you can see, the quadrants are disjoint and partition the space, and moreover are closed in this space. This will actually be true in general topological spaces. (In our example the connected components are also open but this is not true in general).

We proved that if $$X$$ is a topological space and $$Y \subseteq X$$ is connected and $$W \subseteq X$$ satisfies $$Y \subseteq W \subseteq \overline{Y}$$ then $$W$$ is connected. In particular, taking $$W = \overline{Y}$$, this tells us that closures of connected sets are also connected. Thus, closures of connected components must be closed, which means in particular that connected components must be closed.

Finally, we gave a brief review of equivalence relations and the way they go hand-in-hand with partitions.