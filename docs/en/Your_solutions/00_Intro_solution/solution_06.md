# Function Analysis: Finding Local Extrema

This document provides a step-by-step calculus-based analysis of the function:

$$
f(x) = 3x^2 - 12x + 7
$$

---

## 1. Key Definitions and Formulas

To find the local maxima or minima of a function, we use the following concepts:

* **The First Derivative ($f'(x)$):** Represents the slope of the tangent line. Local extrema occur where the slope is zero.
* **Critical Point:** A value $c$ in the domain where $f'(c) = 0$ or $f'(c)$ is undefined.
* **Power Rule:** A basic differentiation rule:
  
$$
\frac{d}{dx}[ax^n] = anx^{n-1}
$$

* **The Second Derivative Test:** * If $f''(c) > 0$, the function is concave up, and $f(c)$ is a **local minimum**.
    * If $f''(c) < 0$, the function is concave down, and $f(c)$ is a **local maximum**.

---

## 2. Step-by-Step Solution

### Step 1: Find the First Derivative
We apply the power rule to each term of $f(x) = 3x^2 - 12x + 7$.

$$
f'(x) = 6x - 12
$$

### Step 2: Identify Critical Points
To find where the "peaks" or "valleys" are, we set the first derivative to zero and solve for $x$:

$$
6x - 12 = 0
$$

$$
6x = 12
$$

$$
x = 2
$$

There is one critical point at **$x = 2$**.

### Step 3: Use the Second Derivative Test
To determine if this point is a maximum or a minimum, we find the second derivative $f''(x)$:

$$
f''(x) = \frac{d}{dx}[6x - 12] = 6
$$

Since $f''(2) = 6$, and **$6 > 0$**, the function is concave up at this point. This confirms that $x = 2$ is a **local minimum**.

### Step 4: Find the Coordinates of the Minimum
Substitute $x = 2$ back into the original function $f(x)$ to find the y-coordinate:

$$
f(2) = 3(2)^2 - 12(2) + 7
$$

$$
f(2) = 3(4) - 24 + 7
$$

$$
f(2) = 12 - 24 + 7 = -5
$$

---

## 3. Conclusion

The function $f(x) = 3x^2 - 12x + 7$ has:

* **Local Minimum:** at $(2, -5)$
* **Local Maximum:** None (the function extends to infinity as $x$ increases or decreases).
