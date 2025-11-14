# Introduction to Signals

```{div} bigidea
A **signal** is a function that conveys information about a physical phenomenon. Signals can be continuous-time or discrete-time.
```

## Continuous-Time Signals

A continuous-time signal $x(t)$ is defined for all values of time $t$ in some interval.

```{div} example
**Common Continuous-Time Signals**

* Unit step: $u(t) = \begin{cases} 1 & t \geq 0 \\ 0 & t < 0 \end{cases}$
* Exponential: $x(t) = e^{at}$
* Sinusoidal: $x(t) = A\cos(\omega t + \phi)$
```

## Discrete-Time Signals

A discrete-time signal $x[n]$ is defined only at discrete time instants, typically integers $n$.

```{div} definition
**Unit Impulse**

The discrete-time unit impulse (or unit sample) is defined as:

$$
\delta[n] = \begin{cases} 1 & n = 0 \\ 0 & n \neq 0 \end{cases}
$$
```

## Energy and Power

```{div} definition
**Signal Energy**

The energy of a continuous-time signal $x(t)$ is:

$$
E = \int_{-\infty}^{\infty} |x(t)|^2 \, dt
$$

For discrete-time signals:

$$
E = \sum_{n=-\infty}^{\infty} |x[n]|^2
$$
```
