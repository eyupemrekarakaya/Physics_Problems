## 11. Dynamics with a Time-Dependent Force

Given:

$$
\vec{F}(t) = (15t,\; 3t - 12,\; -6t^2)
$$

and mass:

$$
m = 3 \text{ kg}
$$

Initial conditions:

$$
\vec{r}(0) = (5, 2, -3), \quad \vec{v}(0) = (2, 0, 1)
$$

---

### 1. Acceleration

Using Newton’s second law:

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

$$
\vec{a}(t) = \left(\frac{15t}{3}, \frac{3t - 12}{3}, \frac{-6t^2}{3}\right)
$$

$$
\vec{a}(t) = (5t,\; t - 4,\; -2t^2)
$$

---

### 2. Velocity

Velocity is the integral of acceleration:

#### x-component

$$
v_x(t) = \int 5t\,dt = \frac{5}{2}t^2 + C_1
$$

Using $v_x(0) = 2$:

$$
C_1 = 2
$$

$$
v_x(t) = \frac{5}{2}t^2 + 2
$$

---

#### y-component

$$
v_y(t) = \int (t - 4)\,dt = \frac{1}{2}t^2 - 4t + C_2
$$

Using $v_y(0) = 0$:

$$
C_2 = 0
$$

$$
v_y(t) = \frac{1}{2}t^2 - 4t
$$

---

#### z-component

$$
v_z(t) = \int (-2t^2)\,dt = -\frac{2}{3}t^3 + C_3
$$

Using $v_z(0) = 1$:

$$
C_3 = 1
$$

$$
v_z(t) = -\frac{2}{3}t^3 + 1
$$

---

### Velocity Vector

$$
\vec{v}(t) = \left(\frac{5}{2}t^2 + 2,\; \frac{1}{2}t^2 - 4t,\; -\frac{2}{3}t^3 + 1\right)
$$

---

### 3. Position

Position is the integral of velocity:

#### x-component

$$
x(t) = \int \left(\frac{5}{2}t^2 + 2\right) dt
$$

$$
x(t) = \frac{5}{6}t^3 + 2t + C_4
$$

Using $x(0) = 5$:

$$
C_4 = 5
$$

$$
x(t) = \frac{5}{6}t^3 + 2t + 5
$$

---

#### y-component

$$
y(t) = \int \left(\frac{1}{2}t^2 - 4t\right) dt
$$

$$
y(t) = \frac{1}{6}t^3 - 2t^2 + C_5
$$

Using $y(0) = 2$:

$$
C_5 = 2
$$

$$
y(t) = \frac{1}{6}t^3 - 2t^2 + 2
$$

---

#### z-component

$$
z(t) = \int \left(-\frac{2}{3}t^3 + 1\right) dt
$$

$$
z(t) = -\frac{1}{6}t^4 + t + C_6
$$

Using $z(0) = -3$:

$$
C_6 = -3
$$

$$
z(t) = -\frac{1}{6}t^4 + t - 3
$$

---

### Final Answers

Velocity:

$$
\vec{v}(t) = \left(\frac{5}{2}t^2 + 2,\; \frac{1}{2}t^2 - 4t,\; -\frac{2}{3}t^3 + 1\right)
$$

Position:

$$
\vec{r}(t) = \left(\frac{5}{6}t^3 + 2t + 5,\; \frac{1}{6}t^3 - 2t^2 + 2,\; -\frac{1}{6}t^4 + t - 3\right)
$$
