# 2D Spring-Pendulum
A numerical simulation of a 2D spring-pendulum system derived using Lagrangian mechanics and implemented in Python using an object-oriented design.

This project models the coupled radial and angular motion of a mass attached to a spring and numerically integrates the resulting nonlinear equations of motion.


## Features
- Derived the equations of motion using the Euler-Lagrange equations
- Modeled the coupled radial and angular dynamics
- Implemented the simulation using object-oriented programming (OOP)
- Numerically solved the equations of motion using SciPy
- Generated the spring pendulum animation using Matplotlib
- Used NumPy for numerical calculations

## Physics

The system is described using polar coordinates, with generalized coordinates:
- $r$ — radial distance from the pivot
- $\theta$ — angular displacement

The Lagrangian is defined as: 

$$
L = T - V
$$

Where the kinetic and potential energies include the motion of the pendulum mass, gravitational potential energy, and the potential energy of the spring.

Applying the Euler-Lagrange equations,

$$
\frac{\partial L}{\partial q_i}
=0,
$$

produces the coupled nonlinear equations of motion for $r(t)$ and $\theta(t)$. These equations are then converted into a system of first-order ordinary differential equations and numerically integrated using SciPy.

## Numerical Methods
The simulation uses numerical ODE integration to calculate the system's position and velocity as functions of time.

The numerical solver computes:
- Radial position and velocity
- Angular position and velocity
- Cartesian position of the mass
- Time evolution of the system

## Object-Oriented Design

The simulation is organized using Python classes to separate the physical model, numerical integration, and visualization components.

This structure makes it easier to modify parameters such as:
- Spring constant
- Mass
- Gravitational acceleration
- Initial radial displacement
- Initial angular velocity
- Simulation duration

## Visualization

The simulation produces an animated representation of the spring-pendulum motion.
![](https://github.com/JBaez-10/Spring-Pendulum/blob/main/Spring_Pendulum.gif)

## Libraries
 - Matplotlib — visualization
 - Numpy — numerical calculations
 - SciPy — numerical integration of the equations of motion

## How to Run

Clone the repository:

git clone https://github.com/JBaez-10/Spring-Pendulum.git
cd Spring-Pendulum

Install the required libraries:

pip install numpy scipy matplotlib

Run the simulation:

python spring_pendulum.py

## Skills Demonstrated

### Physics & Mathematics
- Lagrangian mechanics
- Euler-Lagrange equations
- Nonlinear dynamical systems
- Ordinary differential equations
- Numerical methods

### Programming
- Python
- Object-oriented programming
- NumPy
- SciPy
- Matplotlib
- Numerical simulation
- Data visualization
