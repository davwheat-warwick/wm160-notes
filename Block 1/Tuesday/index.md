# WM160 Applied Maths I / Block 1 / Day 2 notes (2022-10-04)

## Contents

- [WM160 Applied Maths I / Block 1 / Day 2 notes (2022-10-04)](#wm160-applied-maths-i--block-1--day-2-notes-2022-10-04)
  - [Contents](#contents)
  - [Measures of centre](#measures-of-centre)
    - [Mid-range](#mid-range)
    - [Frequency tables](#frequency-tables)
      - [Mean](#mean)
      - [Median](#median)
  - [Measures of spread](#measures-of-spread)
    - [Variance](#variance)
    - [Standard deviation](#standard-deviation)
      - [Equation](#equation)
      - [Example](#example)
      - [Example 2](#example-2)
      - [Example 3 - Population](#example-3---population)
      - [Example 4 - classes and inequalities](#example-4---classes-and-inequalities)

## Measures of centre

### Mid-range

The mid-range of a set of values is the mean average of the smallest and largest value in the dataset.

$$
\text{dataset} = \{ 1, 3, 3, 4, 7 \}
$$

With the example dataset above, we can see how this would be calculated.

$$
\text{mid-range} = \frac{1 + 7}{2} = 4
$$

### Frequency tables

We can estimate measures of centre from a frequency table.

| $x$ (data) | $f$ (frequency) |
| :--------: | :-------------: |
|    $3$     |       $5$       |
|    $5$     |       $1$       |
|    $7$     |       $2$       |
|    $8$     |       $3$       |

#### Mean

The mean can be represented as such:

$$
\text{mean of }x=\bar{x}
$$

$$
\bar{x} = \frac{\sum{fx}}{\sum{f}}
$$

This means that the mean of $x$ is equal to the sum of $f \times x$ (data multiplied by frequency), divided by the total frequency.

| $x$ (data) | $f$ (frequency) | $fx$          |
| :--------: | :-------------: | ------------- |
|    $3$     |       $5$       | $3\times5=15$ |
|    $5$     |       $1$       | $5\times1=5$  |
|    $7$     |       $2$       | $7\times2=14$ |
|    $8$     |       $3$       | $8\times3=24$ |

$$
\sum{f}=11 \\
\sum{fx}=15+5+14+24=58
$$

From this, we can now calculate the mean, which would be $\frac{58}{11}$, which is approximately $5.27$.

#### Median

The median is simpler than the mean. We need to know the total frequency ( $\sum{f}$ ), then add one, and divide by two. This tells us what position the median is within the dataset.

This is easiest with by adding a new cumulative frequency column to our table.

| $x$ (data) | $f$ (frequency) | cumulative frequency |
| :--------: | :-------------: | :------------------: |
|    $3$     |       $5$       |          5           |
|    $5$     |       $1$       |          6           |
|    $7$     |       $2$       |          8           |
|    $8$     |       $3$       |          11          |

In this example, our median is at position $6$ ( $\frac{11 + 1}{2} = 6$ ), so we find where $6$ fits into our cumulative frequency entries.

You can do this by finding the place where the position ( $6$ ) is greater than the cumulative frequency entry, then choose the entry before.

If we look at the first row, the cumulative frequency is $5$. $6$ is not greater than $5$, so we look at the next row. $6$ is not greater than $6$, so we look at the next row. $8$ is greater than $6$, so we look at the row before this.

| $x$ (data) | $f$ (frequency) | cumulative frequency |
| :--------: | :-------------: | :------------------: |
|    $5$     |       $1$       |          6           |

Our median is then the value of $x$ for this row, which is $5$.

## Measures of spread

### Variance

$$
\sigma^2 = \text{variance}
$$

$$
\sigma^2=\frac{\sum{x^2}-n\bar{x}^2}{n-1}
$$

### Standard deviation

#### Equation

$$
\sigma = \text{standard deviation}
$$

$$
\text{Sample: } \sigma^2=\frac{\sum{x^2}-n\bar{x}^2}{n-1}
$$

$$
\text{Population: } \sigma^2=\frac{\sum{x^2}-n\bar{x}^2}{n}
$$

#### Example

$$
\text{example dataset} = \{ 0,0,1,1,1,2,3 \}
$$

$$
\sigma^2=\frac{\sum{x^2}-n\bar{x}^2}{n-1}
$$

Using our dataset, we can calculate the value of $n$ (count of items in dataset) and $\bar{x}$ (the mean of the dataset).

$$
\begin{align*}
n &= 7 \\
\bar{x} &= \frac{1+1+1+2+3}{7} = \frac{8}{7} \\
\end{align*}
$$

Using these values, we can now calculate the variance and sample standard deviation of the dataset.

$$
\begin{align*}
\sigma^2 &= \frac{(1^2+1^2+1^2+2^2+3^2)-7(\frac{8}{7})^2}{7-1} \\
\sigma^2 &=  \frac{16 - \frac{64}{7}}{6} \\
\sigma^2 &= \frac{8}{7} \\
\sigma &= \sqrt{\frac{8}{7}} \\
\sigma &\approx 1.07 \text{ (3 s.f.)}
\end{align*}
$$

#### Example 2

$$
\text{A set of sample data is summarised as:} \\
\begin{align*}
n &= 100 \\
\sum{x} &= 1420 \\
\sum{x^2} &= 22125
\end{align*} \\
\text{Find the mean and standard deviation.}
$$

The mean is relatively straightforward to calculate, since we have the value of $n$ and $\sum{x}$. In this case, we can simply do:

$$
\begin{align*}
\bar{x} &= \frac{\sum{x}}{n} \\
&= \frac{1420}{100} \\
&= 14.2
\end{align*}
$$

For the standard deviation, we need to use the sample standard deviation formula again, inserting the values provided in the question, and our mean calculation.

$$
\begin{align*}
\sigma^2 &= \frac{\sum{x^2}-n\bar{x}^2}{n-1} \\
\sigma^2 &= \frac{22125 - (100)(14.2)^2}{100-1} \\
\sigma^2 &= \frac{22125 - 20164}{99} \\
\sigma^2 &= \frac{1961}{99} \\
\sigma &= \sqrt{\frac{1961}{99}} \\
\sigma &\approx 4.45 \text{ (3 s.f.)} \\
\end{align*}
$$

#### Example 3 - Population

| Number of occupants, $x$ | Frequency, $f$ |
| :----------------------: | :------------: |
|            1             |       26       |
|            2             |       34       |
|            3             |       19       |
|            4             |       57       |
|            5             |       42       |
|            6             |       12       |
|            7             |       3        |
|            8             |       1        |

$$
\text{Find the mean and population standard deviation of this dataset.}
$$

We first start by calculating the mean. This is most easily done by calculating the value of $fx$ for each row of the table.

| Number of occupants, $x$ | Frequency, $f$ | $fx$ |
| :----------------------: | :------------: | :--: |
|            1             |       26       |  26  |
|            2             |       34       |  68  |
|            3             |       19       |  57  |
|            4             |       57       | 228  |
|            5             |       42       | 210  |
|            6             |       12       |  72  |
|            7             |       3        |  21  |
|            8             |       1        |  8   |
|        **Totals**        |      194       | 690  |

We can represent the mean by the sum of $fx$, divided by $f$:

$$
\begin{align*}
\bar{x} &= \frac{\sum{fx}}{\sum{f}} \\
\bar{x} &= \frac{690}{194} \\
\bar{x} &= \frac{345}{97}
\end{align*}
$$

Now we know the mean, we can work out the population standard deviation.

$$
\begin{align*}
\sigma^2 &= \frac{\sum{(fx^2)} - (\sum{f})\bar{x}^2}{\sum{f}}
\end{align*}
$$

We need to work out the value of $fx^2$ for each row in the dataset, as well as the sum of these for the dataset as a whole.

| Number of occupants, $x$ | Frequency, $f$ | $fx$ | $x^2$ | $fx^2$ |
| :----------------------: | :------------: | :--: | :---: | :----: |
|            1             |       26       |  26  |   1   |   26   |
|            2             |       34       |  68  |   4   |  136   |
|            3             |       19       |  57  |   9   |  171   |
|            4             |       57       | 228  |  16   |  912   |
|            5             |       42       | 210  |  25   |  1050  |
|            6             |       12       |  72  |  36   |  432   |
|            7             |       3        |  21  |  49   |  147   |
|            8             |       1        |  8   |  64   |   64   |
|        **Totals**        |      194       | 690  |  N/A  |  2938  |

From this updated table, we can complete the formula:

$$
\begin{align*}
\sigma^2 &= \frac{\sum{(fx^2)} - (\sum{f})\bar{x}^2}{\sum{f}} \\
\sigma^2 &= \frac{2938 - (194)(\frac{345}{97})^2}{194} \\
\sigma^2 &= \frac{2938 - \frac{238050}{97}}{194} \\
\sigma^2 &= \frac{\frac{46936}{97}}{194} \\
\sigma^2 &= \frac{46936}{18818} \\
\sigma^2 &\approx 2.49 \text{ (3 s.f.)} \\
\sigma &= \sqrt{\frac{46936}{18818}} \\
\sigma &\approx 1.58 \text{ (3 s.f.)} \\
\end{align*}
$$

#### Example 4 - classes and inequalities

We use the same method as above for datasets using classes, instead defining $x$ as the midpoint of the class.

Remember, this means that we need to include the bounds that round to the value, too. For example $1.5 \geq x > 2$ includes $1.45$ to $1.95$.
