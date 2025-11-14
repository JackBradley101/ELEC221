# Laplace Transform

```{div} bigidea
The **Laplace transform** is a generalization of the Fourier transform that handles a wider class of signals and simplifies the analysis of LTI systems.
```

## Definition

```{div} definition
**Laplace Transform**

The Laplace transform of $x(t)$ is:

$$
X(s) = \mathcal{L}\{x(t)\} = \int_0^{\infty} x(t)e^{-st} \, dt
$$

where $s = \sigma + j\omega$ is a complex variable.
```

## Region of Convergence (ROC)

```{div} definition
**Region of Convergence**

The ROC is the set of values of $s$ for which the Laplace transform integral converges. The ROC is crucial for determining properties like causality and stability.
```

## Common Transform Pairs

```{div} example
**Common Laplace Transforms**

| Time Domain $x(t)$ | Laplace Domain $X(s)$ | ROC |
|-------------------|----------------------|-----|
| $\delta(t)$ | $1$ | All $s$ |
| $u(t)$ | $\frac{1}{s}$ | $\text{Re}(s) > 0$ |
| $e^{-at}u(t)$ | $\frac{1}{s+a}$ | $\text{Re}(s) > -a$ |
| $te^{-at}u(t)$ | $\frac{1}{(s+a)^2}$ | $\text{Re}(s) > -a$ |
| $\cos(\omega_0 t)u(t)$ | $\frac{s}{s^2 + \omega_0^2}$ | $\text{Re}(s) > 0$ |
```

## Properties

```{div} theorem
**Laplace Transform Properties**

| Property | Time Domain | Laplace Domain |
|----------|------------|----------------|
| Linearity | $ax(t) + by(t)$ | $aX(s) + bY(s)$ |
| Time Shift | $x(t - t_0)u(t - t_0)$ | $e^{-st_0}X(s)$ |
| Differentiation | $\frac{dx(t)}{dt}$ | $sX(s) - x(0^-)$ |
| Integration | $\int_0^t x(\tau)d\tau$ | $\frac{X(s)}{s}$ |
| Convolution | $x(t) * h(t)$ | $X(s)H(s)$ |
```
