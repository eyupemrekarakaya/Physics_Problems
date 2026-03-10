# Solution 10 — Infinite Series

## Problem

Determine the final position of an ant that starts at the origin and moves according to the pattern:

1 m east, 1/2 m north, 1/3 m west, 1/4 m south, 1/5 m east, and so on.

---

## Solution

We separate the motion into horizontal and vertical components.

### Horizontal motion

The horizontal displacements are:

1 - 1/3 + 1/5 - 1/7 + ...

This is the alternating series:

π / 4

So the final x-coordinate is:

x = π / 4

---

### Vertical motion

The vertical displacements are:

1/2 - 1/4 + 1/6 - 1/8 + ...

Factor out 1/2:

= (1/2)(1 - 1/2 + 1/3 - 1/4 + ...)

The alternating harmonic series is:

1 - 1/2 + 1/3 - 1/4 + ... = ln(2)

Therefore:

y = (1/2) ln(2)

---

## Answer

The final position of the ant is:

(x, y) = (π / 4, (1/2)ln(2))

Approximate values:

x ≈ 0.785  
y ≈ 0.347
