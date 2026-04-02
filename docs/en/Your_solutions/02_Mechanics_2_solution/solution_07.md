# Dynamics with Friction: Stacked Blocks



## Definitions and Key Concepts

**Newton's Second Law:** The acceleration of an object as produced by a net force is directly proportional to the magnitude of the net force, in the same direction as the net force, and inversely proportional to the mass of the object. 

**Normal Force ($N$):** The support force exerted upon an object that is in contact with another stable object. For an object resting on a horizontal surface, the normal force is equal in magnitude and opposite in direction to the gravitational force (weight) of the object or objects above it.

**Kinetic Friction ($f_k$):** A force that acts between moving surfaces. An object that is being moved over a surface will experience a force in the opposite direction as its movement.

**Coefficient of Kinetic Friction ($\mu_k$):** A dimensionless number representing the ratio of the force of friction between two bodies to the normal force pressing them together. 

---

## Key Formulas

**Weight:**

$$
W = mg
$$

**Kinetic Friction:**

$$
f_k = \mu_k N
$$

**Newton's Second Law:**

$$
F_{\text{net}} = ma
$$

---

## Problem Statement

A 5 kg block is placed on a 10 kg block. A horizontal force of 45 N is applied to the 10 kg block, and the 5 kg block is tied to the wall. The coefficient of kinetic friction between all moving surfaces is 0.2. Find the acceleration of the 10 kg block.

---

## Step-by-Step Solution

### Step 1: Identify the known variables

* **Mass of top block ($m_1$):** 5 kg
* **Mass of bottom block ($m_2$):** 10 kg
* **Applied force ($F$):** 45 N
* **Coefficient of kinetic friction ($\mu_k$):** 0.2
* **Acceleration due to gravity ($g$):** $\approx 9.81$ m/s²

### Step 2: Analyze the physical system

The top block (5 kg) is tied to the wall, meaning it cannot move horizontally. Its acceleration is zero.
The bottom block (10 kg) is pulled by a 45 N force. As it slides, it experiences **two** different frictional forces opposing its motion:
1. Friction between the bottom block and the ground ($f_{k2}$).
2. Friction between the bottom block and the top block ($f_{k1}$), because the top block is stationary while the bottom block drags underneath it.

### Step 3: Calculate the Normal Forces

**Normal Force 1 ($N_1$):**
This is the force pressing the top block into the bottom block. It is simply the weight of the top block.

$$
N_1 = m_1 g
$$

$$
N_1 = 5 \cdot 9.81 = 49.05 \text{ N}
$$

**Normal Force 2 ($N_2$):**
This is the force pressing the bottom block into the ground. It must support the weight of *both* blocks.

$$
N_2 = (m_1 + m_2) g
$$

$$
N_2 = (5 + 10) \cdot 9.81 = 15 \cdot 9.81 = 147.15 \text{ N}
$$

### Step 4: Calculate the Frictional Forces

Using the formula for kinetic friction, calculate the friction at both surfaces. Both of these forces act in the opposite direction of the applied 45 N force.

**Friction from the top block ($f_{k1}$):**

$$
f_{k1} = \mu_k N_1
$$

$$
f_{k1} = 0.2 \cdot 49.05 = 9.81 \text{ N}
$$

**Friction from the ground ($f_{k2}$):**

$$
f_{k2} = \mu_k N_2
$$

$$
f_{k2} = 0.2 \cdot 147.15 = 29.43 \text{ N}
$$

### Step 5: Set up Newton's Second Law for the bottom block

The net force on the bottom block ($m_2$) is the applied forward force minus both backward frictional forces. We set this equal to the mass of the bottom block times its acceleration ($a$).

$$
F_{\text{net}} = F - f_{k1} - f_{k2} = m_2 a
$$

Substitute all the known and calculated values into the equation:

$$
45 - 9.81 - 29.43 = 10 \cdot a
$$

### Step 6: Solve for acceleration ($a$)

Combine the terms on the left side:

$$
45 - 39.24 = 10 \cdot a
$$

$$
5.76 = 10 \cdot a
$$

Divide by 10 to isolate acceleration:

$$
a = \frac{5.76}{10} = 0.576 \text{ m/s}^2
$$

---

## Final Answer

The acceleration of the 10 kg block is **0.576 m/s²**.
