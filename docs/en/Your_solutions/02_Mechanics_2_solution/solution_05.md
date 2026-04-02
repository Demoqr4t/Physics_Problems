# Inelastic Collision: Runner and Cart

## Definitions and Key Concepts

**Momentum ($p$):** A measure of an object's mass in motion, defined as the product of its mass and velocity. It is a vector quantity, meaning it has a specific direction.

**Conservation of Momentum:** In a closed, isolated system (where no external forces like friction act on it), the total momentum before an event is exactly equal to the total momentum after the event. 

**Perfectly Inelastic Collision:** A type of collision in which two objects collide and stick together, moving as a single combined mass afterward. While total momentum is perfectly conserved, kinetic energy is *not* conserved. 

**Kinetic Energy ($KE$):** The energy that an object possesses due to its motion.

---

## Key Formulas

**Momentum:**

$$
p = mv
$$

**Conservation of Momentum (for a perfectly inelastic collision):**

$$
m_1v_{1i} + m_2v_{2i} = (m_1 + m_2)v_f
$$

**Kinetic Energy:**

$$
KE = \frac{1}{2}mv^2
$$

---

## Problem Statement

A 70 kg runner moving at $3 \text{ m/s}$ jumps onto a 140 kg stationary cart. 
1. What is the final speed of the cart with the runner? 
2. Is kinetic energy conserved in this collision? Explain.

---

## Step-by-Step Solution

### Step 1: Identify the known variables

* **Mass of the runner ($m_1$):** $70 \text{ kg}$
* **Initial velocity of the runner ($v_{1i}$):** $3 \text{ m/s}$
* **Mass of the cart ($m_2$):** $140 \text{ kg}$
* **Initial velocity of the cart ($v_{2i}$):** $0 \text{ m/s}$ (because it is stationary)

### Step 2: Calculate the final speed using Conservation of Momentum

Because there are no external horizontal forces, the total momentum before the runner jumps must equal the total momentum after the runner lands. Since they move together afterward, we set up the inelastic collision equation:

$$
m_1v_{1i} + m_2v_{2i} = (m_1 + m_2)v_f
$$

Substitute the known values:

$$
(70 \cdot 3) + (140 \cdot 0) = (70 + 140)v_f
$$

### Step 3: Solve for final velocity ($v_f$)

Simplify the terms on both sides of the equation:

$$
210 + 0 = 210v_f
$$

$$
210 = 210v_f
$$

Divide both sides by 210 to isolate $v_f$:

$$
v_f = \frac{210}{210} = 1 \text{ m/s}
$$

The cart and the runner are moving at **$1 \text{ m/s}$**.

### Step 4: Analyze Kinetic Energy conservation

To determine if kinetic energy is conserved, we must calculate the total kinetic energy of the system *before* the collision and compare it to the total kinetic energy *after* the collision.

**Initial Kinetic Energy ($KE_i$):**
Before the collision, only the runner is moving. The cart is stationary, so its kinetic energy is zero.

$$
KE_i = \frac{1}{2}m_1v_{1i}^2 + \frac{1}{2}m_2v_{2i}^2
$$

$$
KE_i = \frac{1}{2}(70)(3)^2 + 0
$$

$$
KE_i = 35 \cdot 9 = 315 \text{ Joules}
$$

**Final Kinetic Energy ($KE_f$):**
After the collision, the combined mass ($70 \text{ kg} + 140 \text{ kg} = 210 \text{ kg}$) is moving at the new final velocity of $1 \text{ m/s}$.

$$
KE_f = \frac{1}{2}(m_1 + m_2)v_f^2
$$

$$
KE_f = \frac{1}{2}(210)(1)^2
$$

$$
KE_f = 105 \cdot 1 = 105 \text{ Joules}
$$

### Step 5: Compare the energies

* Initial Kinetic Energy: $315 \text{ J}$
* Final Kinetic Energy: $105 \text{ J}$

Because $315 \text{ J} \neq 105 \text{ J}$, kinetic energy is clearly lost. 

---

## Final Answers

* **Final Speed:** The final speed of the cart with the runner is **$1 \text{ m/s}$**.
* **Is Kinetic Energy Conserved?:** **No.** In a perfectly inelastic collision, kinetic energy is never conserved. The system started with $315 \text{ J}$ of kinetic energy and ended with only $105 \text{ J}$. The missing $210 \text{ J}$ of energy was transformed into other non-mechanical forms of energy, such as heat, sound, or the physical deformation of the cart's suspension when the runner landed on it.
