#  Measurements

##  Problem 1: Measuring Earth's Gravitational Acceleration with a Pendulum

---

###  Motivation

The acceleration $$g$$ due to gravity is a fundamental constant that influences a wide range of physical phenomena. Measuring $$g$$ accurately is crucial for understanding gravitational interactions, designing structures, and conducting experiments in various fields.

One classic method for determining $$g$$ is through the oscillations of a simple pendulum, where the period of oscillation depends on the local gravitational field.

---

###  Task

Measure the acceleration $$g$$ due to gravity using a pendulum and analyze in detail the uncertainties in the measurements.

> This exercise emphasizes rigorous measurement practices, uncertainty analysis, and their role in experimental physics.

---

###  Procedure

#### 1. Materials

- A string (1 or 1.5 meters long)
- A small weight (e.g., bag of coins, bag of sugar, key chain)
- Stopwatch (or smartphone timer)
- Ruler or measuring tape

#### 2. Setup

- Attach the weight to the string and fix the other end to a sturdy support.
- Measure the length of the pendulum, $$L$$, from the suspension point to the center of the weight.
- Record the resolution of the measuring tool and calculate the uncertainty as:

$$
\Delta L = \frac{\text{Ruler Resolution}}{2}
$$

#### 3. Data Collection

- Displace the pendulum slightly ($$<15^\circ$$) and release it.
- Measure the time for 10 full oscillations ($$T_{10}$$), and repeat this 10 times.
- Calculate the mean time for 10 oscillations ($$\overline{T_{10}}$$) and the standard deviation ($$\sigma_T$$).
- Determine the uncertainty in the mean time using:

$$
\Delta T_{10} = \frac{\sigma_T}{\sqrt{n}} \quad \text{where } n = 10
$$

---

###  Calculations

#### 1. Calculate the period

$$
T = \frac{\overline{T_{10}}}{10}, \quad \Delta T = \frac{\Delta T_{10}}{10}
$$

#### 2. Determine $$g$$

$$
g = \frac{4\pi^2 L}{T^2}
$$

#### 3. Propagate uncertainties

$$
\Delta g = g \cdot \sqrt{\left( \frac{\Delta L}{L} \right)^2 + \left( 2 \cdot \frac{\Delta T}{T} \right)^2}
$$

---

###  Analysis

#### 1. Compare your measured $$g$$ with the standard value

$$
g_{\text{standard}} = 9.81 \, \text{m/s}^2
$$

#### 2. Discuss

- The effect of measurement resolution on $$\Delta L$$
- Variability in timing and its impact on $$\Delta T$$
- Any assumptions or experimental limitations

#### 3. Visualization: Histogram of Timing Variability



> This histogram shows the spread of simulated $$T_{10}$$ values. The dashed red line marks the mean of the measurements.

---

![alt text](image.png)
