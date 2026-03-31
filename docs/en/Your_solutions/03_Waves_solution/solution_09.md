## 9. Damped Oscillator

Given:

$$
m\frac{d^2x}{dt^2} + b\frac{dx}{dt} + kx = 0
$$

---

### General Solution

Define:

$$
\Delta = b^2 - 4mk
$$

---

### Cases

- **Underdamped** ($\Delta < 0$):

$$
x(t) = e^{-\frac{b}{2m}t}(C_1\cos(\omega t) + C_2\sin(\omega t))
$$

where

$$
\omega = \sqrt{\frac{4mk - b^2}{4m^2}}
$$

---

- **Critically damped** ($\Delta = 0$):

$$
x(t) = (C_1 + C_2 t)e^{-\frac{b}{2m}t}
$$

---

- **Overdamped** ($\Delta > 0$):

$$
x(t) = C_1 e^{r_1 t} + C_2 e^{r_2 t}
$$

where

$$
r_{1,2} = \frac{-b \pm \sqrt{b^2 - 4mk}}{2m}
$$

---

### Summary

- Underdamped → oscillatory decay  
- Critically damped → fastest return to equilibrium  
- Overdamped → slow, no oscillation
