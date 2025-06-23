---
title: To choose or not to choose
date: 2025-06-23
tags:
  - combinatorics
  - explanations
excerpt: intuitively understanding the number of reflexive relations that can be made on a set.
---

To choose, or not to choose. That is the question.

And that applies specifically while trying to comprehend why the number of reflexive relations that can be made on the set $A$ is $2^{n^{2}- n}$ and not $n$.

I am going to try explaining why that seems to be the case.

But before we get dirty with it, let us see what a reflexive relation looks like:

Considering a set $B = \{ 1, 2, 3 \}$.

Here, if you make a relation $R: B \times B$, you'll get something like this:

- $R_{1} = \{ (1, 1), (2, 2), (3, 3) \}$
- $R_{2} = \{ (1, 3), (1, 2) (1, 1) \}$
- $R_{3} = \{ (1, 1), (2, 2), (3, 3), (1, 2), (3, 2), \}$

where $R_{n} \subset R$.

Note here that $R_{1}$ and $R_{3}$ are, by definition, reflexive. But $R_{2}$ is not. 
Again, if you see clearly, **a reflexive relation may OR may not contain pairs in the form of $(a, a)$.** This is important to understand. 

Now we get our hands dirty.

Let me re-iterate what we will be doing.

Let us consider the set $A$ with $n$ number of elements. We form a relation $R: A \times A$. And now, we want to find the number of **reflexive** relations in $R$.

If you make a square matrix of order $n \times n$ (the same as the number of elements in $A$) and try to see where the reflexive relations lie:

$$
\begin{lgathered}
\begin{array}{c|c c c c c c}
 & a_{1} & a_{2} & a_{3} & a_{4}  & \textellipsis  & a_{n}\\
\hline 
a_{1}  & a_{1}Ra_{1} & . & . & . & . & .\\
a_{2}  & .  & a_{2}Ra_{2} & . & . & . & .\\
a_{3}  & .  & .  & a_{3}Ra_{3} & . & . & .\\
a_{4}  & . & . & . & a_{4}Ra_{4} & . & .\\
\dots  & . & . & . & . & \dots & .\\
a_{n} & .  & . & . & . & . & a_{n}Ra_{n}
\end{array}
\end{lgathered}
$$

You will see that the diagonal elements are reflexive. And there are $n$ diagonal elements. 

So, bro, shouldn't there be $n$ reflexive relations in $R$?

No. Why? We're getting there, son.

There are $n$ elements on each side. Thus, the total number of relations become $n^{2}$

$$
\begin{lgathered}
\underbrace{ \left. \begin{array}{c|c c c c c c}
 & a_{1} & a_{2} & a_{3} & a_{4}  & \textellipsis  & a_{n}\\
\hline 
a_{1}  & a_{1}Ra_{1} & . & . & . & . & .\\
a_{2}  & .  & a_{2}Ra_{2} & . & . & . & .\\
a_{3}  & .  & .  & a_{3}Ra_{3} & . & . & .\\
a_{4}  & . & . & . & a_{4}Ra_{4} & . & .\\
\dots  & . & . & . & . & \dots & .\\
a_{n} & .  & . & . & . & . & a_{n}Ra_{n}
\end{array} \\ \\ \right\} }_{ n \text{ elements} } \small n \text{ elements}
\end{lgathered}
$$

That makes $n^{2}-n$ non-diagonal elements.

Now, remember that we said that "a reflexive relation may or may not have pairs in the form of $(a,a)$"?

Well, you have $n^{2}-n$ elements waiting to be chosen. Or not.

Either way, you'll already have chosen the $n$ diagonal elements (since there is no other way).

If we had to say "To choose, or not to choose the $n^{2} - n$ elements?" in math:

We say:

$$
\begin{lgathered}
2^{n^{2}-n}
\end{lgathered}
$$

That's the number of reflexive relations. Or to be precise, that's the number of the *permutations*. 

Because it was a binary choice (meaning we had only 2 choices), we multiplied $2$ with itself $n^{2}-n$ times. 

I think this is pretty rad.