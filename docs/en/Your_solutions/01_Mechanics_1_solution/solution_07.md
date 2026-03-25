# 7. Elimination of Time and Interpretation of Acceleration

This document provides a detailed walkthrough of solving parametric motion equations, finding the trajectory, and analyzing velocity and acceleration.

---

## 1. Key Definitions and Formulas

Before solving the problem, we must establish the mathematical tools required:

### Position Vector ($\vec{r}$)
The position of a particle in a 2D plane is given by:
$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j}
$$

### Velocity ($\vec{v}$)
Velocity is the first derivative of position with respect to time ($t$):
$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = \dot{x}(t)\hat{i} + \dot{y}(t)\hat{j}
$$
The **magnitude** (speed) is calculated using the Pythagorean theorem:
$$
|\vec{v}(t)| = \sqrt{v_x^2 + v_y^2}
$$

### Acceleration ($\vec{a}$)
Acceleration is the first derivative of velocity (or the second derivative of position) with respect to time ($t$):
$$
\vec{a}(t) = \frac{d\vec{v}}{dt} = \ddot{x}(t)\hat{i} + \ddot{y}(t)\hat{j}
$$
The **magnitude** is:
$$
|\vec{a}(t)| = \sqrt{a_x^2 + a_y^2}
$$

### Constant vs. Variable Acceleration
Acceleration is **constant** if and only if both its magnitude and direction do not change over time (i.e., the expression for $\vec{a}(t)$ contains no $t$ terms).

---

## 2. Problem Statement

Given the parametric equations:

$$
x(t) = 2t^2
$$

$$
y(t) = 3t^3
$$

Find the path equation, calculate kinematic vectors, and determine if acceleration is constant.

---

## 3. Step-by-Step Solution

### Step 1: Eliminate the Parameter $t$
To find the relationship between $y$ and $x$, we solve for $t$ in the $x(t)$ equation:

$$
x = 2t^2 \implies t^2 = \frac{x}{2} \implies t = \sqrt{\frac{x}{2}}
$$

Now, substitute this into the $y(t)$ equation:

$$
y = 3t^3 = 3(t^2)^{3/2}
$$

$$
y = 3 \left( \frac{x}{2} \right)^{3/2} = \frac{3}{2\sqrt{2}} x\sqrt{x}
$$

> **Note:** The trajectory is a semi-cubical parabola. Since $x = 2t^2$, $x$ is always non-negative ($x \ge 0$).

---

### Step 2: Calculate Velocity $\vec{v}(t)$ and Speed $|\vec{v}(t)|$
We differentiate the components with respect to $t$:

$$
v_x(t) = \frac{dx}{dt} = \frac{d}{dt}(2t^2) = 4t
$$

$$
v_y(t) = \frac{dy}{dt} = \frac{d}{dt}(3t^3) = 9t^2
$$

**Velocity Vector:**

$$
\vec{v}(t) = 4t\hat{i} + 9t^2\hat{j}
$$

**Magnitude (Speed):**

$$
|\vec{v}(t)| = \sqrt{(4t)^2 + (9t^2)^2} = \sqrt{16t^2 + 81t^4} = t\sqrt{16 + 81t^2}
$$

---

### Step 3: Calculate Acceleration $\vec{a}(t)$ and Magnitude $|\vec{a}(t)|$
Differentiate the velocity components:

$$
a_x(t) = \frac{dv_x}{dt} = 4
$$

$$
a_y(t) = \frac{dv_y}{dt} = 18t
$$

**Acceleration Vector:**

$$
\vec{a}(t) = 4\hat{i} + 18t\hat{j}
$$

**Magnitude:**

$$
|\vec{a}(t)| = \sqrt{4^2 + (18t)^2} = \sqrt{16 + 324t^2} = 2\sqrt{4 + 81t^2}
$$

---

### Step 4: Is the acceleration constant?
By looking at the acceleration vector $\vec{a}(t) = 4\hat{i} + 18t\hat{j}$:

* The $x$-component is constant ($4$).
* The $y$-component **depends on $t$** ($18t$).

Since the $y$-component changes as time passes, the acceleration is **not constant**.

---

## 4. Summary Table

| Quantity | Expression |
| :--- | :--- |
| **Path Equation** | $y = \frac{3}{2\sqrt{2}}x^{3/2}$ |
| **Velocity Vector** | $(4t, 9t^2)$ |
| **Acceleration Vector** | $(4, 18t)$ |
| **Constant Accel?** | **No** (Depends on time $t$) |

---

## 5. Trajectory Visualization
The path starts at the origin $(0,0)$ and curves upwards. Because the power of $x$ is $1.5$, it rises more steeply than a standard parabola ($x^2$) but less steeply than a cubic function ($x^3$) relative to $x$.
