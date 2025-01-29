---
layout: post
title: "Graphs of functions and other exercises"
categories: lecture
---

In this lecture we did a grab-bag of exercises and propositions to hopefully solidify our understanding of the basic concepts we will be building on in this course.

First, we proved that in a Hausdorff space, finite sets are closed. This is simply because that in a Hausdorff space, singletons are closed (discussed last time) and finite unions of closed sets are closed.

Next, we showed that if $$X$$ and $$Y$$ are topological spaces with $$Y$$ Hausdorff, and $$f : X \rightarrow Y$$ is continuous, then the **graph** of $$f$$, defined $$\textrm{graph}(f) := \{(x, f(x)) \mid x \in X\}$$ is closed as a subset of $$X \times Y$$.
This proof ended up being more challenging than I expected, so I include the argument here.
Suppose $$(x, y)$$ is an arbitrary element of $$X \times Y$$ not in the graph of $$f$$.
Then we have $$y \not= f(x)$$.
So because $$Y$$ is Hausdorff, we can find disjoint open $$V_1, V_2$$ with $$y \in V_1$$ and $$f(x) \in V_2$$.
Let $$U := f^{-1}(V_2)$$ which is open.
Then we can see $$U \times V_1$$ is an open neighborhood of $$(x,y)$$.
To check that it is disjoint from the graph of $$f$$, fix some $$x' \in X$$ and suppose for contradiction that $$(x', f(x')) \in U \times V_1$$.
But by definition of $$U$$ we have $$f(x') \in V_2$$.
So we have $$f(x') \in V_1 \cap V_2$$ which contradicts that they are disjoint.

We also gave another proof that the graph is closed.
First, we proved a lemma which states that if $$X_1, X_2, Y_1, Y_2$$ are topological spaces and $$f : X_1 \rightarrow Y_1$$ and $$g : X_2 \rightarrow Y_2$$ are continuous functions then the function $$h : X_1 \times X_2 \rightarrow Y_1 \times Y_2$$ defined by $$h(x_1, x_2) := (f(x_1), g(x_2))$$ is continuous.
Second, we proved that for any continuous function, preimages of closed sets are always closed.
With these lemmas, we can provide another proof of the previous result. We can define the function $$h : X \times Y \rightarrow Y \times Y$$ by $$h(x, y) = (f(x), y)$$.
Then the preimage under $$h$$ of the diagonal on $$Y$$ (which we proved to be closed last time) is precisely the graph of $$f$$, which is thus closed.

Finally, saw that if $$X$$ is a topological space and $$x \in X$$ and if $$X$$ has a countable basis, then we can construct a decreasing sequence $$(U_n)$$ of open neighborhoods of $$x$$ such that for any other open neighborhood $$V \ni x$$ we can find some $$N$$ such that for all $$n \ge N$$ we have $$U_n \subseteq V$$.
Then if we construct a sequence $$(a_n)$$ with $$a_n \in U_n$$ we have $$a_n \rightarrow x$$.
In particular, if $$A \subseteq X$$ is closed and $$x$$ is a limit point of $$A$$ then we can find a sequence $$(a_n)$$ from $$A$$ such that $$a_n \rightarrow x$$.
But it is very important to keep in mind we used the assumption that there is a countable basis of $$X$$.
We cannot do this in general.