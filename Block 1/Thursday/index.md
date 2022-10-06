# WM160 Applied Maths I / Block 1 / Day 4 notes (2022-10-06)

## Independent events exercise

Given that $A$ and $B$ are independent, determine the values of $x$.

![](./venn.png)

$$
\begin{align*}
P(A \cap B') &= 0.3 \\
P(B \cap A') &= 0.2 \\
P(A \cap B) &= P(A) \times P(B) \\
x &= P(A \cap B) \\
x &= (0.3 + x)(0.2 + x) \\
x &= x^2 + 0.5x + 0.06 \\
x^2 - 0.5x + 0.06 &= 0 \\
x &= \begin{cases} 0.3 \\ 0.2 \end{cases} \\
\therefore P(A \cap B) &= \begin{cases} 0.3 \\ 0.2 \end{cases} \\
\end{align*}
$$

## Binomial distribution

Binomial distribution is a discrete probability distribution, which is useful in many applications and situations.

### Conditions for use

- number of trials must be fixed
- each trial may only have two potential outcomes (a success and failure)
- the trials must be independent
- the probability of success is identical in each trial

### Syntax

For a variable, $X$, which follows a binomial distribution, we write:

$$
X \sim B(n, p)
$$

where $n$ is the number of trials, and $p$ is the probability of a successful outcome.

For example, if $Y$ denotes the number of heads in 3 unbiased coin tosses, it would be:

$$
Y \sim B(3, 0.5)
$$

### Mean, variance and standard deviation

Where...

$$
\begin{align*}
X &\sim B(n, p) \\
n &= \text{number of trials} \\
p &= \text{P(success)} \\
q &= \text{P(failure)} \\
\end{align*}
$$

mean, variation and standard deviation can be calculated as followed:

$$
\begin{align*}
\text{mean} &\rightarrow E(X) = np \\
\text{variance} &\rightarrow \sigma^2 = npq \\
\text{standard deviation} &\rightarrow \sigma = \sqrt{npq} \\
\end{align*}
$$

### Probability of $r$ successful outcomes

**Individual binomial probabilities**

$$
P(X = r) = {n \choose r} p^r(1-p)^{n-r}
$$

**Cumulative binomial probabilities**

$$
P(X \leq x) = \sum^{x}_{r=0} {n \choose r} p^r(1-p)^{n-r}
$$

### Exercises

#### Exercise 1

> $X \sim B(8, 0.6)$
>
> Find the following probabilities:
>
> 1. $P(X = 0)$
> 2. $P(X = 3)$
> 3. $P(X = 6)$

$$
\begin{align*}
P(X = 0) &= {8 \choose 0}0.6^0(1-0.6)^{8-0} \\
&= {8 \choose 0}0.4^{8} \\
&= 0.4^{8} \\
P(X = 0) &\approx 0.000655 \text{ (3 s.f.)} \\
\end{align*}
$$

<br />

$$
\begin{align*}
P(X = 3) &= {8 \choose 3}0.6^3(1-0.6)^{8-3} \\
&= 56 \times 0.6^3 \times 0.4^5 \\
P(X = 3) &\approx 0.124 \text{ (3 s.f.)} \\
\end{align*}
$$

<br />

$$
\begin{align*}
P(X = 6) &= {8 \choose 6}0.6^6(1-0.6)^{8-6} \\
&= 28 \times 0.6^6 \times 0.4^2 \\
P(X = 6) &\approx 0.209 \text{ (3 s.f.)} \\
\end{align*}
$$
