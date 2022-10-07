# WM160 Applied Maths I / Block 1 / Day 5 notes (2022-10-07) <!-- omit in toc -->

## Contents <!-- omit in toc -->

- [Hypothesis testing](#hypothesis-testing)
  - [One-tailed tests](#one-tailed-tests)
  - [Two-tailed tests](#two-tailed-tests)
  - [Determining when to reject the null hypothesis](#determining-when-to-reject-the-null-hypothesis)
    - [p-value](#p-value)
    - [Critical region](#critical-region)
  - [Test exercises](#test-exercises)
    - [Question 1](#question-1)

## Hypothesis testing

A **hypothesis** is a statement that may or may not be true.

A hypothesis test is used to test a claim and draw conclusions about the value of a parameter.

The **null hypothesis** ( $H_0$ ) is the initial assumption, always assumed to be true.

The **alternative hypothesis** ( $H_1$ or $H_a$ ) is the opposite of the null hypothesis, and is what is being tested for.

The **critical region** is the area the sample tested must land in to reject the null hypothesis.

The **critical value(s)** is/are the first value(s) in the critical region.

The **significance level** ( $\alpha$ ) determines the size of the critical region during the hypothesis testing.

The **p-value** ( $p$ ) is the probability of an observed value. It is the probability of finding the observed results when the null hypothesis is true.

$$
\begin{align*}
H_0 &= \text{null hypothesis} \\
H_1 &= \text{alternative hypothesis} \\
H_1 &= \text{alternative hypothesis} \\
\end{align*}
$$

**For example:**

> A manufacturing firm observes that the proportion of defective products in one of its distribution lines is 3%.

The null hypothesis, since we assume that the probability of a defective product is 3%, would be:

$$
H_0: p = 0.03
$$

The alternative hypothesis would take one of these forms:

$$
\begin{align*}
H_1&: p \neq 0.03 \\
H_1&: p \lt 0.03 \\
H_1&: p \gt 0.03
\end{align*}
$$

### One-tailed tests

Where the **critical region** is one-sided, testing that a sample is greater than or less than, but not both. This could be a right-tailed or left-tailed test.

![](./one%20tailed%20test.png)

### Two-tailed tests

Where the **critical region** is split into two, testing that a sample is both greater than and less than predefined values.

The significance level is equally split on either side of the tails. For example, an SL of $5\%$ would be split into $2.5\%$ on the left region, and another $2.5\%$ on the right region.

### Determining when to reject the null hypothesis

#### p-value

We compare the computed p-value with $\alpha$:

- if $p \leq \alpha$, we **reject** $H_0$ (it is statistically significant)
- if $p \gt \alpha$, we **fail to reject** $H_0$ (it is not statistically significant)

#### Critical region

We can also compare the observed value with the critical region:

- if the value falls inside the critical region, we **reject** $H_0$
- if the value falls outside the critical region, we **fail to reject** $H_0$

### Test exercises

#### Question 1

> Jessica complains that a dice she is using is biased so that she is less likely to get a 6.
>
> She decides to test at the 5% significance level the hypothesis that the dice is biased against a six.
>
> 1. Write down the null and alternative hypothesis that Jessica will use.
>
> Jessica throws the dice 20 times and gets just one six.
>
> 2. Find the p-value for this test.
> 3. What is Jessica’s conclusion?

$$
H_0
$$
