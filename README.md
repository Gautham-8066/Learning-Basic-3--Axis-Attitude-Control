# 3-Axis Spacecraft Attitude Controller

A Python-based simulator that uses a **PID (Proportional-Integral-Derivative)** control loop to stabilize a rigid-body spacecraft in 3D space.

## Project Overview
This project simulates the rotational dynamics of a spacecraft and implements a feedback control system to bring the vehicle from an initial "error" state (offset orientation) to a target "nadir-pointing" state (0, 0, 0 degrees).

### Features
* **Physics Engine:** Models rigid body dynamics using Euler integration.
* **PID Control:** Separate gains for Roll, Pitch, and Yaw axes to handle varying moments of inertia.
* **Headless Visualization:** Automatically generates and saves flight telemetry graphs as PNG files.

## 📐 The Physics
The simulator solves the rotational version of Newton's Second Law:
$$\tau = I \alpha$$
Where:
- **$\tau$ (Torque)** is the control effort from the PID.
- **$I$ (Inertia)** represents the mass distribution of the craft.
- **$\alpha$ (Acceleration)** is the resulting change in rotational speed.

## Simulation


https://github.com/user-attachments/assets/28b1aa29-ecd6-4945-ab2e-095f3850a858
<img width="1000" height="600" alt="stabilization_results" src="https://github.com/user-attachments/assets/8b0c5654-abcc-4027-9a72-2f8470eb5e50" />




