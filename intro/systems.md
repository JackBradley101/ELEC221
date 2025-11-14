# Introduction to Systems

```{div} bigidea
A **system** is a process that transforms an input signal into an output signal. We denote a system by $\mathcal{T}$ such that $y = \mathcal{T}\{x\}$ where $x$ is the input and $y$ is the output.
```

## Linear Time-Invariant (LTI) Systems

```{div} definition
**Linear System**

A system is **linear** if it satisfies:

1. **Additivity**: $\mathcal{T}\{x_1 + x_2\} = \mathcal{T}\{x_1\} + \mathcal{T}\{x_2\}$
2. **Homogeneity**: $\mathcal{T}\{ax\} = a\mathcal{T}\{x\}$ for any scalar $a$
```

```{div} definition
**Time-Invariant System**

A system is **time-invariant** if a time shift in the input causes an equal time shift in the output:

$$
\mathcal{T}\{x(t - t_0)\} = y(t - t_0)
$$
```

## System Properties

```{div} theorem
**Causality**

A system is **causal** if the output at any time depends only on present and past inputs, not future inputs.
```

```{div} example
**Causal vs Non-Causal**

* Causal: $y(t) = x(t) + x(t-1)$
* Non-causal: $y(t) = x(t) + x(t+1)$
```
