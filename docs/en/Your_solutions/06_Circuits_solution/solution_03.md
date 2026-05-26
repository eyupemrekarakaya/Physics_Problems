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
