# Pendulum Velocity via Conservation of Energy

## Definitions and Key Concepts



**Conservation of Mechanical Energy:** A fundamental principle stating that in an isolated system subject only to conservative forces (like gravity), the total mechanical energy remains constant. Energy simply transforms between potential and kinetic forms.

**Gravitational Potential Energy ($PE$):** The energy an object possesses due to its position relative to a reference point (usually the lowest point in the system). It is highest when the pendulum is at its maximum angle.

**Kinetic Energy ($KE$):** The energy an object possesses due to its motion. It is zero at the release point and reaches its maximum when the pendulum swings through its lowest point.

**Reference Level ($h = 0$):** We define the lowest point of the pendulum's swing as the zero potential energy level to simplify our calculations.

---

## Key Formulas

**Kinetic Energy:**

$$
KE = \frac{1}{2}mv^2
$$

**Gravitational Potential Energy:**

$$
PE = mgh
$$

**Height of the Pendulum Bob ($h$):**
When a pendulum of length $L$ is displaced by an angle $\theta$, the vertical height it rises from its lowest point is found using trigonometry:

$$
h = L - L\cos(\theta) = L(1 - \cos(\theta))
$$

**Conservation of Energy Equation:**

$$
PE_{\text{initial}} + KE_{\text{initial}} = PE_{\text{final}} + KE_{\text{final}}
$$

---

## Problem Statement

A pendulum with a length of 1.0 meter is released from an initial angle of $15^\circ$. What is the speed of the pendulum bob at the bottom of its swing?

---

## Step-by-Step Solution

### Step 1: Identify the known variables

* **Length of pendulum ($L$):** $1.0$ m
* **Initial angle ($\theta$):** $15^\circ$
* **Initial velocity ($v_i$):** $0$ m/s (released from rest, meaning initial kinetic energy is 0)
* **Acceleration due to gravity ($g$):** $\approx 9.81$ m/s²

### Step 2: Calculate the change in vertical height ($h$)

Before we can use energy conservation, we need to determine how high the pendulum bob is when released, relative to the bottom of the swing.

$$
h = L(1 - \cos(\theta))
$$

Substitute the known values:

$$
h = 1.0 \cdot (1 - \cos(15^\circ))
$$

Using the value $\cos(15^\circ) \approx 0.9659$:

$$
h = 1.0 \cdot (1 - 0.9659) = 0.0341 \text{ m}
$$

### Step 3: Set up the Conservation of Energy equation

At the release point (initial state), the pendulum is briefly at rest, so it only has potential energy. At the lowest point (final state), the height is 0, so all that potential energy has converted completely into kinetic energy.

$$
mgh = \frac{1}{2}mv^2
$$

### Step 4: Simplify the equation

Notice that mass ($m$) appears on both sides of the equation. This means the mass of the bob doesn't matter and cancels out:

$$
gh = \frac{1}{2}v^2
$$

### Step 5: Solve for final velocity ($v$)

Multiply both sides by 2 to isolate $v^2$:

$$
v^2 = 2gh
$$

Take the square root of both sides to get the formula for velocity:

$$
v = \sqrt{2gh}
$$

### Step 6: Plug in the numbers and calculate

Now, substitute the values for gravity ($g$) and the height ($h$) we calculated in Step 2:

$$
v = \sqrt{2 \cdot 9.81 \cdot 0.0341}
$$

$$
v = \sqrt{0.669}
$$

$$
v \approx 0.818 \text{ m/s}
$$

---

## Final Answer

The speed of the pendulum bob at the bottom of its swing is approximately **$0.82$ m/s**.
