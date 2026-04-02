# Work of a Variable Force: The Spring-Mass System

## Definitions and Key Concepts

**Variable Force:** A force whose magnitude and/or direction changes with position or time. In this problem, the force depends entirely on the position $x$.

**Restoring Force (Hooke's Law):** A force that acts to bring a body to its equilibrium position. The force $F(x) = -kx$ is the classic example, where $k$ is the spring constant (a measure of stiffness) and the negative sign indicates the force always points opposite to the displacement $x$.

**Equation of Motion:** A mathematical differential equation that describes the behavior of a physical system in terms of its motion as a function of time. Derived using Newton's Second Law.

**Work ($W$):** The energy transferred to or from an object via the application of force along a displacement. For a variable force, it is the integral of the force with respect to displacement.

**Potential Energy ($U$):** The energy possessed by a body by virtue of its position relative to others, stresses within itself, electric charge, and other factors. For conservative forces (like a spring force), the work done by the force equals the negative change in potential energy.

---

## Key Formulas

**Newton's Second Law (1D):**

$$
F = m \frac{d^2x}{dt^2} = ma
$$

**Work Done by a Variable Force:**

$$
W = \int_{x_i}^{x_f} F(x) dx
$$

**Relationship between Conservative Force and Potential Energy:**

$$
W = -\Delta U = -(U_f - U_i)
$$

$$
F(x) = -\frac{dU}{dx}
$$

---

## Step-by-Step Solution

### 1. Write down the equation of motion and solve it

**The Equation of Motion:**
We start with Newton's Second Law, $F = ma$. Acceleration $a$ is the second derivative of position with respect to time ($a = \frac{d^2x}{dt^2}$).

Setting the net force equal to the restoring force:

$$
m \frac{d^2x}{dt^2} = -kx
$$

Rearranging this gives us a homogeneous second-order linear ordinary differential equation:

$$
\frac{d^2x}{dt^2} + \frac{k}{m}x = 0
$$

To simplify, we define the angular frequency $\omega$ as:

$$
\omega = \sqrt{\frac{k}{m}} \implies \omega^2 = \frac{k}{m}
$$

Substituting this back, we get the standard equation for Simple Harmonic Motion (SHM):

$$
\frac{d^2x}{dt^2} + \omega^2 x = 0
$$

**Solving the Equation:**
The general solution to this differential equation is a combination of sine and cosine functions (or a single phase-shifted cosine/sine), because their second derivatives are proportional to their negative selves.

$$
x(t) = C_1 \cos(\omega t) + C_2 \sin(\omega t)
$$

Alternatively, this is often written in terms of an amplitude $A$ and a phase constant $\phi$:

$$
x(t) = A \cos(\omega t + \phi)
$$

*(Note: $A$ and $\phi$ are determined by the initial conditions of the system, such as initial position and velocity).*

### 2. Calculate the work done during the displacement from $0$ to $x_0$

To find the work done by the variable force $F(x) = -kx$, we must integrate the force over the displacement from $x = 0$ to $x = x_0$.

$$
W = \int_{0}^{x_0} F(x) dx
$$

Substitute the given force equation:

$$
W = \int_{0}^{x_0} (-kx) dx
$$

Since $-k$ is a constant, pull it out of the integral:

$$
W = -k \int_{0}^{x_0} x dx
$$

Use the power rule for integration ($\int x^n dx = \frac{x^{n+1}}{n+1}$):

$$
W = -k \left[ \frac{1}{2} x^2 \right]_{0}^{x_0}
$$

Evaluate the definite integral from $0$ to $x_0$:

$$
W = -k \left( \frac{1}{2} x_0^2 - \frac{1}{2} (0)^2 \right)
$$

$$
W = -\frac{1}{2} k x_0^2
$$

*Explanation: The work done by the spring force is negative because the force pulls in the opposite direction of the displacement (which went from 0 to a positive $x_0$).*

### 3. Interpret the result as potential energy

For a conservative force, the work done by the system is equal to the negative change in potential energy ($\Delta U$):

$$
W = -\Delta U = -(U(x_0) - U(0))
$$

We established that $W = -\frac{1}{2} k x_0^2$. Setting these equal:

$$
-\frac{1}{2} k x_0^2 = -(U(x_0) - U(0))
$$

If we define the reference point for potential energy such that the potential energy at equilibrium is zero ($U(0) = 0$), the equation simplifies to:

$$
\frac{1}{2} k x_0^2 = U(x_0)
$$

*Interpretation: The negative work done by the spring against the stretching motion is stored in the spring as elastic potential energy. To stretch the spring to $x_0$, an external agent must do positive work equal to $\frac{1}{2} k x_0^2$, which becomes the stored potential energy $U(x)$.*

### 4. Verify the relationship $F = -\frac{dU}{dx}$

We now have the generalized potential energy function:

$$
U(x) = \frac{1}{2} k x^2
$$

We are given the relationship that force is the negative derivative of potential energy with respect to position. Let's test this:

$$
F(x) = -\frac{d}{dx} \left( \frac{1}{2} k x^2 \right)
$$

Bring the constant $\frac{1}{2}k$ outside the derivative:

$$
F(x) = -\frac{1}{2} k \frac{d}{dx} (x^2)
$$

Apply the power rule for differentiation ($\frac{d}{dx} x^n = nx^{n-1}$):

$$
F(x) = -\frac{1}{2} k (2x)
$$

The $2$ and the $\frac{1}{2}$ cancel out:

$$
F(x) = -kx
$$

*Verification successful! Taking the negative spatial derivative of our potential energy function returns exactly our original restoring force.*

### 5. Draw the graph of $F(x)$ and $U(x)$

While I cannot generate standard image files directly in Markdown text, here is a precise description and ASCII representation of what these graphs look like.

**Graph of Force: $F(x) = -kx$**
* **Shape:** A straight line passing through the origin $(0,0)$.
* **Slope:** Negative (specifically, $-k$).
* **Interpretation:** In the positive $x$ region (spring is stretched), the force is negative (pulling back). In the negative $x$ region (spring is compressed), the force is positive (pushing forward).

```text
       F(x)
        |
        |  \
        |   \
        |    \ 
--------+-----\-------- x (Displacement)
        |      \
        |       \
        |        \
