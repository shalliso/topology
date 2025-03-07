---
layout: post
title: "Second written assignment"
categories: assignment
---

It is very important that you do **not** look up any answers or ask any AI assistant on these assignments. Each assignment is worth less than 1% of your grade! They provide significant value in helping you understand the material and prepare for the tests, and that is wasted if you take shortcuts. Also, the internet is full of nonsense (some Googling around actually came up with some **incorrect** answers for some of these questions!). On the other hand, AI is a super useful tool (when it gives sensible answers) but is a poison pill if you allow it to erode your critical thinking. But critical thinking is precisely the skill we will need to be successful in a future dominated by AI!

You may work with other classmates on this homework but do not copy down answers. A good rule of thumb is if you solve a problem together, wait at least an hour before writing down the solution, and don't consult any notes from your problem solving session. It is best to first put some effort into each problem on your own before working with someone else.

## Question 1

Let $$X$$ be a set and let $$d_1$$ and $$d_2$$ be two metrics on $$X$$. Suppose for any $$x \in X$$ and $$\epsilon > 0$$ there is some $$\delta > 0$$ such that $$B_{d_2}(x, \delta) \subseteq B_{d_1}(x, \epsilon)$$. Show that the topology generated by $$d_2$$ is finer than the topology generated by $$d_1$$.

## Question 2

Show that the standard Euclidean topology, the Manhattan metric, and the square metric all all indeed metrics and generate the same topology on $$\mathbb{R}^2$$.

## Question 3

In this problem we will adopt the convention that $$0 \in \mathbb{N}$$.

Let $$\mathbb{N}^\mathbb{N}$$ be the set of all functions from $$\mathbb{N}$$ to $$\mathbb{N}$$, which we can think of as infinite sequences $$(a_n)_{n \ge 0}$$ of natural numbers, such as: 0, 1, 2, 3, ..., or 0, 0, 0, 0, ..., or 0, 1, 0, 1, ..., or 1, 10, 100, 1000, ..., and so on. Let $$\mathbb{N}^{<\mathbb{N}}$$ be the set of finite sequences $$(a_n)_{n < N}$$ of natural numbers. For every $$\bar{a} = (a_n)_{n < N} \in \mathbb{N}^{<\mathbb{N}}$$, define the set

$$ \mathcal{N}_{\bar{a}} := \left\{(b_n)_{n \ge 0} \in \mathbb{N}^\mathbb{N} \mid \forall n < \|\bar{a}\| \; a_n = b_n\right\}$$

where $$\|\bar{a}\|$$ represents the length of $$\bar{a}$$.

Show that the collection of theses sets forms a basis for a topology on $$\mathbb{N}^\mathbb{N}$$. This is known as Baire space. It is a super useful and interesting topology that is in some ways very similar to the standard topology on $$\mathbb{R}$$, but in some ways very dissimilar.

Next, define the following two fuctions $$d_1, d_2 : \mathbb{N}^\mathbb{N} \times \mathbb{N}^\mathbb{N} \rightarrow \mathbb{R}$$:

$$d_1((a_n)_{n \ge 0}, (b_n)_{n \ge 0}) = \sum \left\{\frac{1}{2^n} \mid n \ge 0, \; a_n \neq b_n\right\}$$

and

$$d_2((a_n)_{n \ge 0}, (b_n)_{n \ge 0}) = \frac{1}{2^k}$$

for the minimum $$k \ge 0$$ such that $$a_k \not= b_k$$, or 0 if no such $$k$$ exists.

Choose one of these and show that it is a metric and generates the topology we just defined on Baire space (both of them do!).

## Question 4

1. We saw in lecture that $$\mathbb{R}$$ with the upper topology is not T1. Write down a fully rigorous proof of this.

2. We also showed that any Hausdorff (T2) topology satisfies "uniqueness of limits". Does the upper topology satisfy uniqueness of limits? Recall that "uniqueness of limits" means that if $$x_n \rightarrow x_\infty$$ and $$x_n \rightarrow x_\infty'$$ then $$x_\infty = x_\infty'$$.

3. Now show that "uniqueness of limits" implies T1. This tells us that "uniqueness of limits" lies somewhere between T1 and T2 (if you're curious, it's actually strictly between -- ask me in office hours if you're curious why).

4. Recall the cofinite topology on $$\mathbb{R}$$ consists of all sets with finite complements. Is it T0? T1? T2? Does it satisfy "uniqueness of limits"? (A hint will be provided in approximately one week) Prove all your answers.

## Question 5

Do Manetti 3.53(1) and 3.56

## Question 6

A topological space $$X$$ is **metrizable** if there is a metric $$d : X \times X \rightarrow \mathbb{R}$$ that generates the topology.

Do Manetti 3.38 and 3.39. 

## Final remarks

At this point you should be able to do the majority of the exercises in Chapter 3 of Manetti, except for some topics we haven't covered yet such as closed sets.
