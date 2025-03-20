---
layout: post
title: "Countability Examples"
categories: lecture
---
We started off by reviewing what the basis of a topology is and how to verify it.
Then we covered the first problem in the fifth written assignment.

Next, we attemted to prove a false theorem that in any topological space, if it is separable and first-countable, then it is second-countable.
We discussed a proof that started off convincing but ran into a snag.
Indeed, the lower limit topology provides a counterexample to this (we will discuss it in more detail next Wednesday).

Next, we discussed the cofinite topology on $$\mathbb{R}$$ and saw that it is separable but not first-countable (and thus not second-countable either).

I promised to cover a solution to the last problem in the fifth written assignment.
If $$x \in A$$ then we have $$d(x, A) = 0$$ so we can take $$a = x$$, so assume $$x \not\in A$$.
Let $$c = d(x, A)$$ and for each $$\epsilon > 0$$ let $$U_\epsilon = \{y \in X \mid d(y, x) > c + \epsilon\}$$
It's straightforward to check that each $$U_\epsilon$$ is open (using triangle inequality).
If we assume for contradiction there is no $$a \in A$$ with $$d(x, a) = c$$, then we have that $$\mathcal{O} = \{U_\epsilon \mid \epsilon > 0\}$$ forms an open cover for $$A$$.
Since $$A$$ is compact, $$\mathcal{O}$$ has a finite subcover of $$A$$, thus in particular there is $$\epsilon_0 > 0$$ small enough such that $$A \subseteq U_{\epsilon_0}$$.
However, since $$d(x, A) = c$$, there must be some $$b \in A$$ with $$d(x, b) < c + \epsilon_0$$, which is a contradiction.