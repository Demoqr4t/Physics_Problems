# Dynamics with a Time-Dependent Force

## Definitions and Key Concepts

**Position Vector ($\vec{r}$):** A mathematical representation of the location of a particle in 3D space, typically written in Cartesian coordinates as $(x(t), y(t), z(t))$.

**Velocity Vector ($\vec{v}$):** The rate at which the particle's position changes over time. It is the first integral of acceleration and the first derivative of position.

**Acceleration Vector ($\vec{a}$):** The rate at which the particle's velocity changes over time. According to Newton's Second Law, it is directly proportional to the net force acting on the object.

**Newton's Second Law of Motion:** The fundamental principle in classical mechanics stating that the force acting on an object is equal to its mass times its acceleration.

**Initial Conditions:** The known state of the system at time $t=0$, which allows us to find the specific constants of integration when moving from acceleration to velocity, and from velocity to position.

---

## Key Formulas

**Newton's Second Law:**

$$
\vec{F}(t) = m\vec{a}(t) \implies \vec{a}(t) = \frac{\vec{F}(t)}{m}
$$

**Velocity (Integration of Acceleration):**

$$
\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0
$$

**Position (Integration of Velocity):**

$$
\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0
$$

---

## Problem Statement

A particle of mass $m=3$ kg moves in a force field $\vec{F}$ dependent on time in the following way:

$$
\vec{F} = (15t, 3t-12, -6t^2) \text{ N}
$$

Assuming initial conditions $\vec{r}_0=(5,2,-3)$ m, $\vec{v}_0=(2,0,1)$ m/s, find the dependence of the particle's position and velocity on time.

---

## Step-by-Step Solution

### Step 1: Extract the given parameters
* **Mass ($m$):** $3$ kg
* **Force vector ($\vec{F}$):** $(15t, 3t-12, -6t^2)$ N
* **Initial velocity ($\vec{v}_0$):** $(2, 0, 1)$ m/s
* **Initial position ($\vec{r}_0$):** $(5, 2, -3)$ m

### Step 2: Determine the acceleration vector $\vec{a}(t)$
By Newton's Second Law, acceleration is force divided by mass. We divide each component of the force vector by the mass $m=3$.

$$
\vec{a}(t) = \left( \frac{15t}{3}, \frac{3t-12}{3}, \frac{-6t^2}{3} \right)
$$

$$
\vec{a}(t) = (5t, t-4, -2t^2) \text{ m/s}^2
$$

### Step 3: Determine the velocity vector $\vec{v}(t)$
Velocity is the integral of acceleration with respect to time. We integrate each component individually and add the corresponding component of the initial velocity $\vec{v}_0$ as our constant of integration.

**X-component ($v_x$):**

$$
v_x(t) = \int 5t \, dt + v_{0x} = \frac{5}{2}t^2 + 2 = 2.5t^2 + 2
$$

**Y-component ($v_y$):**

$$
v_y(t) = \int (t - 4) \, dt + v_{0y} = \frac{1}{2}t^2 - 4t + 0 = 0.5t^2 - 4t
$$

**Z-component ($v_z$):**

$$
v_z(t) = \int (-2t^2) \, dt + v_{0z} = -\frac{2}{3}t^3 + 1
$$

Putting it all together, the time dependence of the particle's velocity is:

$$
\vec{v}(t) = \left( 2.5t^2 + 2, \, 0.5t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right) \text{ m/s}
$$

### Step 4: Determine the position vector $\vec{r}(t)$
Position is the integral of velocity with respect to time. We integrate each component of our newly found velocity vector and add the corresponding component of the initial position $\vec{r}_0$.

**X-component ($x$):**

$$
x(t) = \int \left( 2.5t^2 + 2 \right) \, dt + r_{0x} = \left( \frac{2.5}{3}t^3 + 2t \right) + 5 = \frac{5}{6}t^3 + 2t + 5
$$

**Y-component ($y$):**

$$
y(t) = \int \left( 0.5t^2 - 4t \right) \, dt + r_{0y} = \left( \frac{0.5}{3}t^3 - \frac{4}{2}t^2 \right) + 2 = \frac{1}{6}t^3 - 2t^2 + 2
$$

**Z-component ($z$):**

$$
z(t) = \int \left( -\frac{2}{3}t^3 + 1 \right) \, dt + r_{0z} = \left( -\frac{2}{12}t^4 + t \right) - 3 = -\frac{1}{6}t^4 + t - 3
$$

Putting it all together, the time dependence of the particle's position is:

$$
\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \, \frac{1}{6}t^3 - 2t^2 + 2, \, -\frac{1}{6}t^4 + t - 3 \right) \text{ m}
$$

---

## Final Answers

* **Velocity Vector:** $\vec{v}(t) = \left( 2.5t^2 + 2, \, 0.5t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right) \text{ m/s}$

* **Position Vector:** $\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \, \frac{1}{6}t^3 - 2t^2 + 2, \, -\frac{1}{6}t^4 + t - 3 \right) \text{ m}$
