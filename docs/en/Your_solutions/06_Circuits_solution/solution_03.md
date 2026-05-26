# Mixed Circuit Resistance Calculation

This project calculates the equivalent resistance of a mixed resistor circuit using a Bash script.

---

# Circuit Information

All resistors in the circuit have a resistance of 5 ohms.

The goal is to calculate the equivalent resistance between the two terminals.

---

# Step-by-Step Solution

## Step 1: Middle Branch

The middle branch contains two resistors connected in series.

Formula:

R = 5Ω + 5Ω

Result:

R = 10Ω

---

## Step 2: Right Branch

The right branch also contains two resistors connected in series.

Formula:

R = 5Ω + 5Ω

Result:

R = 10Ω

---

## Step 3: Parallel Combination

The two 10Ω branches are connected in parallel.

Formula:

R = (10 × 10) / (10 + 10)

Result:

R = 5Ω

---

## Step 4: Final Series Combination

Now the remaining resistors are connected in series.

Formula:

Req = 5Ω + 5Ω + 5Ω

Result:

Req = 15Ω

---

# Final Answer

Equivalent Resistance = 15Ω

---

# Bash Script

```bash
#!/bin/bash

echo "====================================="
echo " Mixed Circuit Resistance Calculator "
echo "====================================="
echo ""

# All resistors are 5 ohms
R=5

echo "All resistors have a value of ${R}Ω"
echo ""

# STEP 1
echo "STEP 1: Calculate the middle branch"
middle=$((R + R))

echo "Middle branch resistors are connected in series:"
echo "5Ω + 5Ω = ${middle}Ω"
echo ""

# STEP 2
echo "STEP 2: Calculate the right branch"
right=$((R + R))

echo "Right branch resistors are connected in series:"
echo "5Ω + 5Ω = ${right}Ω"
echo ""

# STEP 3
echo "STEP 3: Calculate the parallel resistance"

parallel=$(((middle * right) / (middle + right)))

echo "The middle and right branches are in parallel:"
echo "R = (10 × 10) / (10 + 10)"
echo "R = ${parallel}Ω"
echo ""

# STEP 4
echo "STEP 4: Final series calculation"

final=$((R + parallel + R))

echo "Now the remaining resistors are in series:"
echo "Req = 5Ω + 5Ω + 5Ω"
echo "Req = ${final}Ω"
echo ""

echo "====================================="
echo " Final Equivalent Resistance = ${final}Ω "
echo "====================================="
```

---

# How to Run

```bash
chmod +x script.sh
./script.sh
```
