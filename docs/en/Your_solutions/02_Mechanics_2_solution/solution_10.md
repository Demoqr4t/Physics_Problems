# Kinematics and Dynamics: Vector Calculus in Physics

## Definitions and Key Concepts

**Position Vector ($\vec{r}$):** A vector that represents the location of a particle in space relative to an origin. It is typically expressed in Cartesian coordinates as $\vec{r}(t) = (x(t), y(t), z(t))$.

**Velocity ($\vec{v}$):** The rate of change of position with respect to time. It is the first derivative of the position vector.

**Acceleration ($\vec{a}$):** The rate of change of velocity with respect to time. It is the first derivative of the velocity vector and the second derivative of the position vector.

**Momentum ($\vec{p}$):** The product of a particle's mass and its velocity. It represents the quantity of motion an object has.

**Newton's Second Law ($\vec{F}$):** The net force acting on a particle is equal to its mass multiplied by its acceleration.

**Mechanical Power ($P$):** The rate at which work is done or energy is transferred by a force. For a particle, it is calculated as the dot product of the force vector and the velocity vector.

---

## Key Formulas

**Kinematic Derivatives:**

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \left( \frac{dx}{dt}, \frac{dy}{dt}, \frac{dz}{dt} \right)
$$

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \left( \frac{dv_x}{dt}, \frac{dv_y}{dt}, \frac{dv_z}{dt} \right)
$$

**Kinematic Integrals:**

$$
\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0
$$

$$
\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0
$$

**Dynamics:**

$$
\vec{p}(t) = m\vec{v}(t)
$$

$$
\vec{F}(t) = m\vec{a}(t)
$$

**Power:**

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t) = F_x v_x + F_y v_y + F_z v_z
$$

---

## Problem 1: Force field and power

**Question:** In a certain force field, the equations of motion of a particle with mass $m=0.5$ kg are: $x = 5t^2 - t$, $y = 2t^3$, $z = -3t + 2$. Find the time dependence of the particle's velocity, momentum, acceleration, force, and power.

### Step-by-Step Solution

**Step 1: Write down the position vector and identify mass**
* Mass ($m$) = $0.5$ kg
* $\vec{r}(t) = (5t^2 - t, 2t^3, -3t + 2)$

**Step 2: Calculate Velocity**
Take the first derivative of each component of the position vector with respect to time ($t$).

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \left( \frac{d}{dt}(5t^2 - t), \frac{d}{dt}(2t^3), \frac{d}{dt}(-3t + 2) \right)
$$

$$
\vec{v}(t) = (10t - 1, 6t^2, -3) \text{ m/s}
$$

**Step 3: Calculate Momentum**
Multiply the mass by the velocity vector.

$$
\vec{p}(t) = m\vec{v}(t) = 0.5 \cdot (10t - 1, 6t^2, -3)
$$

$$
\vec{p}(t) = (5t - 0.5, 3t^2, -1.5) \text{ kg}\cdot\text{m/s}
$$

**Step 4: Calculate Acceleration**
Take the derivative of the velocity vector with respect to time.

$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \left( \frac{d}{dt}(10t - 1), \frac{d}{dt}(6t^2), \frac{d}{dt}(-3) \right)
$$

$$
\vec{a}(t) = (10, 12t, 0) \text{ m/s}^2
$$

**Step 5: Calculate Force**
Use Newton's Second Law ($\vec{F} = m\vec{a}$).

$$
\vec{F}(t) = 0.5 \cdot (10, 12t, 0)
$$

$$
\vec{F}(t) = (5, 6t, 0) \text{ N}
$$

**Step 6: Calculate Power**
Compute the dot product of the Force and Velocity vectors.

$$
P(t) = \vec{F}(t) \cdot \vec{v}(t) = (F_x \cdot v_x) + (F_y \cdot v_y) + (F_z \cdot v_z)
$$

$$
P(t) = (5 \cdot (10t - 1)) + (6t \cdot 6t^2) + (0 \cdot -3)
$$

$$
P(t) = (50t - 5) + (36t^3) + 0
$$

$$
P(t) = 36t^3 + 50t - 5 \text{ W}
$$

---

## Problem 2: Dynamics with a time-dependent force

**Question:** A particle of mass $m=3$ kg moves in a force field $\vec{F} = (15t, 3t-12, -6t^2)$ N. Given initial conditions $\vec{r}_0=(5,2,-3)$ m and $\vec{v}_0=(2,0,1)$ m/s, find the dependence of the particle's position and velocity on time.

### Step-by-Step Solution

**Step 1: Identify given variables**
* Mass ($m$) = $3$ kg
* Force ($\vec{F}(t)$) = $(15t, 3t-12, -6t^2)$ N
* Initial Velocity ($\vec{v}_0$) = $(2, 0, 1)$ m/s
* Initial Position ($\vec{r}_0$) = $(5, 2, -3)$ m

**Step 2: Find Acceleration**
Divide the force vector by the mass.

$$
\vec{a}(t) = \frac{\vec{F}(t)}{m} = \left( \frac{15t}{3}, \frac{3t-12}{3}, \frac{-6t^2}{3} \right)
$$

$$
\vec{a}(t) = (5t, t-4, -2t^2) \text{ m/s}^2
$$

**Step 3: Determine Velocity via Integration**
Integrate the acceleration vector with respect to time. We will add the integration constants which correspond to the initial velocity components ($v_{0x}=2, v_{0y}=0, v_{0z}=1$).

$$
\vec{v}(t) = \int \vec{a}(t) \, dt + \vec{v}_0
$$

* $v_x(t) = \int 5t \, dt + 2 = 2.5t^2 + 2$
* $v_y(t) = \int (t - 4) \, dt + 0 = 0.5t^2 - 4t$
* $v_z(t) = \int (-2t^2) \, dt + 1 = -\frac{2}{3}t^3 + 1$

$$
\vec{v}(t) = \left( 2.5t^2 + 2, \, 0.5t^2 - 4t, \, -\frac{2}{3}t^3 + 1 \right) \text{ m/s}
$$

**Step 4: Determine Position via Integration**
Integrate the velocity vector with respect to time. The integration constants will correspond to the initial position components ($r_{0x}=5, r_{0y}=2, r_{0z}=-3$).

$$
\vec{r}(t) = \int \vec{v}(t) \, dt + \vec{r}_0
$$

* $x(t) = \int (2.5t^2 + 2) \, dt + 5 = \left(\frac{2.5}{3}t^3 + 2t\right) + 5 = \frac{5}{6}t^3 + 2t + 5$
* $y(t) = \int (0.5t^2 - 4t) \, dt + 2 = \left(\frac{0.5}{3}t^3 - \frac{4}{2}t^2\right) + 2 = \frac{1}{6}t^3 - 2t^2 + 2$
* $z(t) = \int \left(-\frac{2}{3}t^3 + 1\right) \, dt - 3 = \left(-\frac{2}{12}t^4 + t\right) - 3 = -\frac{1}{6}t^4 + t - 3$

$$
\vec{r}(t) = \left( \frac{5}{6}t^3 + 2t + 5, \, \frac{1}{6}t^3 - 2t^2 + 2, \, -\frac{1}{6}t^4 + t - 3 \right) \text{ m}
$$
