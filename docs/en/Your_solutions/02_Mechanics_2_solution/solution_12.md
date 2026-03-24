## 12. Work and Energy with a Constant Force

Given:

$$
m = 2 \text{ kg}
$$

$$
\vec{F} = [6, 2] \text{ N}
$$

Initial conditions:

$$
\vec{v}(0) = (1, -1) \text{ m/s}
$$

$$
\vec{r}(0) = (0, 0) \text{ m}
$$

---

### 1. Acceleration

Using Newton’s second law:

$$
\vec{a} = \frac{\vec{F}}{m}
$$

$$
\vec{a} = \left(\frac{6}{2}, \frac{2}{2}\right)
$$

$$
\vec{a}(t) = (3, 1) \text{ m/s}^2
$$

---

### 2. Velocity

Velocity is obtained by integrating acceleration:

$$
\vec{v}(t) = \vec{v}(0) + \vec{a}t
$$

$$
\vec{v}(t) = (1, -1) + (3, 1)t
$$

$$
\vec{v}(t) = (1 + 3t,\; -1 + t) \text{ m/s}
$$

---

### 3. Position

Position is obtained by integrating velocity:

$$
\vec{r}(t) = \vec{r}(0) + \vec{v}(0)t + \frac{1}{2}\vec{a}t^2
$$

$$
\vec{r}(t) = (0,0) + (1,-1)t + \frac{1}{2}(3,1)t^2
$$

$$
\vec{r}(t) = \left(t + \frac{3}{2}t^2,\; -t + \frac{1}{2}t^2\right) \text{ m}
$$

So the components are:

$$
x(t) = t + \frac{3}{2}t^2
$$

$$
y(t) = -t + \frac{1}{2}t^2
$$

---

### 4. Trajectory

From

$$
x(t) = t + \frac{3}{2}t^2
$$

$$
y(t) = -t + \frac{1}{2}t^2
$$

the trajectory is a parabola in the plane.

At some sample times:

$$
t=0 \Rightarrow (x,y)=(0,0)
$$

$$
t=1 \Rightarrow (x,y)=\left(2.5,-0.5\right)
$$

$$
t=2 \Rightarrow (x,y)=(8,0)
$$

$$
t=3 \Rightarrow (x,y)=\left(16.5,1.5\right)
$$

So the particle first moves downward, then curves upward under the constant force.

---

### 5. Work Done by the Force at $t=3$ s

First find the displacement at $t=3$:

$$
\vec{r}(3) = \left(3 + \frac{3}{2}(9),\; -3 + \frac{1}{2}(9)\right)
$$

$$
\vec{r}(3) = (16.5,\; 1.5)
$$

Since the initial position is $(0,0)$, the displacement is:

$$
\Delta \vec{r} = (16.5,\; 1.5)
$$

Work done by the constant force:

$$
W = \vec{F} \cdot \Delta \vec{r}
$$

$$
W = (6,2)\cdot(16.5,1.5)
$$

$$
W = 6(16.5) + 2(1.5)
$$

$$
W = 99 + 3
$$

$$
W = 102 \text{ J}
$$

---

### 6. Check with the Work-Energy Theorem

Initial kinetic energy:

$$
K_i = \frac{1}{2}m v_0^2
$$

where

$$
v_0^2 = 1^2 + (-1)^2 = 2
$$

so

$$
K_i = \frac{1}{2}(2)(2) = 2 \text{ J}
$$

Now find the velocity at $t=3$:

$$
\vec{v}(3) = (1+3\cdot3,\; -1+3)
$$

$$
\vec{v}(3) = (10,2)
$$

Thus,

$$
v^2 = 10^2 + 2^2 = 104
$$

Final kinetic energy:

$$
K_f = \frac{1}{2}(2)(104) = 104 \text{ J}
$$

Change in kinetic energy:

$$
\Delta K = K_f - K_i
$$

$$
\Delta K = 104 - 2 = 102 \text{ J}
$$

Since

$$
W = \Delta K = 102 \text{ J}
$$

the work-energy theorem is verified.

---

### Final Answers

Acceleration:

$$
\vec{a}(t) = (3,1) \text{ m/s}^2
$$

Velocity:

$$
\vec{v}(t) = (1+3t,\; -1+t) \text{ m/s}
$$

Position:

$$
\vec{r}(t) = \left(t+\frac{3}{2}t^2,\; -t+\frac{1}{2}t^2\right) \text{ m}
$$

Work done at $t=3$ s:

$$
W = 102 \text{ J}
$$

Work-energy theorem check:

$$
W = \Delta K = 102 \text{ J}
$$
