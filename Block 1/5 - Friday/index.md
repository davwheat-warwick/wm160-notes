# WM160 Applied Maths I / Block 1 / Day 5 notes (2022-10-07) <!-- omit in toc -->

## Contents <!-- omit in toc -->

- [Hypothesis testing](#hypothesis-testing)
  - [One-tailed tests](#one-tailed-tests)
  - [Two-tailed tests](#two-tailed-tests)
  - [Determining when to reject the null hypothesis](#determining-when-to-reject-the-null-hypothesis)
    - [p-value](#p-value)
    - [Critical region](#critical-region)
    - [Step-by-step](#step-by-step)
  - [Test exercises](#test-exercises)
    - [Question 1](#question-1)
    - [Question 2](#question-2)
    - [Question 3](#question-3)
    - [Question 4](#question-4)
    - [Question 5](#question-5)
    - [Question 6 - two-tailed](#question-6---two-tailed)

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

Where the **critical region** is one-sided, we are testing that a sample is greater than or less than, but not both. This could be a right-tailed or left-tailed test.

![](./one%20tailed%20test.png)

### Two-tailed tests

Where the **critical region** is split into two, we are testing that a sample is both greater than and less than predefined values.

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

#### Step-by-step

1. State the probability in context
2. Write down the null and alternative hypothesis
3. Write down the significance level, $\alpha$
4. Assume $H_0$ is true, and write down $B \sim B(n, p)$
5. Carry out necessary calculations
6. Make your decision: reject or fail to reject $H_0$
7. State the conclusion in the context of the problem

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
p = P(\text{roll a six}) = \frac{1}{6}
$$

$$
\begin{align*}
H_0&: p = \frac{1}{6} \\
H_1&: p < \frac{1}{6} \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of sixes in 20 throws.

$$
\begin{align*}
X &\sim B(20, \frac{1}{6}) \\
P(X \leq 1) &= 0.130 \text{ (3 s.f.)} \\
0.130 &> 0.05
\end{align*}
$$

$\therefore$ There is insufficient evidence to reject $H_0$.

There is insufficient evidence to suggest the die may be biased against rolling sixes.

#### Question 2

> Hassan complains that a dice he is using is biased so that he is more likely to get a 1 than any other number.
>
> He decides to test at the 10% significance level the hypothesis that the dice is biased towards a 1.
>
> 1. Write down the null and alternative hypothesis that Hassan will use.
>
> Hassan throws the dice 12 times and gets 5 ones.
>
> 2. Find the p-value for this test.
> 3. What is Hassan’s conclusion?

$$
p = P(\text{roll a one}) = \frac{1}{6}
$$

$$
\begin{align*}
H_0&: p = \frac{1}{6} \\
H_1&: p > \frac{1}{6} \\
\alpha &= 0.1
\end{align*}
$$

Let $X$ be the number of ones in 12 throws.

$$
\begin{align*}
X &\sim B(12, \frac{1}{6}) \\
P(X \geq 5) &= 1 - P(X \leq 4) \\
P(X \geq 5) &= 1 - 0.9636\dots \\
P(X \geq 5) &= 0.0363\dots \\
0.0363 \dots &< 0.1
\end{align*}
$$

$\therefore$ There is sufficient evidence to reject $H_0$.

$\therefore$ There is sufficient evidence to suggest the die may be biased towards rolling ones.

#### Question 3

> A bus company claims that a particular service is on time in 90% of journeys. I think it is less than this. I decide to test this at the 5% significance level.
>
> 1. Write down the null and alternative hypothesis that I should use.
>
> In my next 15 journeys, the bus is on time 10 times.
>
> 2. Find the p-value for this test.
> 3. What is my conclusion?

$$
p = P(\text{bus is on time}) = 0.9
$$

$$
\begin{align*}
H_0&: p = 0.9 \\
H_1&: p < 0.9 \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of times the bus is on time in 15 journeys.

$$
\begin{align*}
X &\sim B(15, 0.9) \\
P(X \leq 10) &= 0.0127\dots \\
0.0127\dots &< 0.05
\end{align*}
$$

$\therefore$ There is sufficient evidence to reject $H_0$.

$\therefore$ There is sufficient evidence to suggest that the company's buses arrive on time in fewer than 90% of journeys.

#### Question 4

> A school estimates the probability that a student gets an A or B pass in a Statistics exam to be 0.4.
>
> The school appoints a new teacher, who has never taught statistics before. The Head of Maths is concerned that the A and B pass-rate may decrease.
>
> Although all students passed in the following year, out of a group of 19 students only 2 got an A or B grade.
>
> Comment on the Head of Department’s concerns, by using a hypothesis test with a 5% significance level.

$$
p = P(\text{get grade A or B}) = 0.4
$$

$$
\begin{align*}
H_0&: p = 0.4 \\
H_1&: p < 0.4 \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of students who got grade A or B.

$$
\begin{align*}
X &\sim B(19, 0.4) \\
P(X \leq 2) &= 0.0054\dots \\
0.0054\dots &< 0.05
\end{align*}
$$

$\therefore$ There is sufficient evidence to reject $H_0$.

$\therefore$ There is sufficient evidence to suggest that the A and B pass-rate may have decreased.

#### Question 5

> Over a long period of time, it is found that a particular bus service is on time in 80% of journeys.
>
> The bus company claims that it has made improvements to the service and that the bus is now on time more often. I decide to test this at the 5% significance level.
>
> 1. Write down the null and alternative hypotheses that I should use.
>
> In my next 10 journeys, the bus is on time every time.
>
> 2. Find the p-value for this hypothesis test.
> 3. What is my conclusion?
> 4. Explain why this hypothesis test is unfair on the bus company, and state how many journeys I need to make so that it is possible that the null hypothesis could be rejected using the same significance level.

$$
p = P(\text{bus is on time}) = 0.8
$$

$$
\begin{align*}
H_0&: p = 0.8 \\
H_1&: p > 0.8 \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of buses that are on time.

$$
\begin{align*}
X &\sim B(10, 0.8) \\
P(X \geq 10) &= 1 - P(X \leq 9) \\
P(X \geq 10) &= 1 - 0.8926\dots \\
&= 0.1073\dots
\end{align*}
$$

p-level is $0.1073\dots$

$$
\begin{align*}
0.1073\dots &> 0.05
\end{align*}
$$

$\therefore$ There is insufficient evidence to reject $H_0$.

$\therefore$ There is insufficient evidence to suggest that the bus is on time more than 80% of the time.

This test is unfair as it requires more trials to more accurately determine whether $H_0$ should be rejected or not. In this test, the bus was on time every journey, but the null hypothesis was still rejected.

Since $P(\text{bus on time}) = 0.8$, and $\alpha = 0.05$:

$$\log_{0.8}(0.05) \approx 13.425$$

$\therefore$ The minimum number of trials for the null hypothesis to be rejected is $14$.

#### Question 6 - two-tailed

> Records from a school show that 2 out of 3 students got grades A to C in Mathematics.
>
> In the following year 16 out of 20 students get grades A to C.
>
> 1. The Head of Sixth form claimed at the start of the year that the results would be different because of a new tutor team. Test this claim at the 5% significance level.

$$
p = P(\text{get grade A to C}) = \frac{2}{3}
$$

$$
\begin{align*}
H_0&: p = \frac{2}{3} \\
H_1&: p \neq \frac{2}{3} \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of students who got grade A to C.

16 is in the upper tail, so we need to check the cumulative distribution from 16 to the end of the dataset, and compare this to the upper tail significance level.

$$
\begin{align*}
X &\sim B(20, \frac{2}{3}) \\
P(X \geq 16) &= 1 - P(X \leq 15)\dots \\
 &= 1 - 0.9395\dots \\
 &= 0.1515\dots \\
0.1515 &> 0.025
\end{align*}
$$

$\therefore$ There is insufficient evidence to reject $H_0$.

$\therefore$ There is insufficient evidence to suggest that the A to C pass-rate may have changed.

> 2. The Head of Mathematics claims this improvement is due to the appointment of a brilliant new teacher. Test this claim at the 5% significance level.

$$
\begin{align*}
H_0&: p = \frac{2}{3} \\
H_1&: p > \frac{2}{3} \\
\alpha &= 0.05
\end{align*}
$$

Let $X$ be the number of students who got grade A to C.

This test is one-tailed.

$$
\begin{align*}
X &\sim B(20, \frac{2}{3}) \\
P(X \geq 16) &= 1 - P(X \leq 15)\dots \\
 &= 1 - 0.9395\dots \\
 &= 0.1515\dots \\
0.1515 &> 0.05
\end{align*}
$$

$\therefore$ There is insufficient evidence to reject $H_0$.

$\therefore$ There is insufficient evidence to suggest that the A to C pass-rate may have increased due to the new teacher.
