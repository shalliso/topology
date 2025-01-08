---
layout: post
title: "First written assignment"
categories: assignment
---

1. If $$(A_i)_{i \in I}$$ is a collection of subsets of a set $$X$$, prove the following:
$$ X \setminus \bigcup_{i \in I} A_i = \bigcap_{i \in I} X \setminus A_i.$$
If $$(B_j)_{j \in J}$$ is another collection of subsets of $$X$$, prove the following:
$$ (\bigcup_{i \in I} A_i) \cap (\bigcup_{j \in J} B_j) = \bigcup_{i \in I} \bigcup_{j \in J} A_i \cap B_j $$

2. Let $$A$$ be a set of real numbers which is **bounded**, meaning there is a real number $$r$$ that is an **upper bound** of $$A$$ (i.e. $$a \le r$$ for every $$a$$ in $$A$$). We say that a real number $$s$$ is a **supremum** of $$A$$ (also known as **least-upper-bound**) if it is an upper bound of $$A$$ and moreover if $$s'$$ is another real number that bounds $$A$$, then $$s \le s'$$. Show that if a supremum of a set $$A$$ exists, then it is unique.
Now we confirm that supremums of bounded sets exist. This is known as the least-upper-bound property of the real numbers, which is a fundamental property of the reals. Let's prove this assuming that Cauchy sequences converge. We define a sequence $$(a_n)$$ of elements of $$A$$ and a sequence $$(b_n)$$ of upper bounds of $A$ recursively as follows: let $$a_0$$ be an arbitrary element of $$A$$ and let $$b_0$$ be an arbitrary upper bound of $$A$$. In general if $$a_n$$ and $$b_n$$ are defined, check if the average of $$a_n$$ and $$b_n$$ is an upper bound of $$A$$. If it is, let $$b_{n+1} = (a_n + b_n)/2$$ and let $$a_{n+1} = a_n$$. Otherwise, let $$a_{n+1} = (a_n + b_n)/2$$ and $$b_{n+1} = b_n$$. Show that these sequences are Cauchy and in fact converge to the same point, and that point is the supremum of $$A$$.

3. In-class exercise 1 from the first lecture 2025-01-06

4. In-class exercise 2 from the first lecture 2025-01-06

5. Manetti 3.3

6. Manetti 3.4

7. Show that the collection of intervals $$(a, b)$$ for *rational* $$a$$ and $$b$$ forms a basis for the standard topology. Show that the collection of half-open intervals $$[a, b)$$ for *rational* $$a$$ and $$b$$ does *not* form a basis for the lower-limit topology. Find a nice basis of the upper topology consisting of only finitely-many sets.

