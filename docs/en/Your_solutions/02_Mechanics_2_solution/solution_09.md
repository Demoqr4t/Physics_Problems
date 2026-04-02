# Vertical Throw with Linear Drag



## Definitions and Key Concepts

**Linear Drag Force ($F_d$):** A resistive force exerted by a fluid (like air) that opposes the motion of an object. For relatively slow-moving objects, this force is often modeled as proportional to the velocity ($v$), defined as $F_d = -kv$, where $k$ is the drag coefficient.

**Terminal Velocity ($v_T$):** The constant speed that a freely falling object eventually reaches when the resistance of the medium prevents further acceleration. This occurs when the drag force equals the gravitational pull ($mg = kv_T$, so $v_T = \frac{mg}{k}$).

**Equation of Motion:** Derived from Newton's Second Law ($\Sigma F = ma$), it describes how the forces acting on the object dictate its acceleration ($\frac{dv}{dt}$).

---

## Key Formulas

**Newton's Second Law (with drag):**

$$

m\frac{dv}{dt} = -mg - kv

$$

**Kinematic relationship for position:**

$$

v = \frac{dx}{dt}

$$

---

## Step-by-Step Solution

### 1. Solve the equation by analytical methods

**Step 1.1: Separate the variables**
We start with the equation of motion and rearrange it to group the velocity terms ($v$) on one side and time ($dt$) on the other.

$$

m \frac{dv}{dt} = - (mg + kv)

$$

$$

\frac{dv}{mg + kv} = -\frac{1}{m} dt

$$

**Step 1.2: Integrate to find velocity $v(t)$**
Integrate both sides from time $t = 0$ to $t$, with initial velocity $v(0) = v_0$.

$$

\int_{v_0}^{v} \frac{1}{mg + ku} du = \int_{0}^{t} -\frac{1}{m} d\tau

$$

Using the rule $\int \frac{1}{a + bx} dx = \frac{1}{b} \ln|a + bx|$, we evaluate the left side:

$$

\frac{1}{k} \left[ \ln(mg + kv) - \ln(mg + kv_0) \right] = -\frac{t}{m}

$$

Combine the logarithms:

$$

\ln \left( \frac{mg + kv}{mg + kv_0} \right) = -\frac{k}{m} t

$$

Take the exponential of both sides to solve for $v$:

$$

\frac{mg + kv}{mg + kv_0} = e^{-\frac{k}{m} t}

$$

$$

mg + kv = (mg + kv_0) e^{-\frac{k}{m} t}

$$

$$

v(t) = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t} - \frac{mg}{k}

$$

*Note: $\frac{mg}{k}$ is the terminal velocity magnitude, $v_T$.*

**Step 1.3: Integrate velocity to find position $x(t)$**
Since $v = \frac{dx}{dt}$, we integrate $v(t)$ from $0$ to $t$ to find the position. We know $x(0) = 10$.

$$

x(t) - x(0) = \int_{0}^{t} \left[ \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} \tau} - \frac{mg}{k} \right] d\tau

$$

Evaluating the integral:

$$

x(t) - 10 = \left[ -\frac{m}{k} \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} \tau} - \frac{mg}{k} \tau \right]_{0}^{t}

$$

Apply the limits (subtract the evaluation at $0$ from the evaluation at $t$):

$$

x(t) = 10 + \frac{m}{k} \left( v_0 + \frac{mg}{k} \right) \left( 1 - e^{-\frac{k}{m} t} \right) - \frac{mg}{k} t

$$

### 2. Determine the maximum height

**Step 2.1: Find the time to reach maximum height ($t_{max}$)**
At the maximum height, the instantaneous velocity is zero ($v(t_{max}) = 0$).

$$

0 = \left( v_0 + \frac{mg}{k} \right) e^{-\frac{k}{m} t_{max}} - \frac{mg}{k}

$$

$$

e^{\frac{k}{m} t_{max}} = \frac{v_0 + \frac{mg}{k}}{\frac{mg}{k}} = 1 + \frac{kv_0}{mg}

$$

Taking the natural log of both sides:

$$

t_{max} = \frac{m}{k} \ln \left( 1 + \frac{kv_0}{mg} \right)

$$

**Step 2.2: Calculate the maximum height ($H_{max}$)**
Substitute $t_{max}$ back into the position equation $x(t)$. Notice that $e^{-\frac{k}{m} t_{max}} = \frac{mg}{mg + kv_0}$.

