# Collision and Conservation Laws: Energy & Momentum



## Definitions and Key Concepts

**Conservation of Mechanical Energy:** In an isolated system where only conservative forces (like gravity) are acting, the total mechanical energy remains constant. The energy at the top of the track (purely potential) will completely convert into kinetic energy at the bottom of the frictionless track.

**Conservation of Momentum:** The total momentum of a closed system remains constant before and after a collision, provided no external forces (like friction) act upon it during the collision event.

**Perfectly Inelastic Collision:** A specific type of collision where two objects collide, stick together, and move as a single combined mass afterward. Kinetic energy is *not* conserved in this type of collision (some is lost to heat/sound/deformation), but momentum *is* conserved.

**Momentum ($p$):** The product of an object's mass and its velocity. It is a vector quantity, meaning it has both magnitude and direction.

---

## Key Formulas

**Gravitational Potential Energy ($PE$):**

$$
PE = mgh
$$

**Kinetic Energy ($KE$):**

$$
KE = \frac{1}{2}mv^2
$$

**Conservation of Energy (for the sliding block):**

$$
PE_{\text{initial}} + KE_{\text{initial}} = PE_{\text{final}} + KE_{\text{final}}
$$

**Conservation of Momentum (for the inelastic collision):**

$$
m_1v_1 + m_2v_2 = (m_1 + m_2)v_f
$$

---

## Problem Statement

A 0.5 kg block slides down a frictionless track from a height of 3.0 m. At the bottom, it collides and sticks to a 1.5 kg block, which is initially at rest. What is the speed of the combined mass just after the collision?

---

## Step-by-Step Solution

This problem must be solved in two distinct parts: First, we use the Conservation of Energy to find how fast the first block is moving when it reaches the bottom of the track. Second, we use the Conservation of Momentum to find the speed of the combined blocks after they stick together.

### Step 1: Identify the known variables

* **Mass of block 1 ($m_1$):** $0.5$ kg
* **Initial height of block 1 ($h$):** $3.0$ m
* **Mass of block 2 ($m_2$):** $1.5$ kg
* **Initial velocity of block 2 ($v_{2i}$):** $0$ m/s (at rest)
* **Acceleration due to gravity ($g$):** $\approx 9.81$ m/s²

### Step 2: Calculate the speed of Block 1 at the bottom of the track

At the top of the track, Block 1 is released from rest, so it only has potential energy ($PE = m_1gh$). At the bottom of the track (height = 0), all of this energy has been converted into kinetic energy ($KE = \frac{1}{2}m_1v_1^2$). 

Set the initial potential energy equal to the final kinetic energy:

$$
m_1gh = \frac{1}{2}m_1v_1^2
$$

Because $m_1$ is on both sides of the equation, it cancels out. This means the block's speed at the bottom depends only on gravity and the initial height:

$$
gh = \frac{1}{2}v_1^2
$$

Rearrange to solve for the velocity of block 1 ($v_1$) right before the collision:

$$
v_1 = \sqrt{2gh}
$$

Now, plug in the known values:

$$
v_1 = \sqrt{2 \cdot 9.81 \cdot 3.0}
$$

$$
v_1 = \sqrt{58.86} \approx 7.672 \text{ m/s}
$$

### Step 3: Set up the Conservation of Momentum for the collision

Right as Block 1 reaches the bottom, it collides with Block 2. They stick together, making this a perfectly inelastic collision. 

The initial momentum of the system is the sum of the momentums of the two individual blocks. The final momentum is the combined mass moving at a new final velocity ($v_f$).

$$
m_1v_1 + m_2v_{2i} = (m_1 + m_2)v_f
$$

Since Block 2 is initially at rest, its velocity ($v_{2i}$) is $0$, meaning its initial momentum is zero.

$$
m_1v_1 + 0 = (m_1 + m_2)v_f
$$

### Step 4: Solve for the final combined speed ($v_f$)

Isolate $v_f$ by dividing both sides by the total mass:

$$
v_f = \frac{m_1v_1}{m_1 + m_2}
$$

Substitute the known values and the velocity ($v_1$) we calculated in Step 2:

$$
v_f = \frac{0.5 \cdot 7.672}{0.5 + 1.5}
$$

$$
v_f = \frac{3.836}{2.0}
$$

$$
v_f \approx 1.918 \text{ m/s}
$$

---

## Final Answer

The speed of the combined mass just after the collision is approximately **$1.92$ m/s**.
