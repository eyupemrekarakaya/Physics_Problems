## 9. Vertical Throw with Drag

We are given the equation of motion:

$$
m\frac{dv}{dt} = -mg - kv
$$

with initial conditions

$$
v(0) = v_0, \qquad x(0) = 10
$$

---

### 1. Analytical Solution

First rewrite the equation:

$$
\frac{dv}{dt} + \frac{k}{m}v = -g
$$

This is a first-order linear differential equation.

The solution for velocity is:

$$
v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}
$$

---

### 2. Position as a Function of Time

Since

$$
v = \frac{dx}{dt}
$$

we integrate:

$$
x(t) = x(0) + \int_0^t v(s)\,ds
$$

Substituting the velocity expression:

$$
x(t) = 10 + \int_0^t \left[\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}s} - \frac{mg}{k}\right] ds
$$

Carrying out the integration:

$$
x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t
$$

So the full analytical solution is:

$$
v(t) = \left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t} - \frac{mg}{k}
$$

$$
x(t) = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t}\right) - \frac{mg}{k}t
$$

---

### 3. Maximum Height

The maximum height occurs when the velocity becomes zero:

$$
v(t_{\max}) = 0
$$

So,

$$
\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{\max}} - \frac{mg}{k} = 0
$$

$$
\left(v_0 + \frac{mg}{k}\right)e^{-\frac{k}{m}t_{\max}} = \frac{mg}{k}
$$

$$
e^{-\frac{k}{m}t_{\max}} = \frac{\frac{mg}{k}}{v_0 + \frac{mg}{k}}
$$

Taking the natural logarithm:

$$
t_{\max} = \frac{m}{k}\ln\left(\frac{v_0 + \frac{mg}{k}}{\frac{mg}{k}}\right)
$$

$$
t_{\max} = \frac{m}{k}\ln\left(1 + \frac{k v_0}{mg}\right)
$$

Then the maximum height is:

$$
x_{\max} = x(t_{\max})
$$

Thus,

$$
x_{\max} = 10 + \frac{m}{k}\left(v_0 + \frac{mg}{k}\right)\left(1 - e^{-\frac{k}{m}t_{\max}}\right) - \frac{mg}{k}t_{\max}
$$

Using the relation for $e^{-\frac{k}{m}t_{\max}}$, this can also be simplified to:

$$
x_{\max} = 10 + \frac{m v_0}{k} - \frac{m^2 g}{k^2}\ln\left(1 + \frac{k v_0}{mg}\right)
$$

---

### 4. Comparison with the Case Without Drag

Without drag, the equation becomes:

$$
m\frac{dv}{dt} = -mg
$$

so

$$
\frac{dv}{dt} = -g
$$

The solutions are:

$$
v(t) = v_0 - gt
$$

$$
x(t) = 10 + v_0 t - \frac{1}{2}gt^2
$$

The maximum height is reached when $v=0$:

$$
t_{\max} = \frac{v_0}{g}
$$

and therefore

$$
x_{\max} = 10 + \frac{v_0^2}{2g}
$$

So compared with the no-drag case:

- the upward velocity decreases faster,
- the time to reach the top is shorter,
- the maximum height is smaller.

---

### 5. Numerical Simulation in Python

A simple numerical simulation can be done using Euler’s method:

```python
import numpy as np
import matplotlib.pyplot as plt

# Parameters
m = 1.0
k = 0.5
g = 9.8
v0 = 20.0
x0 = 10.0

# Time settings
dt = 0.01
t_max = 5
t_values = np.arange(0, t_max, dt)

# Arrays
x_values = []
v_values = []

# Initial conditions
x = x0
v = v0

for t in t_values:
    x_values.append(x)
    v_values.append(v)

    # dv/dt = -g - (k/m)v
    a = -g - (k/m) * v
    v = v + a * dt
    x = x + v * dt

plt.plot(t_values, x_values, label="x(t)")
plt.xlabel("Time (s)")
plt.ylabel("Height (m)")
plt.title("Vertical Throw with Drag")
plt.legend()
plt.grid(True)
plt.show()
