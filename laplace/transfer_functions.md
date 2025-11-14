# Transfer Functions

```{div} bigidea
The **transfer function** $H(s)$ is the Laplace transform of the impulse response. It completely characterizes an LTI system and enables algebraic analysis.
```

## Definition

```{div} definition
**Transfer Function**

For an LTI system with impulse response $h(t)$:

$$
H(s) = \mathcal{L}\{h(t)\} = \frac{Y(s)}{X(s)}
$$

where $Y(s)$ and $X(s)$ are the Laplace transforms of the output and input with zero initial conditions.
```

## System Analysis

```{div} theorem
**Input-Output Relationship**

The output in the Laplace domain is:

$$
Y(s) = H(s)X(s)
$$

In time domain:

$$
y(t) = x(t) * h(t) = \mathcal{L}^{-1}\{H(s)X(s)\}
$$
```

## Poles and Zeros

```{div} definition
**Poles and Zeros**

For a rational transfer function:

$$
H(s) = \frac{N(s)}{D(s)} = K\frac{(s-z_1)(s-z_2)\cdots(s-z_m)}{(s-p_1)(s-p_2)\cdots(s-p_n)}
$$

* **Zeros** $z_i$ are roots of the numerator $N(s) = 0$
* **Poles** $p_i$ are roots of the denominator $D(s) = 0$
```

## Stability

```{div} theorem
**Stability from Poles**

An LTI system is BIBO stable if and only if all poles of $H(s)$ lie in the left-half of the complex plane (i.e., $\text{Re}(p_i) < 0$ for all poles $p_i$).
```

```{div} example
**First-Order System**

Consider an RC circuit with transfer function:

$$
H(s) = \frac{1}{1 + RCs}
$$

* Pole at $s = -\frac{1}{RC}$ (in left-half plane)
* System is stable
* Time constant $\tau = RC$
* Impulse response: $h(t) = \frac{1}{RC}e^{-t/RC}u(t)$
```

## Frequency Response

```{div} definition
**Frequency Response**

The frequency response is obtained by evaluating the transfer function on the imaginary axis:

$$
H(j\omega) = H(s)\bigg|_{s=j\omega}
$$

This describes the system's steady-state response to sinusoidal inputs.
```
