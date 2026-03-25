# 10. Kinematics: 3D Parametric Motion and Path Length

This analysis examines the motion of a point $M$ moving in three-dimensional space along a trajectory defined by trigonometric and linear components.

---

## 1. Key Definitions and Formulas

To analyze motion in 3D, we use the following calculus-based definitions:

### Position Vector ($\vec{r}$)
The position of a particle in 3D space is given by its components along the $x$, $y$, and $z$ axes:

$$
\vec{r}(t) = x(t)\hat{i} + y(t)\hat{j} + z(t)\hat{k}
$$

### Velocity Vector ($\vec{v}$)
Velocity is the derivative of position with respect to time:

$$
\vec{v}(t) = \frac{d\vec{r}}{dt} = (\dot{x}, \dot{y}, \dot{z})
$$

### Path Length ($s$)
The total distance traveled along a curve from time $0$ to $t_0$ is the integral of the speed (magnitude of velocity):

$$
s = \int_{0}^{t_0} |\vec{v}(t)| \, dt = \int_{0}^{t_0} \sqrt{\left(\frac{dx}{dt}\right)^2 + \left(\frac{dy}{dt}\right)^2 + \left(\frac{dz}{dt}\right)^2} \, dt
$$

---

## 2. Problem Statement

A point $M$ moves according to:

$$
x(t) = a \cos(\omega t)
$$

$$
y(t) = b \sin(\omega t)
$$

$$
z(t) = bt
$$

Where $a, b, \omega > 0$ are constants.

---

## 3. Step-by-Step Solution

### a) Finding the Trajectory Equation
To find the geometric path, we eliminate the parameter $t$. Let's look at the relationship between $x$ and $y$:

$$
\frac{x}{a} = \cos(\omega t), \quad \frac{y}{b} = \sin(\omega t)
$$

Using the trigonometric identity $\cos^2(\theta) + \sin^2(\theta) = 1$:

$$
\left(\frac{x}{a}\right)^2 + \left(\frac{y}{b}\right)^2 = 1
$$

This equation represents an **elliptical cylinder** extending along the $z$-axis. Since $z = bt$, the point moves upward at a constant rate while circling this cylinder.

**Result:** The trajectory is an **elliptical helix**.



---

### b) Computing the Path Length from $t=0$ to $t=t_0$
First, we find the velocity components:

$$
v_x = \frac{dx}{dt} = -a\omega \sin(\omega t)
$$

$$
v_y = \frac{dy}{dt} = b\omega \cos(\omega t)
$$

$$
v_z = \frac{dz}{dt} = b
$$

Now, calculate the speed $|\vec{v}(t)|$:

$$
|\vec{v}(t)| = \sqrt{(-a\omega \sin(\omega t))^2 + (b\omega \cos(\omega t))^2 + b^2}
$$

$$
|\vec{v}(t)| = \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2}
$$

The path length $s$ is:

$$
s = \int_{0}^{t_0} \sqrt{a^2\omega^2 \sin^2(\omega t) + b^2\omega^2 \cos^2(\omega t) + b^2} \, dt
$$

**Special Case ($a = b$):** If $a = b$, the expression simplifies significantly using $\sin^2 + \cos^2 = 1$:

$$
s = \int_{0}^{t_0} \sqrt{a^2\omega^2 + b^2} \, dt = t_0 \sqrt{a^2\omega^2 + b^2}
$$

*(Note: For $a \neq b$, this integral is an "Elliptic Integral of the second kind", which typically requires numerical methods or tables to solve exactly.)*

---

### c) Visualization and Special Cases
Below is a Python script using `matplotlib` to visualize this trajectory.

```python
import numpy as np
import matplotlib.pyplot as plt

# Constants
a, b, omega = 5, 3, 0.5
t0 = 20
t = np.linspace(0, t0, 1000)

# Parametric equations
x = a * np.cos(omega * t)
y = b * np.sin(omega * t)
z = b * t

# Plotting
fig = plt.figure(figsize=(10, 7))
ax = fig.add_subplot(111, projection='3d')
ax.plot(x, y, z, label='Trajectory (Elliptical Helix)', color='blue')

ax.set_xlabel('X axis')
ax.set_ylabel('Y axis')
ax.set_zlabel('Z axis')
ax.set_title(f'Trajectory for a={a}, b={b}, omega={omega}')
plt.legend()
plt.show()
