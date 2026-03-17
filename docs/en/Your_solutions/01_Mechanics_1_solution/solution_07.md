## 7. Elimination of Time and Interpretation of Acceleration

The path is given in parametric form by

$$
x(t) = 2t^2,
\qquad
y(t) = 3t^3
$$

---

### Step 1: Eliminate the parameter $$t$$

From

$$
x = 2t^2
$$

we get

$$
t^2 = \frac{x}{2}
$$

So,

$$
t = \pm \sqrt{\frac{x}{2}}
$$

Now use

$$
y = 3t^3 = 3t\cdot t^2
$$

Substitute $$t^2 = \frac{x}{2}$$:

$$
y = 3t\left(\frac{x}{2}\right)
$$

Since $$t = \pm \sqrt{\frac{x}{2}}$$, we obtain

$$
y = 3\left(\pm \sqrt{\frac{x}{2}}\right)\left(\frac{x}{2}\right)
$$

This gives the Cartesian relation more cleanly by squaring:

$$
y^2 = (3t^3)^2 = 9t^6
$$

and since

$$
t^2 = \frac{x}{2},
\qquad
t^6 = \left(\frac{x}{2}\right)^3
$$

we get

$$
y^2 = 9\left(\frac{x}{2}\right)^3
$$

$$
y^2 = \frac{9x^3}{8}
$$

So the trajectory is

$$
y^2 = \frac{9x^3}{8}
$$

---

### Step 2: Draw / describe the trajectory

The curve

$$
y^2 = \frac{9x^3}{8}
$$

is a **semicubical parabola**.

Since

$$
x = 2t^2 \ge 0
$$

the motion exists only for

$$
x \ge 0
$$

Also:

- for $$t>0$$, we have $$y>0$$
- for $$t<0$$, we have $$y<0$$
- at $$t=0$$, the particle is at the origin

So the trajectory has two symmetric branches about the $$x$$-axis, starting from the origin.

---

### Step 3: Calculate velocity vector $$\vec{v}(t)$$

Velocity is the derivative of position:

$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}
= 2t^2\hat{i} + 3t^3\hat{j}
$$

Therefore,

$$
\vec{v}(t) = \frac{d\vec{r}}{dt}
= \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j}
$$

Differentiate:

$$
\frac{dx}{dt} = 4t
$$

$$
\frac{dy}{dt} = 9t^2
$$

Hence,

$$
\vec{v}(t) = 4t\hat{i} + 9t^2\hat{j}
$$

---

### Step 4: Calculate speed $$|\vec{v}(t)|$$

The speed is the magnitude of velocity:

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2}
$$

$$
|\vec{v}(t)| = \sqrt{16t^2 + 81t^4}
$$

$$
|\vec{v}(t)| = \sqrt{t^2(16 + 81t^2)}
$$

$$
|\vec{v}(t)| = |t|\sqrt{16 + 81t^2}
$$

---

### Step 5: Calculate acceleration vector $$\vec{a}(t)$$

Acceleration is the derivative of velocity:

$$
\vec{a}(t) = \frac{d\vec{v}}{dt}
$$

Differentiate each component:

$$
\frac{d}{dt}(4t) = 4
$$

$$
\frac{d}{dt}(9t^2) = 18t
$$

So,

$$
\vec{a}(t) = 4\hat{i} + 18t\hat{j}
$$

---

### Step 6: Calculate acceleration magnitude $$|\vec{a}(t)|$$

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2}
$$

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

---

### Step 7: Is the acceleration constant?

The acceleration vector is

$$
\vec{a}(t) = 4\hat{i} + 18t\hat{j}
$$

Since the $$j$$-component depends on $$t$$, the acceleration vector changes with time.

Therefore,

$$
\text{the acceleration is not constant}
$$

Also, its magnitude

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

also depends on $$t$$, so the magnitude is not constant either.

---

## Final Result

$$
y^2 = \frac{9x^3}{8}
$$

$$
\vec{v}(t) = 4t\hat{i} + 9t^2\hat{j}
$$

$$
|\vec{v}(t)| = |t|\sqrt{16 + 81t^2}
$$

$$
\vec{a}(t) = 4\hat{i} + 18t\hat{j}
$$

$$
|\vec{a}(t)| = \sqrt{16 + 324t^2}
$$

$$
\text{Acceleration is not constant.}
$$