$$

H_{max} = 10 + \frac{m}{k} \left( \frac{mg + kv_0}{k} \right) \left( 1 - \frac{mg}{mg + kv_0} \right) - \frac{mg}{k} \left( \frac{m}{k} \ln \left( 1 + \frac{kv_0}{mg} \right) \right)

$$

Simplify the middle term $\left( 1 - \frac{mg}{mg + kv_0} = \frac{kv_0}{mg + kv_0} \right)$:

$$

H_{max} = 10 + \frac{m}{k} \left( \frac{mg + kv_0}{k} \right) \left( \frac{kv_0}{mg + kv_0} \right) - \frac{m^2 g}{k^2} \ln \left( 1 + \frac{kv_0}{mg} \right)

$$

The term simplifies beautifully to yield the final maximum height equation:

$$

H_{max} = 10 + \frac{mv_0}{k} - \frac{m^2 g}{k^2} \ln \left( 1 + \frac{kv_0}{mg} \right)

$$

### 3. Compare with the case without drag

If we assume no air resistance ($k = 0$), the equations simplify to classic kinematic equations:
* **Velocity:** $v(t) = v_0 - gt$
* **Position:** $x(t) = 10 + v_0t - \frac{1}{2}gt^2$
* **Maximum Height:** $H_{max, no\_drag} = 10 + \frac{v_0^2}{2g}$

**Comparisons:**
1. **Height:** The drag force acts downwards during the ascent, assisting gravity. Therefore, the object with drag will reach a **lower maximum height** than the object without drag ($H_{max} < H_{max, no\_drag}$). 
2. **Time to peak:** Because there is more total downward force acting on the mass ($mg + kv$ instead of just $mg$), the object decelerates faster. It reaches its peak in **less time** than the case without drag.

*(Fun mathematical fact: If you take the Maclaurin series expansion of the natural logarithm in our $H_{max}$ formula for very small $k$, it perfectly reduces to the no-drag formula $10 + \frac{v_0^2}{2g}$!)*

---

### 4. Numerical Simulation (Python)

Here is a Python script using `scipy.integrate.solve_ivp` and `matplotlib` to numerically simulate and plot both cases (with and without drag) for comparison. 

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy.integrate import solve_ivp

# Parameters
m = 1.0       # Mass (kg)
g = 9.81      # Gravity (m/s^2)
k = 0.5       # Drag coefficient (kg/s)
v0 = 20.0     # Initial velocity (m/s)
x0 = 10.0     # Initial position (m)

# 1. Differential equations for the drag case
# state vector y = [x, v]
def drag_system(t, y):
    x, v = y
    dxdt = v
    dvdt = -g - (k/m)*v
    return [dxdt, dvdt]

# 2. Event to stop the simulation when the object hits the ground (x=0)
def hit_ground(t, y):
    return y[0]  # The event is triggered when position is 0
hit_ground.terminal = True
hit_ground.direction = -1

# Time span for the simulation
t_span = (0, 10)
y0 = [x0, v0]

# Solve the system with drag
sol_drag = solve_ivp(drag_system, t_span, y0, events=hit_ground, dense_output=True)

# 3. Calculate the analytical no-drag case for comparison
t_no_drag = np.linspace(0, sol_drag.t[-1], 100)
x_no_drag = x0 + v0*t_no_drag - 0.5*g*t_no_drag**2

# Filter out negative heights for the no-drag plot
t_no_drag = t_no_drag[x_no_drag >= 0]
x_no_drag = x_no_drag[x_no_drag >= 0]

# 4. Plotting the results
plt.figure(figsize=(10, 6))

# Plot drag numerical solution
t_eval = np.linspace(0, sol_drag.t[-1], 200)
y_eval = sol_drag.sol(t_eval)
plt.plot(t_eval, y_eval[0], 'b-', linewidth=2, label='With Linear Drag (Numerical)')

# Plot no drag analytical solution
plt.plot(t_no_drag, x_no_drag, 'r--', linewidth=2, label='No Drag (Analytical)')

# Formatting
plt.title('Vertical Throw: With vs Without Linear Drag')
plt.xlabel('Time (s)')
plt.ylabel('Height (m)')
plt.axhline(0, color='black', lw=1)
plt.grid(True)
plt.legend()

plt.show()
