# Work and Energy with a Constant Force

## Definitions and Key Concepts

**Constant Force:** A force whose magnitude and direction do not change over time. When a constant force acts on an object, it produces a constant acceleration.

**Kinematics (Position, Velocity, Acceleration):** The branch of mechanics that describes the motion of points, bodies, and systems of bodies without considering the forces that cause them to move. Acceleration is the derivative of velocity, and velocity is the derivative of position.

**Work ($W$):** The measure of energy transfer that occurs when an object is moved over a distance by an external force at least part of which is applied in the direction of the displacement. For a constant force, it is the dot product of the force vector and the displacement vector.

**Kinetic Energy ($E_k$):** The energy that an object possesses due to its motion.

**Work-Energy Theorem:** A fundamental theorem in physics stating that the net work done on an object by all forces equals the change in its kinetic energy.

---

## Key Formulas

**Newton's Second Law:**

$$
\vec{F} = m\vec{a}
$$

**Kinematic Integrals:**

$$
\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}(0)
$$

$$
\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}(0)
$$

**Work Done by a Constant Force:**

$$
W = \vec{F} \cdot \Delta\vec{r} = F_x \Delta x + F_y \Delta y
$$

**Kinetic Energy:**

$$
E_k = \frac{1}{2} m |\vec{v}|^2 = \frac{1}{2} m (v_x^2 + v_y^2)
$$

**Work-Energy Theorem:**

$$
W = \Delta E_k = E_k(\text{final}) - E_k(\text{initial})
$$

---

## Problem Statement

A constant force acts on a body of mass **$m = 2$ kg**:

$$
\vec{F} = [6, 2]\ \text{N}
$$

The body starts with an initial velocity $\vec{v}(0) = (1, -1)$ m/s from the point $\vec{r}(0) = (0,0)$ m.
1. Determine $\vec{a}(t)$.
2. Determine $\vec{v}(t)$.
3. Determine $\vec{r}(t)$.
4. Draw the trajectory of the motion.
5. Calculate the work done by the force at time $t=3$ s.
6. Check the consistency with the work-energy theorem.

---

## Step-by-Step Solution

### Step 1: Determine Acceleration $\vec{a}(t)$

According to Newton's Second Law, acceleration is the net force divided by the mass.

$$
\vec{a}(t) = \frac{\vec{F}}{m} = \left[ \frac{6}{2}, \frac{2}{2} \right]
$$

$$
\vec{a}(t) = [3, 1]\ \text{m/s}^2
$$

Because the force is constant, the acceleration is also constant over time.

### Step 2: Determine Velocity $\vec{v}(t)$

Velocity is the integral of acceleration with respect to time, plus the initial velocity vector $\vec{v}(0)$.

$$
\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}(0)
$$

$$
\vec{v}(t) = \int [3, 1] \, dt + [1, -1]
$$

$$
\vec{v}(t) = [3t, t] + [1, -1]
$$

Combine the components:

$$
\vec{v}(t) = [3t + 1, t - 1]\ \text{m/s}
$$

### Step 3: Determine Position $\vec{r}(t)$

Position is the integral of velocity with respect to time, plus the initial position vector $\vec{r}(0)$. Since the object starts at the origin, $\vec{r}(0) = [0, 0]$.

$$
\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}(0)
$$

$$
\vec{r}(t) = \int [3t + 1, t - 1] \, dt + [0, 0]
$$

Integrate each component:

$$
\vec{r}(t) = \left[ \frac{3}{2}t^2 + t, \frac{1}{2}t^2 - t \right]\ \text{m}
$$

$$
\vec{r}(t) = [1.5t^2 + t, 0.5t^2 - t]\ \text{m}
$$

### Step 4: Draw the trajectory of the motion

To draw the trajectory (the path the particle takes in the $x$-$y$ plane), we can use a Python script. Below is the code utilizing `matplotlib` to plot the parametric equations $x(t)$ and $y(t)$ from $t = 0$ to $t = 3$.

```python
import numpy as np
import matplotlib.pyplot as plt

# Time vector from 0 to 3 seconds
t = np.linspace(0, 3, 100)

# Parametric equations of motion
x = 1.5 * t**2 + t
y = 0.5 * t**2 - t

# Create the plot
plt.figure(figsize=(8, 6))
plt.plot(x, y, label='Trajectory from t=0 to t=3s', color='blue', linewidth=2)
plt.scatter(x[0], y[0], color='green', zorder=5, label='Start (t=0)')
plt.scatter(x[-1], y[-1], color='red', zorder=5, label='End (t=3)')

# Formatting the plot
plt.title('Particle Trajectory under Constant Force')
plt.xlabel('x Position (m)')
plt.ylabel('y Position (m)')
plt.axhline(0, color='black', linewidth=0.5)
plt.axvline(0, color='black', linewidth=0.5)
plt.grid(True, linestyle='--', alpha=0.7)
plt.legend()

# Display
plt.show()
