# Impulse Response

```{div} bigidea
The **impulse response** $h(t)$ completely characterizes an LTI system. It is the output when the input is a unit impulse $\delta(t)$.
```

## Definition

```{div} definition
**Impulse Response**

For an LTI system $\mathcal{T}$, the impulse response is:

$$
h(t) = \mathcal{T}\{\delta(t)\}
$$

For discrete-time systems:

$$
h[n] = \mathcal{T}\{\delta[n]\}
$$
```

## Properties

The impulse response provides complete information about the system:

* **Stability**: A system is BIBO stable if $\int_{-\infty}^{\infty} |h(t)| \, dt < \infty$
* **Causality**: A system is causal if $h(t) = 0$ for $t < 0$
* **Memory**: A system is memoryless if $h(t) = k\delta(t)$ for some constant $k$

```{div} example
**RC Circuit**

For an RC circuit with impulse response:

$$
h(t) = \frac{1}{RC}e^{-t/RC}u(t)
$$

This system is:
* Causal (since $h(t) = 0$ for $t < 0$)
* Stable (since the integral of $|h(t)|$ converges)
* Has memory (depends on past inputs)
```
