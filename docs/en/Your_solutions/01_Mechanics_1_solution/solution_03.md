## 3. Path Intersection

Alice's position is given by

$$
A(t) = (2+t,\; 8-3t)
$$

and Bob's position is given by

$$
B(t) = (2t-1,\; 2t+2)
$$

We want to determine whether their paths intersect, and if so, whether they collide.

### Step 1: Check for intersection

Their paths intersect when their coordinates are equal:

$$
(2+t,\; 8-3t) = (2t-1,\; 2t+2)
$$

So we equate the components.

For the $$x$$-coordinates:

$$
2+t = 2t-1
$$

$$
t = 3
$$

For the $$y$$-coordinates:

$$
8-3t = 2t+2
$$

$$
6 = 5t
$$

$$
t = \frac{6}{5}
$$

Since the two equations give different values of $$t$$, there is no single time at which both coordinates are equal.

Therefore, Alice and Bob do **not** collide.

---

### Step 2: Check whether the geometric paths intersect

Alice's path:

$$
x = 2+t \quad \Rightarrow \quad t = x-2
$$

Substitute into $$y = 8-3t$$:

$$
y = 8 - 3(x-2)
$$

$$
y = 14 - 3x
$$

So Alice moves along the line

$$
y = 14 - 3x
$$

Bob's path:

$$
x = 2t-1 \quad \Rightarrow \quad t = \frac{x+1}{2}
$$

Substitute into $$y = 2t+2$$:

$$
y = 2\left(\frac{x+1}{2}\right)+2
$$

$$
y = x+3
$$

So Bob moves along the line

$$
y = x+3
$$

To find the intersection of the two paths, solve:

$$
14 - 3x = x + 3
$$

$$
11 = 4x
$$

$$
x = \frac{11}{4}
$$

Then

$$
y = x+3 = \frac{11}{4} + 3 = \frac{23}{4}
$$

Thus, the two geometric paths intersect at

$$
\left(\frac{11}{4},\; \frac{23}{4}\right)
$$

But they reach that point at different times, so they do not collide.

For Alice:

$$
2+t = \frac{11}{4}
$$

$$
t = \frac{3}{4}
$$

For Bob:

$$
2t-1 = \frac{11}{4}
$$

$$
2t = \frac{15}{4}
$$

$$
t = \frac{15}{8}
$$

So the paths intersect, but not at the same time.

---

## Final Result

$$
\text{The paths intersect geometrically at } \left(\frac{11}{4},\; \frac{23}{4}\right)
$$

$$
t_{\text{Alice}} = \frac{3}{4}, \qquad t_{\text{Bob}} = \frac{15}{8}
$$

$$
\text{Therefore, they do not collide.}
$$
