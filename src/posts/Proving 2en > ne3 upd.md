---
title: Proving 2^n > n^3 for all n > 9 (updated)
date: 2025-06-26
tags:
  - number-theory
  - proof
excerpt: by mathematical induction and log
---
## Prove $2^n > n^3$ for all $n > 9$

**Proof:**

By mathematical induction.

Let $A(n)$ denote $2^{n}> n^{3}$.

For $n=10$ (base step)

$$
\begin{aligned}
2^{10} > 10^{3} \\
1024 > 1000
\end{aligned}
$$

Thus, $A(10)$ is true.

Now, assuming $A(n)$ is true, we get:

$$
\begin{aligned}
2^{n} > n^{3}
\end{aligned}
$$

Multiplying by $2$ on both sides:

$$
\begin{aligned}
&2^{n} \cdot 2 > 2 n^{3} \\
\implies &2^{n+1} > 2n^{3} \qquad (\text{i})
\end{aligned}
$$

We want to deduce, for $A(n+1)$:

$$
\begin{aligned}
2^{n+1} > (n+1)^{3}
\end{aligned}
$$

To prove this, we have to prove that: (from $\text{(i)}$)

$$
\begin{aligned}
2n^{3} \geq (n+1)^{3} \qquad(\text{ii})
\end{aligned}
$$

($\forall n> 9$)

We do this by contradiction.

Assuming $(\text{ii})$ is false, then $2n^{3} < (n+1)^{3}$ must be true for all $n>9$.

But for $n=10$, 

$$
\begin{aligned}
2(10)^{3} = 2000 > (10+1)^{3} = 1331
\end{aligned}
$$

Contradiction.

Thus, $\text{(ii)}$ is true, and which follows that $(\text{i})$ must be true.

Consequently:

$$
\begin{aligned}
2^{n+1} > (n+1)^{3}
\end{aligned}
$$

Which follows that $A(n)$ must be true.

Therefore, by the principle of mathematical induction, we have proven that $2^n > n^3$ for all $n > 9$.