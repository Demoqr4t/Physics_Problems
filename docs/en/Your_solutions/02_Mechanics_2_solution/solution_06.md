# Energy Dissipation in a Bouncing Ball



## Definitions and Key Concepts

**Mechanical Energy ($E$):** The sum of potential and kinetic energy in a system. When the ball is at its maximum height before dropping or after a bounce, its velocity is zero, meaning all of its mechanical energy is in the form of potential energy.

**Gravitational Potential Energy ($PE$):** The energy an object possesses due to its height above a reference point (the ground). It is directly proportional to the object's mass, gravity, and height.

**Energy Dissipation:** The loss of mechanical energy in a system, usually transformed into other forms like thermal energy (heat) or acoustic energy (sound). In this problem, energy is dissipated during the inelastic collision when the ball hits the floor.

**Energy Retention:** If an object loses a certain percentage of its energy, it retains the remaining percentage. For example, losing **30%** of its energy means it retains **70%** (or a fraction of $0.70$) of its previous energy.

---

## Key Formulas

**Gravitational Potential Energy:**

$$
PE = mgh
$$

**Energy After a Bounce ($E_{n}$):**
If $r$ is the fraction of energy retained, the energy after the $n$-th bounce is:

$$
E_n = r \cdot E_{n-1}
$$

Because mass ($m$) and gravity ($g$) remain constant, the peak height ($h$) is directly proportional to the total energy ($E$). Therefore, we can apply the retention fraction directly to the height:

$$
h_n = r \cdot h_{n-1}
$$

---

## Problem Statement

A tennis ball is dropped from a height of **2.0 m**. After each bounce, it loses **30%** of its mechanical energy. To what height does it rise after the second bounce?

---

## Step-by-Step Solution

### Step 1: Identify the known variables and the retention factor

* **Initial height ($h_0$):** **2.0 m**
* **Energy loss per bounce:** **30%**

To find out how much energy (and therefore height) the ball *keeps*, we subtract the loss from the whole:
* **Energy retained per bounce ($r$):** $100\% - 30\% = 70\%$
* Expressed as a decimal, the retention factor is **$0.70$**.

### Step 2: Understand the relationship between energy and height

At the peak of any bounce, all the ball's kinetic energy has converted back into potential energy ($PE = mgh$). Because the mass of the tennis ball ($m$) and the acceleration due to gravity ($g$) do not change, any percentage loss in total mechanical energy results in the exact same percentage loss in maximum height.

### Step 3: Calculate the height after the first bounce ($h_1$)

The ball retains **70%** of its initial energy, so it will reach **70%** of its initial height.

$$
h_1 = 0.70 \cdot h_0
$$

Substitute the initial height (**2.0 m**):

$$
h_1 = 0.70 \cdot 2.0
$$

$$
h_1 = 1.4 \text{ m}
$$

After the first bounce, the ball rises to **1.4 meters**.

### Step 4: Calculate the height after the second bounce ($h_2$)

The ball undergoes a second collision and again loses **30%** of the energy it had *just before* the bounce. This means it will rise to **70%** of the height of the *previous* bounce ($h_1$).

$$
h_2 = 0.70 \cdot h_1
$$

Substitute the height from the first bounce (**1.4 m**):

$$
h_2 = 0.70 \cdot 1.4
$$

$$
h_2 = 0.98 \text{ m}
$$

---

## Final Answer

After the second bounce, the tennis ball rises to a height of **0.98 meters**.
