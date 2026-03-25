# 7. Elimination of Time and Interpretation of Acceleration

This guide explains how to convert parametric equations of motion into a path equation and how to break down acceleration into its physical components.

---

## 1. Key Definitions and Formulas

### Parametric Equations
Motion is often described by separate functions for each coordinate:

$$
x = x(t), \quad y = y(t)
$$

### Elimination of Time (Path Equation)
To find the trajectory $y = f(x)$, we solve the $x(t)$ equation for $t$ and substitute it into $y(t)$. This "eliminates" the time variable to show the geometric shape of the path.

### Velocity and Acceleration Vectors
The velocity vector $\vec{v}$ and acceleration vector $\vec{a}$ are found by differentiating the position components:

$$
\vec{v} = \frac{dx}{dt}\hat{i} + \frac{dy}{dt}\hat{j}
$$

$$
\vec{a} = \frac{dv_x}{dt}\hat{i} + \frac{dv_y}{dt}\hat{j}
$$

### Tangential and Normal Acceleration
Acceleration can be interpreted as having two components:
1. **Tangential ($a_t$):** Changes the **speed** (magnitude of velocity).
2. **Normal ($a_n$):** Changes the **direction** of motion.

$$
a_t = \frac{d|\vec{v}|}{dt}, \quad a_n = \sqrt{|\vec{a}|^2 - a_t^2}
$$

---

## 2. Example Problem

**Given Equations:**

$$
x(t) = 2t
$$

$$
y(t) = t^2
$$

**Goal:** Eliminate time to find the path equation and interpret the acceleration.

---

## 3. Step-by-Step Solution

### Step 1: Eliminate the Time Variable ($t$)
First, we isolate $t$ from the $x$ equation:

$$
x = 2t \implies t = \frac{x}{2}
$$

Now, substitute this expression for $t$ into the $y$ equation:

$$
y = \left( \frac{x}{2} \right)^2
$$

$$
y = \frac{1}{4}x^2
$$

> **Interpretation:** The path of the object is a **parabola** opening upwards.

---

### Step 2: Find the Velocity Vector $\vec{v}(t)$
Differentiate the position components with respect to time:

$$
v_x = \frac{dx}{dt} = 2
$$

$$
v_y = \frac{dy}{dt} = 2t
$$

The velocity vector is $\vec{v}(t) = (2, 2t)$. The speed (magnitude) is:

$$
|\vec{v}| = \sqrt{2^2 + (2t)^2} = \sqrt{4 + 4t^2} = 2\sqrt{1 + t^2}
$$

---

### Step 3: Find the Acceleration Vector $\vec{a}(t)$
Differentiate the velocity components:

$$
a_x = \frac{dv_x}{dt} = 0
$$

$$
a_y = \frac{dv_y}{dt} = 2
$$

> **Interpretation:** The acceleration is constant, $\vec{a} = (0, 2)$. It points entirely in the positive y-direction.

---

### Step 4: Interpret Acceleration Components
We find the tangential acceleration by differentiating the speed:

$$
a_t = \frac{d}{dt}(2\sqrt{1+t^2}) = 2 \cdot \frac{1}{2\sqrt{1+t^2}} \cdot 2t = \frac{2t}{\sqrt{1+t^2}}
$$

The normal acceleration is found using the Pythagorean relationship:

$$
a_n = \sqrt{|\vec{a}|^2 - a_t^2} = \sqrt{2^2 - \left( \frac{2t}{\sqrt{1+t^2}} \right)^2}
$$

---

## 4. Final Results Summary

| Concept | Result |
| :--- | :--- |
| **Path Equation** | $y = \frac{1}{4}x^2$ (Parabolic) |
| **Velocity Vector** | $\vec{v} = 2\hat{i} + 2t\hat{j}$ |
| **Acceleration Vector** | $\vec{a} = 0\hat{i} + 2\hat{j}$ |
| **Interpretation** | The object accelerates vertically, changing both speed and direction. |
