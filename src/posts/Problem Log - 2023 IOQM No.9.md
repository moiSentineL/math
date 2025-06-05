---
title: Problem Log - 2023 IOQM No. 9
tags:
  - problem
  - number-theory
date: 2025-06-04
excerpt: classic casework.
---
- Topic: Casework, NT
- [Source:: [2023 IOQM #9](https://artofproblemsolving.com/wiki/index.php/2023_IOQM/Problem_9)]
- [Time Taken:: 30m]
- [Solved?:: Kinda]

---
## Problem
Find the number of triples $(a, b, c)$ of positive integers such that:

(a) $ab$ is a prime;
(b) $bc$ is a product of two primes;
(c) $abc$ is not divisible by square of any prime and
(d) $abc\leq30$ 

## Solution
From (a), we know that one of $a$ or $b$ must be a prime and the other one 1.
### Case 1
Let's say we pick $a =1$.

In this case, $b$ and $c$ must both be different primes (that is, $b \neq c$, and both primes).

We find $A = \{ (a, b, c) : abc\leq 30 \implies bc\leq 30 \}$ ($\because a = 1$)

The set $A$ becomes:

$$
\begin{lgathered}
\{ (1, 2, 3), (1, 2, 5), (1, 2, 7), (1, 2, 11), (1, 2, 13), (1, 3, 2), (1, 3, 5), (1, 3, 7), (1, 5, 2), (1, 5, 3), (1, 7, 2), (1, 7, 3), (1, 11, 2), (1, 13, 2) 
\end{lgathered}
$$

and $\boxed{ n(A) = 14 }$ .
### Case 2
Now we pick $b = 1$.

In this case, since $bc$ is a product of two prime, and $b=1$, $c$ must be a product of two primes. That is $c \in \{ 6, 10, 14, 15, \dots \}$

We are also limited by $a$, which is also a prime ($\because ab$ is a prime)

Now, we need to find $B = \{ (a, b, c) : abc \leq 30 \implies ac \leq 30 \}$ ($\because b = 1$)

Again, $\because abc$ should not be divisible by square of any prime, we need to make sure that $ac$ is not divisible by any square as well.

So, the set $B$ becomes:

$$
\begin{lgathered}
\{ (2, 1, 15), (5, 1, 6), (3, 1, 10) \}
\end{lgathered}
$$

and $\boxed{ n(B) = 3 }$.

So, total possibilities = $n(A) + n(B) = 14 + 3 = \boxed{ 17 }$
