# WM160 Applied Maths I / Block 1 / Day 3 notes (2022-10-05)

## Measures of spread (continued)

### Interquartile range

The interquartile range is the difference between the first quartile ( $Q_{1}$ ) and the third quartile ( $Q_{3}$ ).

$Q_1$ can be calculated by finding the median of the lower half of the sorted dataset (excluding the overall median).

$$
\begin{align*}
\{ 1, 2, 3, 4, 5, 6, 7 \} \\
Q_1 &= 2 \\
Q_2 &= 4 \\
Q_3 &= 6 \\
\text{IQR} = 6 - 2 &= 4 \\
\end{align*}
$$

We can use the IQR to find outliers in dataset. Typically, outliers can be defined as any value more than $1.5 \times \text{IQR}$ from the lower and upper quartiles. This can be shown as:

$$
x_{min} < Q_1 - 1.5 \times (Q_3 - Q-1) \\
x_{max} > Q_3 + 1.5 \times (Q_3 - Q-1) \\
$$

#### Box plots

Box plots are a way of representing a dataset and its spread.

A box plot of a dataset shows:

- the median
- the lower and upper quartiles
- the interquartile range
- the range (excluding outliers)
- outliers

An example labelled box plot is shown below:

![Example of a box plot, with its key elements labelled](box%20plot.png)

> This is a derivative work of RobSeb's `Elements of a boxplot.svg` [available on Wikimedia Commons](https://commons.wikimedia.org/wiki/File:Elements_of_a_boxplot.svg), licensed under CC-BY-SA 3.0. This derivative is also licensed under CC-BY-SA 3.0.
