# The Fly and the Bicycle Problem

## 1. Key Definitions & Formulas

To solve this problem efficiently, we need to understand the relationship between distance, constant speed, and time.

* **Constant Speed Formula**: The relationship between distance ($d$), speed ($v$), and time ($t$) is given by:

$$
d = v \cdot t
$$

* **Relative Speed**: When two objects move toward each other, their relative speed is the sum of their individual speeds.
* **Total Distance**: For an object moving at a constant speed, the total distance traveled is the product of its speed and the *total duration* of its travel, regardless of how many times it changes direction.

---

## 2. Step-by-Step Solution

### Step 1: Calculate the total time until impact
Instead of calculating every "zig-zag" the fly makes, we first determine how long the bicycle takes to reach the wall. Since the bicycle's speed is constant, the fly will stop flying exactly when the bicycle hits the wall.

Given:
* Initial distance ($d_b$) = $10\text{ m}$
* Bicycle speed ($v_b$) = $1\text{ m/s}$

Using $t = \frac{d}{v}$:

$$
t = \frac{10\text{ m}}{1\text{ m/s}} = 10\text{ s}
$$

The entire "event" lasts exactly **10 seconds**.

### Step 2: Analyze the fly's motion
We know the fly is moving at a constant speed of $2\text{ m/s}$ throughout these 10 seconds. Even though the fly changes direction every time it hits the wall or the bicycle, its **speed** remains constant.

Given:
* Fly speed ($v_f$) = $2\text{ m/s}$
* Total time ($t$) = $10\text{ s}$

### Step 3: Calculate total distance
The total distance ($D_f$) traveled by the fly is simply its speed multiplied by the total time it was in the air:

$$
D_f = v_f \cdot t
$$

$$
D_f = 2\text{ m/s} \cdot 10\text{ s} = 20\text{ m}
$$

---

## 3. Conclusion
The fly travels a total distance of **20 meters** before it is crushed against the wall.

> **Note on the Infinite Series:** While you *could* solve this by summing the infinite geometric series of each leg of the fly's journey, the time-based approach is the "logical" shortcut that simplifies the math significantly.
