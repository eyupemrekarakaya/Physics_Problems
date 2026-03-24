## 10. Force Field and Power

The position of the particle is given by:

$$
x(t) = 5t^2 - t
$$

$$
y(t) = 2t^3
$$

$$
z(t) = -3t + 2
$$

and the mass is

$$
m = 0.5 \text{ kg}
$$

---

### 1. Velocity

Velocity is the time derivative of position:

$$
v_x(t) = \frac{dx}{dt} = 10t - 1
$$

$$
v_y(t) = \frac{dy}{dt} = 6t^2
$$

$$
v_z(t) = \frac{dz}{dt} = -3
$$

So the velocity vector is

$$
\vec{v}(t) = (10t - 1)\hat{i} + 6t^2\hat{j} - 3\hat{k}
$$

---

### 2. Momentum

Momentum is

$$
\vec{p}(t) = m\vec{v}(t)
$$

Substituting $m = 0.5$:

$$
\vec{p}(t) = 0.5\left[(10t - 1)\hat{i} + 6t^2\hat{j} - 3\hat{k}\right]
$$

$$
\vec{p}(t) = (5t - 0.5)\hat{i} + 3t^2\hat{j} - 1.5\hat{k}
$$

---

### 3. Acceleration

Acceleration is the derivative of velocity:

$$
a_x(t) = \frac{d^2x}{dt^2} = 10
$$

$$
a_y(t) = \frac{d^2y}{dt^2} = 12t
$$

$$
a_z(t) = \frac{d^2z}{dt^2} = 0
$$

Thus,

$$
\vec{a}(t) = 10\hat{i} + 12t\hat{j} + 0\hat{k}
$$

---

### 4. Force

Using Newton’s second law:

$$
\vec{F}(t) = m\vec{a}(t)
$$

$$
\vec{F}(t) = 0.5(10\hat{i} + 12t\hat{j} + 0\hat{k})
$$

$$
\vec{F}(t) = 5\hat{i} + 6t\hat{j}
$$

---

### 5. Power

Power delivered by the force field is

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t)
$$

Substitute:

$$
\vec{F}(t) = (5, 6t, 0)
$$

$$
\vec{v}(t) = (10t - 1, 6t^2, -3)
$$

Now compute the dot product:

$$
P(t) = 5(10t - 1) + (6t)(6t^2) + 0(-3)
$$

$$
P(t) = 50t - 5 + 36t^3
$$

So,

$$
P(t) = 36t^3 + 50t - 5
$$

---

### Final Answers

Velocity:

$$
\vec{v}(t) = (10t - 1)\hat{i} + 6t^2\hat{j} - 3\hat{k}
$$

Momentum:

$$
\vec{p}(t) = (5t - 0.5)\hat{i} + 3t^2\hat{j} - 1.5\hat{k}
$$

Acceleration:

$$
\vec{a}(t) = 10\hat{i} + 12t\hat{j}
$$

Force:

$$
\vec{F}(t) = 5\hat{i} + 6t\hat{j}
$$

Power:

$$
P(t) = 36t^3 + 50t - 5
$$
