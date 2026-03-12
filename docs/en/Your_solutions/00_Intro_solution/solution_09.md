To find the dimensions that maximize the area, we need to express the area as a function of one variable and then find its maximum value using calculus.

### 1. Define the Rectangle

Since the rectangle is in the first quadrant and sits under the curve $y = 3 - x^2$, its vertices are:

* $(0, 0)$ at the origin.
* $(x, 0)$ on the x-axis.
* $(x, y)$ on the curve.
* $(0, y)$ on the y-axis.

The dimensions of the rectangle are **width = $x$** and **height = $y$**.

### 2. Set Up the Area Function

The area $A$ of the rectangle is:


$$A = x \cdot y$$

Since the point $(x, y)$ lies on the curve $y = 3 - x^2$, we can substitute $y$:


$$A(x) = x(3 - x^2)$$

$$A(x) = 3x - x^3$$

### 3. Find the Critical Points

To find the maximum area, take the derivative of $A(x)$ with respect to $x$ and set it to zero:


$$A'(x) = 3 - 3x^2$$

$$0 = 3 - 3x^2$$

$$3x^2 = 3$$

$$x^2 = 1$$

$$x = 1$$

 (We take the positive value since we are in the first quadrant).

### 4. Verify the Maximum

To ensure this is a maximum, we can check the second derivative:


$$A''(x) = -6x$$


At $x = 1$, $A''(1) = -6$, which is negative. This confirms that $x = 1$ is a **local maximum**.

### 5. Calculate the Dimensions

Now, find the corresponding height $y$ using the curve equation:


$$y = 3 - (1)^2$$

$$y = 2$$

---

### Final Answer:

The dimensions of the rectangle with the maximum area are:

* **Width ($x$):** $1$
* **Height ($y$):** $2$

The maximum area itself would be $A = 1 \times 2 = 2$.

