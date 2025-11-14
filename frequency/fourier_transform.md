# Fourier Transform

```{div} bigidea
The **Fourier transform** extends Fourier analysis to aperiodic signals, representing any signal as a continuous spectrum of frequencies.
```

## Definition

```{div} definition
**Fourier Transform**

The Fourier transform of a signal $x(t)$ is:

$$
X(\omega) = \mathcal{F}\{x(t)\} = \int_{-\infty}^{\infty} x(t)e^{-j\omega t} \, dt
$$

The inverse Fourier transform is:

$$
x(t) = \mathcal{F}^{-1}\{X(\omega)\} = \frac{1}{2\pi}\int_{-\infty}^{\infty} X(\omega)e^{j\omega t} \, d\omega
$$
```

## Properties

```{div} theorem
**Fourier Transform Properties**

| Property | Time Domain | Frequency Domain |
|----------|------------|------------------|
| Linearity | $ax(t) + by(t)$ | $aX(\omega) + bY(\omega)$ |
| Time Shift | $x(t - t_0)$ | $X(\omega)e^{-j\omega t_0}$ |
| Frequency Shift | $x(t)e^{j\omega_0 t}$ | $X(\omega - \omega_0)$ |
| Scaling | $x(at)$ | $\frac{1}{|a|}X(\frac{\omega}{a})$ |
| Differentiation | $\frac{dx(t)}{dt}$ | $j\omega X(\omega)$ |
| Convolution | $x(t) * h(t)$ | $X(\omega)H(\omega)$ |
```

## Convolution Theorem

```{div} theorem
**Convolution Theorem**

Convolution in time domain is multiplication in frequency domain:

$$
y(t) = x(t) * h(t) \quad \Leftrightarrow \quad Y(\omega) = X(\omega)H(\omega)
$$

This is fundamental for analyzing LTI systems in the frequency domain.
```

```{div} example
**Rectangular Pulse**

For a rectangular pulse $x(t) = \text{rect}(t/T)$, the Fourier transform is:

$$
X(\omega) = T\text{sinc}\left(\frac{\omega T}{2\pi}\right)
$$

This shows the inverse relationship between time and frequency widths.
```
