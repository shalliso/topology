---
layout: post
title: "Sequences and axioms of separation"
categories: lecture
---

From now on we're going to relax our notation and (usually) stop giving our topology a special symbol. 
So if I say that $$X$$ is a topological space, I mean that $$X$$ is a set and it comes with an unnnamed topology that dictates when subsets of $$X$$ are open.
Even more, if I simply state that $$f : X \rightarrow Y$$ is a continuous function, I am implying that $$X$$ and $$Y$$ are not just sets but topological spaces.
This usually does not create any ambiguity but sometimes (like when we are working with multiple topologies on the same set) we will have to be careful.
Also, when we have a point $$x_0$$ and an open set $$U \ni x_0$$, we often call $$U$$ an **open neighborhood** of $$x_0$$.

## More continuity 

We started by showing that if $$X$$, $$Y$$, and $$Z$$ are topological spaces and $$f : X \rightarrow Y$$ and $$g : Y \rightarrow Z$$ then the composition $$g \circ f : X \rightarrow Z$$ is a continuous function.

I explained that continuity of a function is what is known as a "global" property because it says something about $$f$$ everywhere on its domain. But continuity has a "local" definition as well.
Given a function $$f : X \rightarrow Y$$ and a point $$x_0 \in X$$, we say that $$f$$ is **continuous at** $$x_0$$ if for every open neighborhood $$V \ni f(x_0)$$ there is an open neighborhood $$U \ni x_0$$ such that $$f(U) \subseteq V$$.
We proved that a function $$f : X \rightarrow Y$$ is continuous if and only if $$f$$ is continuous at every point $$x_0 \in X$$.

In the case that we have a bijection $$f : X \rightarrow Y$$ such that both $$f$$ and the inverse $$f^{-1}$$ are continuous, then we call $$f$$ a **homeomorphism**, and that $$X$$ and $$Y$$ are **homeomorphic**. We can think of this as saying that $$X$$ and $$Y$$ are topologicaly the same.
In particular, if $$X$$ satisfies some topological property (such as the axioms T0, T1, T2 mentioned below), then $$Y$$ should satisfy the property too.
More on this later.

## Sequences and limits

Given a topological space $$X$$ we say that a sequence $$(x_n)$$ **converges** to a point $$x_\infty$$ if for every open neighborhood $$U \ni x_\infty$$ there is some large enough natural number $$N$$ such that for every $$n \ge N$$ we have $$x_n \in U$$.
In this case we can write $$x_n \rightarrow x_\infty$$ and also say that $$x_\infty$$ is **a limit** of $$(x_n)$$.

Why "a" limit? In some (admittedly silly) topologies, a sequence may have multiple limits. For example, consider the topology on the set $$\{0, 1\}$$ where only the sets $$\emptyset$$ and $$\{0, 1\}$$ are open. Then the sequence $$0, 0, 0, ...$$ has both 0 and 1 as limits.

## Separation axioms

What additional assumptions do we need to get uniqueness of limits?
We began looking at the hierarchy of separation axioms, which are additional assumptions we can make about a topological space $$X$$.

* (T0, aka Kolmogorov) For any $$x_0, x_1 \in X$$ with $$x_0 \neq x_1$$ there is either an open neighborhood $$U \ni x_0$$ with $$x_1 \not\in U$$ or there is an open neighborhood $$U \ni x_1$$ with $$x_0 \not\in U$$.

* (T1, aka Frechet) For any $$x_0, x_1 \in X$$ with $$x_0 \neq x_1$$ there are open neighborhoods $$U_0 \ni x_0$$ and $$U_1 \ni x_1$$ with $$x_0 \not\in U_1$$ and $$x_1 \not\in U_0$$.

* (T2, aka Hausdorff) For any $$x_0, x_1 \in X$$ with $$x_0 \neq x_1$$ there are open neighborhoods $$U_0 \ni x_0$$ and $$U_1 \ni x_1$$ with $$U_0 \cap U_1 = \emptyset$$.

You should remember the Hausdorff property (we will refer to it as "Hausdorff", not T2). I don't expect you to remember the other two, but you should be able to use them if I remind you what they are.
Observe that T2 implies T1, and T1 implies T0.
We will introduce a couple more (stronger) separation axioms later in the course.

We showed that in any Hausdorff space, limits of sequences (if they exist) are unique.
To be answered in the future, we asked where exactly "uniqueness of limits" appears in this hierarchy. Does "uniqueness of limits" imply Hausdorff? Does T_1 imply it?
These are often the types of questions that active mathematics researchers try to answer.

For an exercise, we determined which separation axioms the upper topology, standard topology, and lower limit topologies on $$\mathbb{R}$$ satisfy.
The upper topology is T0 but not T1 (and thus not T2).
The standard topology is T2 (and thus also T1 and T0).
Since the lower limit topology is finer than the standard topology, it is also T2 (and thus T1 and T0).

## Returning to continuity

We showed that if $$f : X \rightarrow Y$$ is continuous and $$x_n \rightarrow x_\infty$$ in $$X$$ then $$f(x_n) \rightarrow f(x_\infty)$$.
In fact, you should be able to see that it is enough to assume that $$f$$ is continuous at $$x_\infty$$ for the proof to go through.

Warning: if lecture attendance drops too low I will stop posting these notes online!