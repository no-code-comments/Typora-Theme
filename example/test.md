# Typora Theme Preview File

## Basic Usage

### Paragraph

This paper is motivated by <u>the difficulty in deploying novel deep neural networks to embedded systems with limited hardware resources</u>. Although state-of-the-art deep neural networks can achieve extremely high performance, it requires **considerable storage** and **memory bandwidth** to normally execute, which is not suitable for deployment over light devices such as mobile systems, because of unacceptable large binary files and excessive energy consumption.

### List

Here are a collection of graph search algorithms

- **DFS** (Depth First Search)
- **BFS** (Breadth First Search)
- **UCS** (Uniform Cost Search)
- **A$^*$** (A$^*$ Search)

### Math

The loss function for binary classification is given by

$ \mathcal{L} = \dfrac{1}{N} \displaystyle \sum_{i = 1}^{N} \left[ -y_i \log \hat{y}_i - (1 - y_i) \log (1 - \hat{y}_i) \right] $

### Table

Comparison of common documentation tools are shown in the following table.

| **Tools** | **Language** | **Pros**                           | **Cons**                     |
| --------- | ------------ | ---------------------------------- | ---------------------------- |
| Typora    | Markdown     | real-time rendering, customization | not extensible               |
| VS Code   | Markdown     | integrated, extensible             | no real-time rendering       |
| LyX       | Latex        | real-time rendering                | no customization             |
| Overleaf  | Latex        | online working, shared documents   | network issue                |
| Word      | Word         | widely used                        | inefficient to type formulas |

### Code

File `./calc_max.py` implements the function of calculating max values for each column given a csv file.

```python
import pandas as pd

def calc_max_for_each_column(file_name):
    data = pd.read_csv(file_name)
    max_values = {key: data[key].max for key in data.keys()[1:]}
    return max_values
```

### Pseudo-code

> **<u>Algorithm 1 Euclidean Algorithm</u>**
>
> **Inputs:** $a, b \in \mathbb{R}$
>
> **Outputs:** the greatest common divisor of pair $(a, b)$
>
> ---
>
> **Function** $\texttt{gcd} (a, b)$
>
> > $r = a \ \operatorname{mod} \ b$
> >
> > **while** $r \neq 0$
> >
> > > $a = b$; $b = r$; $r = a \ \operatorname{mod} \ b$
> >
> > **return** $b$

