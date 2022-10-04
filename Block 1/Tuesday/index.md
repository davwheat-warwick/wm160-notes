# WM160 Applied Maths I / Block 1 / Day 2 notes (2022-10-04)

## Contents

- [WM160 Applied Maths I / Block 1 / Day 2 notes (2022-10-04)](#wm160-applied-maths-i--block-1--day-2-notes-2022-10-04)
  - [Contents](#contents)
  - [Measures of centre](#measures-of-centre)
    - [Mid-range](#mid-range)
    - [Frequency tables](#frequency-tables)
      - [Mean](#mean)
      - [Median](#median)

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
\sum{f}=11
\\
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
