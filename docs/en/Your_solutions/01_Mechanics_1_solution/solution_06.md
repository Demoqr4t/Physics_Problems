# Variable Velocity Problem Analysis

This document provides a step-by-step solution for calculating the position and acceleration of an object with a time-dependent velocity function.

---

## 1. Key Definitions and Formulas

To solve problems involving variable velocity, we use the fundamental principles of calculus:

### Acceleration ($a$)
Acceleration is defined as the instantaneous rate of change of velocity with respect to time. Mathematically, it is the first derivative of the velocity function:

$$
a(t) = \frac{dv}{dt} = v'(t)
$$

### Position ($x$)
Position is the integral of velocity with respect to time. Because integration produces a constant ($C$), we use initial conditions (the starting position) to find the specific position function:

$$
x(t) = \int v(t) \, dt + C
$$

---

## 2. Problem Statement

Given the velocity function:

$$
v(t) = t^2 + 2t - 5
$$

**Initial Conditions:**
* At $t = 0$, the position $x = 4$.

**Goal:**
* Find the **acceleration** at $t = 3$.
* Find the **position** at $t = 3$.

---

## 3. Step-by-Step Solution

### Step 1: Calculate Acceleration $a(t)$
We differentiate the velocity function $v(t) = t^2 + 2t - 5$.

$$
a(t) = \frac{d}{dt}(t^2 + 2t - 5)
$$

Applying the power rule ($d/dx[x^n] = nx^{n-1}$):

$$
a(t) = 2t + 2
$$

**Calculation for $t = 3$:**

$$
a(3) = 2(3) + 2 = 8
$$

> **Result:** The acceleration at $t = 3$ is **8 units/s²**.

---

### Step 2: Find the General Position Function $x(t)$
We integrate the velocity function to move from velocity back to position.

$$
x(t) = \int (t^2 + 2t - 5) \, dt
$$

Performing the integration:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + C
$$

---

### Step 3: Solve for the Constant $C$
We use the initial condition: when $t = 0$, $x = 4$.

$$
4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C
$$

$$
4 = 0 + 0 - 0 + C \implies C = 4
$$

The specific position function is:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4
$$

---

### Step 4: Calculate Position at $t = 3$
Substitute $t = 3$ into our specific position function:

$$
x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4
$$

$$
x(3) = \frac{1}{3}(27) + 9 - 15 + 4
$$

$$
x(3) = 9 + 9 - 15 + 4 = 7
$$

> **Result:** The position at $t = 3$ is **7 units**.

---

## 4. Final Results Summary

| Parameter | Function | Value at $t = 3$ |
| :--- | :--- | :--- |
| **Velocity** | $v(t) = t^2 + 2t - 5$ | $10$ |
| **Acceleration** | $a(t) = 2t + 2$ | **8** |
| **Position** | $x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$ | **7** |# Variable Velocity Problem Analysis

This document provides a step-by-step solution for calculating the position and acceleration of an object with a time-dependent velocity function.

---

## 1. Key Definitions and Formulas

To solve problems involving variable velocity, we use the fundamental principles of calculus:

### Acceleration ($a$)
Acceleration is defined as the instantaneous rate of change of velocity with respect to time. Mathematically, it is the first derivative of the velocity function:

$$
a(t) = \frac{dv}{dt} = v'(t)
$$

### Position ($x$)
Position is the integral of velocity with respect to time. Because integration produces a constant ($C$), we use initial conditions (the starting position) to find the specific position function:

$$
x(t) = \int v(t) \, dt + C
$$

---

## 2. Problem Statement

Given the velocity function:

$$
v(t) = t^2 + 2t - 5
$$

**Initial Conditions:**
* At $t = 0$, the position $x = 4$.

**Goal:**
* Find the **acceleration** at $t = 3$.
* Find the **position** at $t = 3$.

---

## 3. Step-by-Step Solution

### Step 1: Calculate Acceleration $a(t)$
We differentiate the velocity function $v(t) = t^2 + 2t - 5$.

$$
a(t) = \frac{d}{dt}(t^2 + 2t - 5)
$$

Applying the power rule ($d/dx[x^n] = nx^{n-1}$):

$$
a(t) = 2t + 2
$$

**Calculation for $t = 3$:**

$$
a(3) = 2(3) + 2 = 8
$$

> **Result:** The acceleration at $t = 3$ is **8 units/s²**.

---

### Step 2: Find the General Position Function $x(t)$
We integrate the velocity function to move from velocity back to position.

$$
x(t) = \int (t^2 + 2t - 5) \, dt
$$

Performing the integration:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + C
$$

---

### Step 3: Solve for the Constant $C$
We use the initial condition: when $t = 0$, $x = 4$.

$$
4 = \frac{1}{3}(0)^3 + (0)^2 - 5(0) + C
$$

$$
4 = 0 + 0 - 0 + C \implies C = 4
$$

The specific position function is:

$$
x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4
$$

---

### Step 4: Calculate Position at $t = 3$
Substitute $t = 3$ into our specific position function:

$$
x(3) = \frac{1}{3}(3)^3 + (3)^2 - 5(3) + 4
$$

$$
x(3) = \frac{1}{3}(27) + 9 - 15 + 4
$$

$$
x(3) = 9 + 9 - 15 + 4 = 7
$$

> **Result:** The position at $t = 3$ is **7 units**.

---

## 4. Final Results Summary

| Parameter | Function | Value at $t = 3$ |
| :--- | :--- | :--- |
| **Velocity** | $v(t) = t^2 + 2t - 5$ | $10$ |
| **Acceleration** | $a(t) = 2t + 2$ | **8** |
| **Position** | $x(t) = \frac{1}{3}t^3 + t^2 - 5t + 4$ | **7** |
