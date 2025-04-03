# Orbital Period and Orbital Radius

## Motivation

The relationship between the square of the orbital period and the cube of the orbital radius, known as **Kepler's Third Law**, forms a foundational pillar of celestial mechanics. It reveals the harmony of planetary motion and provides a gateway to calculating distances and masses in space.

---

## Kepler's Third Law: Derivation for Circular Orbits

From Newton's law of gravitation and centripetal force:

## Kepler’s Third Law

## Kepler’s Third Law

From Newton’s law of gravitation and the requirement for centripetal force:

$$
F = \frac{G M m}{r^2} = m \frac{v^2}{r} \Rightarrow v = \sqrt{\frac{G M}{r}}
$$

Orbital period $T$ is the time taken to complete one full orbit:

$$
T = \frac{2 \pi r}{v} = 2 \pi r \cdot \sqrt{\frac{r}{G M}} = 2 \pi \sqrt{\frac{r^3}{G M}}
$$

Thus:

$$
T^2 = \frac{4 \pi^2}{G M} r^3
$$

This shows:

$$
T^2 \propto r^3
$$



---

## Python Simulation for Verification

```python
import numpy as np
import matplotlib.pyplot as plt

# Constants
G = 6.67430e-11       # m^3 kg^-1 s^-2
M = 5.972e24          # kg (mass of Earth)

# Orbital radii (in meters)
radii = np.linspace(7e6, 4.2e7, 100)  # from LEO to GEO

# Calculate orbital periods
periods = 2 * np.pi * np.sqrt(radii**3 / (G * M))

# Plot T^2 vs r^3
plt.figure(figsize=(8, 6))
plt.plot(radii**3, periods**2)
plt.xlabel("$r^3$ (m³)")
plt.ylabel("$T^2$ (s²)")
plt.title("Kepler's Third Law: $T^2$ vs $r^3$")
plt.grid(True)
plt.show()
```

---

## Applications in Astronomy

- **Planetary Motion**: By observing $T$, we can estimate orbital radius $r$.
- **Satellite Orbits**: Used to determine periods for communication and GPS satellites.
- **Binary Star Systems**: Inferring masses from orbital characteristics.

---

## Real-World Example: Moon

- Orbital radius: $r = 3.84 \times 10^8$ m
- $T = 2\pi \sqrt{\frac{r^3}{G M}} \approx 2.36 \times 10^6$ s $\approx$ 27.3 days

