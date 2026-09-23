# Chronos Quantum: Universal Spacetime & Chronometry Engine

An interactive, high-precision web application modeling the physics, standards, and historical evolution of time measurement—from ancient elemental clocks to atomic SI standards and relativistic exoplanetary dynamics.

---

## Overview

Chronos Quantum is a zero-dependency, single-page application built with HTML5 Canvas, Tailwind CSS, and vanilla modern JavaScript. All visualization engines and counters are synchronized directly to a unified real-time clock epoch, preventing background lag and multi-engine phase drifts.

---

## The 9 Integrated Engines

### 1. 24-Hour Earth Analog Precision Clock
* Continuous sweeping 24-hour dial representing full planetary diurnal rotation.
* High-speed dual sub-dials tracking active millisecond ($0-1000\text{ ms}$) and microsecond ($0-1000\ \mu\text{s}$) progression.
* Synchronized digital microsecond readout.

### 2. Cesium-133 Atomic Fountain Engine
* Visual simulation of an atomic fountain clock with cold atoms propelled through a Ramsey microwave cavity ($9.192631770\text{ GHz}$).
* Dynamic hyperfine transition simulation ($F=3 \to F=4$).
* Hardware-aware delta-time ($\Delta t$) physics loop that normalizes toss velocity and gravity across varying mobile and desktop refresh rates (30 Hz to 120 Hz).
* Continuous cumulative cycle counter synchronized with the real-time SI definition and 1-hour resonance milestone target of $33,093,474,372,000\text{ cycles}$.

### 3. Strontium-87 Optical Lattice Clock
* 2D optical lattice simulation representing Strontium atoms held in an optical dipole trap.
* Visual laser probe frequency sweep triggering electronic state excitation ($^1S_0 \to\, ^3P_0$).
* Tracking optical oscillations at $429.228\text{ THz}$ ($429,228,004,229,873\text{ Hz}$).

### 4. Relativistic 1-Light-Second Photon Engine
* Light-clock demonstration with stationary emitter and receiver plates separated by a fixed distance $d = 299,792.458\text{ km}$.
* Fixed single-leg transit duration of $\Delta t = d / c \equiv 1.000\text{ s}$.
* Real-time light-propagation distance metric outputting cumulative displacement in Light-Seconds and Light-Years.

### 5. Mars 1 Sol Planetary Clock
* Martian solar day tracking based on $1\text{ Sol} = 88,775.244\text{ Earth seconds}$.
* Epoch resets deterministically from `00:00:00.000` Martian time.
* Martian second time dilation ratio ($1.02749125\times$ stretched relative to Earth SI seconds).
* Interactive planetary globe rendering diurnal terminator angles and rotational arc percentage.

### 6. Proxima Centauri b Exoplanetary Clock
* Orbital tracking of the habitable-zone exoplanet orbiting Proxima Centauri with a period of $T = 11.186\text{ Earth days}$ and semi-major axis $a \approx 7,267,000\text{ km}$.
* Dynamic Euclidean distance vector calculation demonstrating tidal lock displacement from initial coordinates $(x_a, y_a)$ to present orbital coordinates $(x_b, y_b)$:
  $$\Delta d = \sqrt{(x_b - x_a)^2 + (y_b - y_a)^2}$$
* Visual tidal lock orientation keeping one hemisphere locked toward the host star.

### 7. Ancient Clepsammia (Sand Hourglass)
* Granular gravity-flow simulation calibrated to a 1-hour cycle ($3,600\text{ seconds}$).
* Visual particle stream and dynamic reservoir accumulation displaying both active hour percentage and completed hour cycles for the current day.

### 8. Ancient Clepsydra (Water Clock)
* Hydraulic outflow engine modeling uniform droplet drainage and lower chamber fill rate over a 1-hour window ($3,600\text{ seconds}$).
* Digital readouts for active basin capacity percentage and total elapsed reservoirs.

### 9. Top-View Solar Sundial
* Authentic horizontal dial plate featuring calibrated Roman numerals ($\text{VI AM}$ to $\text{VI PM}$).
* Fixed triangular gnomon style fin aligned permanently on the North-South ($\text{XII}$) meridian.
* Physically accurate broad cast shadow polygon projecting from the entire gnomon style crest to the dial rim based on real solar elevation and hour angles.
* Automatic transition to night phase when the Sun descends below the horizon.

---

## Technical Architecture

* **Unified Master Clock Loop:** Driven by `requestAnimationFrame` and `performance.now()`, ensuring all sub-engines remain phase-locked to standard system time and selected IANA time zones.
* **Delta-Time Normalization:** Eliminates hardware discrepancies between desktop monitors and battery-throttled mobile screens.
* **Responsive Layout:** Tailwind CSS grid supporting matrix overview and individual single-engine focus modes.
* **PWA & Offline Capable:** Includes manifest configuration and cache control setup for offline operation.

---
