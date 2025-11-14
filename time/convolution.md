# Convolution

```{div} bigidea
**Convolution** describes how an LTI system transforms any input signal using its impulse response. The output is the convolution of the input with the impulse response.
```

## Convolution Integral

```{div} definition
**Continuous-Time Convolution**

For an LTI system with impulse response $h(t)$ and input $x(t)$, the output is:

$$
y(t) = x(t) * h(t) = \int_{-\infty}^{\infty} x(\tau)h(t-\tau) \, d\tau
$$
```

```{div} definition
**Discrete-Time Convolution**

For discrete-time signals:

$$
y[n] = x[n] * h[n] = \sum_{k=-\infty}^{\infty} x[k]h[n-k]
$$
```

## Properties of Convolution

```{div} theorem
**Convolution Properties**

Convolution is:

1. **Commutative**: $x * h = h * x$
2. **Associative**: $x * (h_1 * h_2) = (x * h_1) * h_2$
3. **Distributive**: $x * (h_1 + h_2) = x * h_1 + x * h_2$
```

## Computing Convolution

```{div} example
**Graphical Convolution**

To compute $y(t) = x(t) * h(t)$ graphically:

1. Reflect $h(\tau)$ about the vertical axis to get $h(-\tau)$
2. Shift by $t$ to get $h(t-\tau)$
3. Multiply $x(\tau)h(t-\tau)$ pointwise
4. Integrate over all $\tau$
```
