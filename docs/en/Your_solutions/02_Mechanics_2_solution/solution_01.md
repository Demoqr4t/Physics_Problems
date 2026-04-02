# Simple Pendulum: Period and Length Calculations

## Definitions and Key Concepts

**Simple Pendulum:** An idealized system consisting of a point mass (the bob) suspended by a weightless, inextensible string of length $L$. When displaced from its equilibrium position, it oscillates back and forth under the influence of gravity.

**Period ($T$):** The time it takes for the pendulum to complete one full cycle of its swing (back and forth).

**Gravitational Acceleration ($g$):** The acceleration of an object due to the pull of gravity. On Earth, standard gravity is approximately **9.81 m/s²**.

### The Formula

For small angles of oscillation, the period $T$ of a simple pendulum is calculated using the following formula:

$$
T = 2\pi \sqrt{\frac{L}{g}}
$$

Where:
* $T$ is the period in seconds (s)
* $L$ is the length of the pendulum in meters (m)
* $g$ is the acceleration due to gravity in meters per second squared (m/s²)
* $\pi$ is the mathematical constant (approximately **3.14159**)

---

## Problem 1: Period of the Pendulum on the Moon

**Question:** A simple pendulum has a period of 4 seconds on Earth. What would its period be on the Moon, where the gravitational acceleration is about 1/6th of Earth's?

**Step 1: Express the period on Earth.** Let $g_E$ be Earth's gravity. The period on Earth ($T_E$) is given as **4 seconds**.

$$
T_E = 2\pi \sqrt{\frac{L}{g_E}} = 4
$$

**Step 2: Express the period on the Moon.** Let $g_M$ be the Moon's gravity. We are told that $g_M = \frac{1}{6} g_E$. We need to find the period on the Moon ($T_M$).

$$
T_M = 2\pi \sqrt{\frac{L}{g_M}}
$$

**Step 3: Substitute the Moon's gravity into the equation.**

$$
T_M = 2\pi \sqrt{\frac{L}{\frac{1}{6} g_E}}
$$

**Step 4: Simplify the expression.** Dividing by a fraction is equivalent to multiplying by its reciprocal. We can move the **6** up into the numerator.

$$
T_M = 2\pi \sqrt{6 \cdot \frac{L}{g_E}}
$$

We can then factor the $\sqrt{6}$ out from the rest of the square root:

$$
T_M = \sqrt{6} \cdot \left( 2\pi \sqrt{\frac{L}{g_E}} \right)
$$

**Step 5: Substitute the known Earth period.** Notice that the term inside the parentheses is exactly our formula for $T_E$, which we know is **4**.

$$
T_M = \sqrt{6} \cdot 4
$$

**Step 6: Calculate the final value.**

$$
T_M \approx 2.449 \cdot 4 \approx 9.80 \text{ seconds}
$$

**Answer:** The period of the pendulum on the Moon would be approximately **9.80 seconds**. Because gravity is weaker, the restoring force is smaller, causing the pendulum to swing much slower.

---

## Problem 2: Length of a 1-Second Pendulum on Earth

**Question:** What is the required length of a simple pendulum to have a period of exactly 1 second on Earth?

**Step 1: Identify the known variables.**
* $T = 1$ s
* $g \approx 9.81$ m/s² (Standard acceleration due to gravity on Earth)

**Step 2: Set up the equation using the period formula.**

$$
1 = 2\pi \sqrt{\frac{L}{9.81}}
$$

**Step 3: Isolate the square root.** Divide both sides by $2\pi$:

$$
\frac{1}{2\pi} = \sqrt{\frac{L}{9.81}}
$$

**Step 4: Square both sides.** This removes the square root so we can solve for $L$:

$$
\left(\frac{1}{2\pi}\right)^2 = \frac{L}{9.81}
$$

$$
\frac{1}{4\pi^2} = \frac{L}{9.81}
$$

**Step 5: Solve for $L$.** Multiply both sides by **9.81**:

$$
L = \frac{9.81}{4\pi^2}
$$

**Step 6: Calculate the final value.** Using the approximation $\pi^2 \approx 9.8696$:

$$
L \approx \frac{9.81}{4 \cdot 9.8696} \approx \frac{9.81}{39.478} \approx 0.248 \text{ meters}
$$

**Answer:** To have a period of exactly 1 second on Earth, the pendulum must be approximately **0.248 meters** (or **24.8 cm**) long.
