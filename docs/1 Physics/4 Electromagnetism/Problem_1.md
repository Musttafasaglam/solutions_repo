# Simulating the Effects of the Lorentz Force

## 1. Motivation

The Lorentz force governs the motion of charged particles in electric and magnetic fields. It is given by:

$$
\vec{F} = q\vec{E} + q\vec{v} \times \vec{B}
$$

This force plays a key role in systems such as:

- Particle accelerators
- Mass spectrometers
- Plasma confinement devices
- Cyclotrons and magnetic traps

---

## 2. Task Summary

We simulate and visualize the trajectory of a charged particle under:

- A uniform magnetic field
- Combined electric and magnetic fields
- Crossed electric and magnetic fields

We explore:

- Effects of varying field strengths ($\vec{E}$, $\vec{B}$)
- Initial velocity $\vec{v}$
- Charge $q$ and mass $m$

---

## 3. Python Simulation

```python
import numpy as np
import matplotlib.pyplot as plt

# Constants
q = 1.0      # charge (C)
m = 1.0      # mass (kg)
E = np.array([0.0, 0.0, 0.0])  # electric field (V/m)
B = np.array([0.0, 0.0, 1.0])  # magnetic field (T)

# Initial conditions
v = np.array([1.0, 0.0, 0.0])  # initial velocity (m/s)
r = np.array([0.0, 0.0, 0.0])  # initial position (m)

# Time settings
dt = 0.01
steps = 2000

# Arrays to store trajectory
trajectory = np.zeros((steps, 3))
velocity = np.zeros((steps, 3))

# Euler method
for i in range(steps):
    trajectory[i] = r
    velocity[i] = v
    F = q * (E + np.cross(v, B))
    a = F / m
    v = v + a * dt
    r = r + v * dt

# Plotting
fig = plt.figure()
ax = fig.add_subplot(111)
ax.plot(trajectory[:, 0], trajectory[:, 1])
ax.set_xlabel('x (m)')
ax.set_ylabel('y (m)')
ax.set_title('Trajectory of a Charged Particle in a Uniform Magnetic Field')
ax.grid(True)
plt.axis('equal')
plt.show()
```

---

## 4. Observations

- The particle moves in a circular or helical path in a uniform magnetic field.
- Larmor radius $r_L = \frac{mv_\perp}{qB}$ depends on the perpendicular component of velocity.
- Adding an electric field causes drift and changes trajectory.

---

## 5. Suggestions for Extension

- Vary $\vec{E}$ and $\vec{B}$ for non-uniform fields.
- Implement 3D visualization using `matplotlib` or `plotly`.
- Add Runge-Kutta integration for higher accuracy.

---

## 6. Practical Relevance

- In **cyclotrons**, particles follow spiral paths under Lorentz force.
- In **mass spectrometers**, charge-to-mass ratio is calculated from curvature.
- In **plasma physics**, this governs confinement and drift dynamics.

