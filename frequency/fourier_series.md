# Fourier Series

```{div} bigidea
**Fourier series** represents periodic signals as sums of sinusoids (or complex exponentials). This decomposes a signal into its frequency components.
```

## Trigonometric Fourier Series

```{div} definition
**Fourier Series Representation**

A periodic signal $x(t)$ with period $T$ can be expressed as:

$$
x(t) = a_0 + \sum_{n=1}^{\infty} \left[a_n \cos(n\omega_0 t) + b_n \sin(n\omega_0 t)\right]
$$

where $\omega_0 = \frac{2\pi}{T}$ is the fundamental frequency.
```

## Exponential Fourier Series

```{div} definition
**Complex Exponential Form**

Using Euler's formula, the Fourier series can be written as:

$$
x(t) = \sum_{n=-\infty}^{\infty} c_n e^{jn\omega_0 t}
$$

where the Fourier coefficients are:

$$
c_n = \frac{1}{T} \int_0^T x(t)e^{-jn\omega_0 t} \, dt
$$
```

## Properties

```{div} theorem
**Parseval's Theorem**

For periodic signals:

$$
\frac{1}{T}\int_0^T |x(t)|^2 \, dt = \sum_{n=-\infty}^{\infty} |c_n|^2
$$

This states that power in time domain equals power in frequency domain.
```

```{div} example
**Square Wave**

A square wave with period $T$ has Fourier series:

$$
x(t) = \frac{4}{\pi} \sum_{n=1,3,5,...}^{\infty} \frac{1}{n}\sin(n\omega_0 t)
$$

Notice only odd harmonics are present due to symmetry.
```
