# Control Systems (ME5659) Project

## Project Title
MPC, LQR, Robust Controller via µ-Synthesis for Quadcopters

## Team Members
- Arun Srinivasan V K
- Ashwin Vaidya
- Sujai
- Praanesh

## Table of Contents
1. [Introduction](#introduction)
    - [Quadcopter](#quadcopter)
    - [How it Works](#how-it-works)
    - [Difference from a Drone](#difference-from-a-drone)
2. [Importance of Controller in Quadcopters](#importance-of-controller-in-quadcopters)
3. [Discussion](#discussion)
    - [Problem Statement](#problem-statement)
    - [Scope of the Project](#scope-of-the-project)
    - [Existing Solutions](#existing-solutions)
    - [Our Contribution](#our-contribution)
4. [Challenges](#challenges)
5. [Controllers Used](#controllers-used)
    - [MPC Controller](#mpc-controller)
    - [LQR Controller](#lqr-controller)
    - [Robust Controller via µ-Synthesis](#robust-controller-via-µ-synthesis)
6. [Use and Implementation](#use-and-implementation)
    - [MPC Controller](#use-and-implementation-of-mpc-controller)
    - [LQR Controller](#use-and-implementation-of-lqr-controller)
    - [Robust Controller via µ-Synthesis](#use-and-implementation-of-robust-controller-via-µ-synthesis)
7. [Analysis](#analysis)
    - [LQR Controller Analysis](#lqr-controller-analysis)
    - [Robust Controller Analysis](#robust-controller-analysis)
    - [MPC Controller Analysis](#mpc-controller-analysis)
8. [Future Aspects](#future-aspects)

## Introduction

### Quadcopter
A quadcopter is a rotary-wing aircraft equipped with four rotors, commonly used for aerial photography, surveillance, search and rescue, agriculture, and military operations. The simplicity in the flight control system due to its compact size and minimal mass makes it highly feasible for various applications.

### How it Works
A quadcopter operates with four rotors in a square configuration, with two rotating clockwise and the other two counterclockwise. The flight control is managed by adjusting the rotor speeds, enabling it to maneuver in multiple directions by modulating lift and torque.

### Difference from a Drone
While all quadcopters are drones, not all drones are quadcopters. Drones can be any unmanned vehicle operating on air, water, or land, whereas quadcopters specifically utilize four rotors for flight.

## Importance of Controller in Quadcopters
Controllers are critical in stabilizing and managing the quadcopter's motion. They utilize sensor data to regulate rotor speeds, ensuring stability and precision in movements.

## Discussion

### Problem Statement
Designing controllers for quadcopters involves addressing complex problems to manage the aircraft's 6 degrees of freedom, model the multivariate system accurately, and handle operational complexities in a 3D environment with disturbances.

### Scope of the Project
This project covers:
- LQR Controller: Balancing performance and energy consumption.
- Robust Controller: Maintaining stability and performance over bounded uncertainties.
- MPC: Following predefined trajectories or paths.

### Existing Solutions
Common solutions include PID controllers, altitude hold controllers, Kalman filters, optimal control techniques like MPC and LQR, and dedicated flight controllers.

### Our Contribution
We focused on understanding and implementing MPC, Robust Controller via µ-Synthesis, and LQR controllers by translating mathematical models into MATLAB code and Simulink models.

## Challenges
Key challenges included understanding the mathematical components, tuning controllers, designing Simulink models, and implementing algorithms.

## Controllers Used

### MPC Controller
Model Predictive Control (MPC) uses a system model to forecast future behavior and manage multiple inputs and outputs effectively. It enhances stability and precision, particularly in constrained environments.

### LQR Controller
The Linear Quadratic Regulator (LQR) optimizes a cost function to balance performance and energy consumption. It is robust with assured gain and phase margin and helps solve the LQG problem.

### Robust Controller via µ-Synthesis
This technique designs controllers to handle uncertainties by minimizing robust H∞ performance. It ensures stability and performance despite disturbances.

## Use and Implementation

### Use and Implementation of MPC Controller
MPC controllers enhance quadcopter stability and precision by using sensor data to regulate rotor speeds and follow predefined paths.

### Use and Implementation of LQR Controller
LQR controllers ensure stable and efficient flight by dynamically adjusting rotor speeds based on sensor inputs to maintain correct altitude and tilt.

### Use and Implementation of Robust Controller via µ-Synthesis
This controller addresses uncertainties and disturbances using the µ synthesis algorithm, ensuring reliable and accurate flight.

## Analysis

### LQR Controller Analysis
The LQR controller balances between performance and energy consumption. Higher performance cost leads to better path tracking but higher energy use, while higher control cost results in less energy consumption but poorer path tracking.

### Robust Controller Analysis
The µ-synthesis controller stabilizes the quadcopter under bounded disturbances, with robust stability and performance demonstrated through Monte Carlo simulations.

### MPC Controller Analysis
MPC is designed for trajectory tracking, utilizing a prediction model to manage multiple states and sensor inputs, ensuring stable and precise flight.

## Future Aspects
Future work includes improving control algorithms, integrating advanced sensor technologies, and exploring new applications in diverse fields such as autonomous navigation and artificial vision.

---


