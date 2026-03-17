## 10. Kinematics

The point moves according to

$$
\vec{r}(t) = \bigl(a\cos(\omega t),\; b\sin(\omega t),\; bt\bigr)
$$

where $$a,b,\omega > 0$$.

---

### (a) Equation of the trajectory

The parametric equations are

$$
x(t) = a\cos(\omega t)
$$

$$
y(t) = b\sin(\omega t)
$$

$$
z(t) = bt
$$

From the first two equations,

$$
\cos(\omega t) = \frac{x}{a}
$$

$$
\sin(\omega t) = \frac{y}{b}
$$

Using the identity

$$
\cos^2(\omega t) + \sin^2(\omega t) = 1
$$

we obtain

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

So, in the $$xy$$-plane, the projection of the motion is an ellipse.

Since

$$
z = bt
$$

we also have

$$
t = \frac{z}{b}
$$

Substitute into $$x(t)$$ and $$y(t)$$:

$$
x = a\cos\left(\frac{\omega z}{b}\right)
$$

$$
y = b\sin\left(\frac{\omega z}{b}\right)
$$

Hence, the full spatial trajectory is an **elliptic helix**.

---

### (b) Path length from $$t=0$$ to $$t=t_0$$

The arc length is

$$
s = \int_0^{t_0} \left|\vec{r}\,'(t)\right|\,dt
$$

First compute the velocity:

$$
\vec{r}\,'(t) = \bigl(-a\omega\sin(\omega t),\; b\omega\cos(\omega t),\; b\bigr)
$$

Its magnitude is

$$
\left|\vec{r}\,'(t)\right|
=
\sqrt{a^2\omega^2\sin^2(\omega t) + b^2\omega^2\cos^2(\omega t) + b^2}
$$

Therefore, the path length is

$$
s = \int_0^{t_0}
\sqrt{a^2\omega^2\sin^2(\omega t) + b^2\omega^2\cos^2(\omega t) + b^2}
\,dt
$$

This is the general arc-length formula.

---

### Special case: circular helix when $$a=b$$

If $$a=b$$, then

$$
\left|\vec{r}\,'(t)\right|
=
\sqrt{a^2\omega^2\sin^2(\omega t) + a^2\omega^2\cos^2(\omega t) + a^2}
$$

$$
=
\sqrt{a^2\omega^2\bigl(\sin^2(\omega t)+\cos^2(\omega t)\bigr)+a^2}
$$

$$
=
\sqrt{a^2\omega^2 + a^2}
=
a\sqrt{\omega^2+1}
$$

So in this case the speed is constant, and the arc length becomes

$$
s = \int_0^{t_0} a\sqrt{\omega^2+1}\,dt
$$

$$
s = a\sqrt{\omega^2+1}\,t_0
$$

---

### (c) Description of the trajectory and special cases

The trajectory is a three-dimensional helix:

- The $$x$$- and $$y$$-coordinates trace an ellipse:
  
  $$
  \frac{x^2}{a^2} + \frac{y^2}{b^2} = 1
  $$

- The $$z$$-coordinate increases linearly with time:
  
  $$
  z = bt
  $$

So the point winds upward while moving around an ellipse.

#### Special cases

1. **If $$a=b$$**  
   Then the ellipse becomes a circle:

   $$
   x^2 + y^2 = a^2
   $$

   and the trajectory is a **circular helix**.

2. **If $$\omega$$ increases**  
   The point rotates faster around the axis, so the helix becomes more tightly wound.

3. **If $$b$$ increases**  
   The vertical rise per unit time increases, so the helix stretches upward more rapidly.

4. **If $$b=0$$**  
   Then

   $$
   z=0
   $$

   and the motion stays in the plane, tracing an ellipse.

---

## Final Result

$$
x(t)=a\cos(\omega t),\qquad y(t)=b\sin(\omega t),\qquad z(t)=bt
$$

$$
\frac{x^2}{a^2}+\frac{y^2}{b^2}=1
$$

$$
x = a\cos\left(\frac{\omega z}{b}\right),\qquad
y = b\sin\left(\frac{\omega z}{b}\right)
$$

$$
\vec{r}\,'(t)=\bigl(-a\omega\sin(\omega t),\; b\omega\cos(\omega t),\; b\bigr)
$$

$$
\left|\vec{r}\,'(t)\right|
=
\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}
$$

$$
s=\int_0^{t_0}
\sqrt{a^2\omega^2\sin^2(\omega t)+b^2\omega^2\cos^2(\omega t)+b^2}\,dt
$$

If $$a=b$$, then

$$
s=a\sqrt{\omega^2+1}\,t_0
$$

So the trajectory is an **elliptic helix**, and in the special case $$a=b$$ it becomes a **circular helix**.
