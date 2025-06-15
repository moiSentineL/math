---
title: Problem Log - 2023 IOQM No. 3
tags:
  - problem
  - number-theory
  - inequality
date: 2025-06-15
excerpt: easy but hard inequalities
---
- Topic: Number Theory, Inequalities
- [Source:: [IOQM 2023-24 #3](https://artofproblemsolving.com/wiki/index.php/2023_IOQM/Problem_3)]
- [Time Taken:: 47m]
- [Solved?:: Yes]

---
## Problem
Let $\alpha$ and $\beta$ be positive integers such that 

$$\frac{16}{37}<\frac{\alpha}{\beta}<\frac{7}{16}$$

Find the smallest possible value of β . 

## Solution

Reciprocal the inequality:

$$
\begin{lgathered}
\frac{16}{7} < \frac{\beta}{\alpha} < \frac{37}{16}
\end{lgathered}
$$

(the terms will switch sides)

Now, multiply all the terms with $\alpha$:

$$
\begin{lgathered}
\frac{16}{7} \alpha < \beta < \frac{37}{16} \alpha 
\end{lgathered}
$$

Now, $\frac{16}{7} \approx 2. 28$ and $\frac{37}{16} \approx 2.31$

We need to pick an $\alpha$ such that $\beta$ has a solution in the $\mathbb{Z}$ and that too, the smallest.

Through trial and error, we may find that if $\alpha = 10$, then 

$$
\begin{lgathered}
22.8 < \beta < 23.1 \\
\therefore \beta = 23
\end{lgathered}
$$

Which is the smallest possible value.

## Reflection
- What tripped me?
	- The fact that it took me over 10 minutes is a disgrace. (It took 47m). But since I am a learning mathematician, that is normal. I learned a lot from the problem.
- What pattern did I recognize?
	- I saw that the differences between the inequalities (no matter what $\alpha$ you pick) remains almost negligible.
	- I tried $\alpha = LCM(7, 16)$, but that was too large.
- What did I learn?
	- I was trying HUGE numbers for $\alpha$, when I could've tried $\alpha = 10$.
	- It took me 47m to get there,
	- But the next time, whenever there will be decimals, or inequalities, I will try smaller numbers and 10.

## Rating
🧠: 1–5 for [Insight:: 4]
⚔️: 1–5 for [Difficulty:: 2]

