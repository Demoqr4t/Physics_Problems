# Mass-Spring System: Spring Constant and Energy Calculations

## Definitions and Key Concepts

**Simple Harmonic Motion (SHM):** A type of periodic motion where the restoring force is directly proportional to the displacement and acts in the direction opposite to that of displacement.

**Amplitude ($A$):** The maximum extent of a vibration or oscillation, measured from the position of equilibrium. In this context, it's the maximum stretch or compression of the spring.

**Angular Frequency ($\omega$):** A scalar measure of rotation rate, indicating how many radians the system oscillates through per second. It dictates how fast the mass bounces back and forth.

**Spring Constant ($k$):** A parameter that quantifies the stiffness of a given spring (from Hooke's Law). Higher values mean a stiffer spring that requires more force to stretch.

**Total Mechanical Energy ($E$):** In an ideal, frictionless mass-spring system, the total energy is conserved. It is the continuous sum of kinetic and potential energy, which is exactly equal to the maximum potential energy stored in the spring when it is at its peak displacement.

---

## Key Formulas

**Position Equation for SHM:**

$$
x(t) = A \cos(\omega t + \phi)
$$

**Angular Frequency:**

$$
\omega = \sqrt{\frac{k}{m}}
$$

**Spring Constant (Derived from Angular Frequency):**

$$
k = m \omega^2
$$

**Total Mechanical Energy:**

$$
E = \frac{1}{2} k A^2
$$

---

## Problem Statement

A 10 kg mass is attached to a spring and oscillates according to the equation $x(t) = 0.2 \cos(10\pi t)$ (in meters). 
1. What is the spring constant $k$? 
2. What is the total mechanical energy of the system?

---

## Step-by-Step Solution

### Step 1: Identify the given parameters

By comparing the given equation of motion $x(t) = 0.2 \cos(10\pi t)$ to the general standard form $x(t) = A \cos(\omega t + \phi)$, we can extract the essential variables:

* **Amplitude ($A$):** $0.2$ m
* **Angular frequency ($\omega$):** $10\pi$ rad/s
* **Mass ($m$):** $10$ kg

### Step 2: Calculate the Spring Constant ($k$)

We know the mathematical relationship between angular frequency, mass, and the spring constant:

$$
\omega = \sqrt{\frac{k}{m}}
$$

To isolate the spring constant $k$, we square both sides of the equation and multiply by the mass $m$:

$$
k = m \omega^2
$$

Now, substitute the extracted values into the formula:

$$
k = 10 \cdot (10\pi)^2
$$

Square the angular frequency term first:

$$
k = 10 \cdot 100\pi^2
$$

Multiply by the mass to find the exact value of $k$:

$$
k = 1000\pi^2 \text{ N/m}
$$

*(Note: Using the approximation $\pi^2 \approx 9.8696$, the spring constant is approximately **$9869.6$ N/m**).*

### Step 3: Calculate the Total Mechanical Energy ($E$)

The total mechanical energy of a simple harmonic oscillator is constant and is equal to the maximum potential energy. We use the formula:

$$
E = \frac{1}{2} k A^2
$$

Substitute the calculated spring constant $k$ and the known amplitude $A$ into the energy formula:

$$
E = \frac{1}{2} (1000\pi^2) \cdot (0.2)^2
$$

Calculate the square of the amplitude:

$$
E = 500\pi^2 \cdot 0.04
$$

Multiply the terms together to find the exact energy:

$$
E = 20\pi^2 \text{ J}
$$

*(Note: Using the approximation $\pi^2 \approx 9.8696$, the total mechanical energy is approximately **$197.39$ Joules**).*

---

## Final Answers
* The spring constant $k$ is **$1000\pi^2$ N/m**.
* The total mechanical energy $E$ is **$20\pi^2$ J**.
