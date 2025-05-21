#  Measurements

##  Problem 1: Measuring Earth's Gravitational Acceleration with a Pendulum

---

###  Motivation

The acceleration $g$ due to gravity is a fundamental constant that influences a wide range of physical phenomena. Measuring $g$ accurately is crucial for understanding gravitational interactions, designing structures, and conducting experiments in various fields.

One classic method for determining $g$ is through the oscillations of a simple pendulum, where the period of oscillation depends on the local gravitational field.

---

###  Task

Measure the acceleration $g$ due to gravity using a pendulum and analyze in detail the uncertainties in the measurements.

> This exercise emphasizes rigorous measurement practices, uncertainty analysis, and their role in experimental physics.

---

###  Calculations

#### 1. Calculate the period

$$
T = \frac{\overline{T_{10}}}{10}, \quad \Delta T = \frac{\Delta T_{10}}{10}
$$

#### 2. Determine $g$

$$
g = \frac{4\pi^2 L}{T^2}
$$

#### 3. Propagate uncertainties

$$
\Delta g = g \sqrt{ \left( \frac{\Delta L}{L} \right)^2 + \left( 2 \cdot \frac{\Delta T}{T} \right)^2 }
$$

---

###  Analysis

1. Compare your measured $g$ with the standard value ($9.81 \, \text{m/s}^2$).
2. Discuss:
   - The effect of measurement resolution on $\Delta L$.
   - Variability in timing and its impact on $\Delta T$.
   - Any assumptions or experimental limitations.

---

###  Deliverables

#### 1. Tabulated data in markdown

| Quantity        | Value               |
|----------------|---------------------|
| $L$             | ... m               |
| $\Delta L$      | ... m               |
| $T_{10}$ values | [t1, t2, ..., t10]  |
| $\overline{T_{10}}$ | ... s           |
| $\sigma_T$      | ... s               |
| $\Delta T$      | ... s               |
| $g$             | ... m/s²            |
| $\Delta g$      | ... m/s²            |

#### 2. Discussion on uncertainties

- Discuss how the resolution of your measuring tools contributes to $\Delta L$.
- Analyze how human reaction time or stopwatch accuracy impacts $\Delta T$.
- Mention assumptions such as small-angle approximation, air resistance, and ideal string properties.

---


