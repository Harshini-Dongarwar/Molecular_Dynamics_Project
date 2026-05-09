# Molecular_Dynamics_Project
Project: Build Your Own MD Simulation

 MODULE-1
 Learning Objectives
 
• Understand how atomic motion is driven by potential energy.

• Implement the Lennard-Jones (LJ) potential as a model for an inert system.

• Master the concept of Reduced (Dimensionless) Units.

MODULE-2

Learning Objectives

• Understand how to simulate a “bulk” material using a finite number of atoms.

• Implement Periodic Boundary Conditions (PBC) to eliminate surface effects.

• Apply the Minimum Image Convention to ensure consistent interatomic interactions.

• Generate a stable starting geometry using a Face-Centered Cubic (FCC) lattice.

MODULE-3

Learning Objectives

• Understand numerical integration as a “time machine” for atomic systems.

• Implement the Velocity Verlet algorithm to solve Newton’s equations of motion.

• Learn to diagnose code accuracy through Total Energy conservation.

MODULE-4

Learning Objectives

• Identify the computational bottleneck in MD simulations.

• Implement Verlet Neighbor Lists to reduce the scaling of force calculations from O(N**2) to O(N).

• Apply NumPy Vectorization to accelerate mathematical operations in Python.

MODULE-5

Learning Objectives

• Establish a physically valid starting state for the system.

• Apply Statistical Mechanics to initialize velocities from a Maxwell-Boltzmann distribution.

• Implement Velocity Rescaling to drive the system toward a target temperature.

• Assemble the “Main Loop” of an MD simulation following the master algorithm.

OBSERVATIONS:
<img width="1189" height="989" alt="image" src="https://github.com/user-attachments/assets/5d9dece4-5c33-4a7f-8106-ff2793960d23" />

 The instantaneous temperature fluctuated around the target value T ∗ =0.5, confirming correct velocity initialization and equilibration. The total energy remained approximately conserved during the production phase, demonstrating the stability and correctness of the Velocity Verlet integrator. The potential energy exhibited bounded thermal fluctuations without numerical divergence, indicating stable Lennard-Jones interactions and proper implementation of periodic boundary conditions and neighbor lists


MODULE-6

Learning Objectives

• Structural Analysis: Use the Radial Distribution Function g(r).
<img width="790" height="1189" alt="image" src="https://github.com/user-attachments/assets/24275ac9-78dc-493d-bf56-c7d91a794db5" />

CHECKING FOR ARGON:
<img width="790" height="1189" alt="image" src="https://github.com/user-attachments/assets/49f3b7ec-477c-44d7-b613-e1020f2fac08" />



OBSERVATION:
Here our nearest neighbour distance at T*=0.01(which we will consider as solid) is given as 1.12, which means a/root2=1.12

calculating **a** we get it as 1.414*1.12=1.58368  (this is in reduced units)

for argon sigma=3.40 A

so lattice parameter=1.58368*3.40=5.38 ( which approximately matches the experimental value)

The epsilon value for argon=0.0104, 
for T*=0.6
Treal=T*(epsilon/Kb)=0.6(120.69)=72.41 kelvin, this is the temperature where we notice even according to the graph that argon is transitioning into liquid state.

We notice that as the temp rises, the peaks broaden and Argon shifts into liquid state.


