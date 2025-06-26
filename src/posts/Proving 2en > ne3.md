---
title: Proving $2^n > n^3$ for all $n > 9$
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

Taking the $\log$ of both sides:

$$
\begin{aligned}
&\log (2^{n}) > \log (n^{3}) \\
&\boxed{ n\log 2 > 3\log n }  \qquad (\ast)
\end{aligned}
$$

Now, for $A(n+1)$:

$$
\begin{aligned}
& (n+1) \log 2 > 3 \log (n+1) \\
& \implies n\log 2 + \log 2  > 3 [\log n + \log 1] \\
&\implies n \log 2 + \log 2 > 3 \log n 
\end{aligned}
$$

This is true since $(\ast)$ - induction hypothesis. 

Which follows that $A(n)$ must be true.

Therefore, by the principle of mathematical induction, we have proven that $2^n > n^3$ for all $n > 9$.