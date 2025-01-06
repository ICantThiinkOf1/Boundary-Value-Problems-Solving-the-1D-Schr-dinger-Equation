# **Boundary Value Problems: Solving the 1D Schrödinger Equation**

This repository contains a Python-based exploration of boundary value problems applied to the **one-dimensional, time-independent Schrödinger equation**. The tasks focus on solving and analyzing quantum systems under various potential functions.

---

## **Schrödinger Equation**
The time-independent Schrödinger equation is given as:  
(ħ² / 2m) * (d²ψ / dx²) + V(x)ψ(x) = Eψ(x)

Where:  
- **\( V(x) \)**: Potential of the electron  
- **\( \psi(x) \)**: Wavefunction  
- **\( m \)**: Mass of the electron  
- **\( x \)**: Position  
- **\( \hbar \)**: Reduced Planck's constant  

---

## **Tasks Overview**

### **Task 1: A Quantum Dot in the Vacuum (Infinite Square Well)**
1. **Finding the Ground State Energy**  
   - The potential \( V(x) \) for a square well of width \( 2a \) with infinitely high walls is:  
     \[
     V(x) = 
     \begin{cases} 
     0 & -a \leq x \leq +a \\ 
     \infty & |x| > a 
     \end{cases}
     \]  
   - **Boundary conditions**: \( \psi(-a) = \psi(+a) = 0 \).  

2. **Finding the Ground State Wavefunction**  
   - Plots the ground state wavefunction with boundaries denoted by vertical lines.  

3. **Finding Higher Energy States**  
   - Calculates and plots the first few excited states (\( n = 2, 3, 4 \)).  
   - Includes methods for generating initial guesses for arbitrary potentials.  

4. **Extension to 3D**  
   - Analyzes the **3D extension** with the energy states expressed as:  
     \[
     E_{n_x, n_y, n_z} = \frac{(n_x^2 + n_y^2 + n_z^2)\pi^2\hbar^2}{2md^2}
     \]  
   - Where \( n_x, n_y, n_z \) are quantum numbers.  

---

### **Task 2: The Infinite "Unsquare" Well**
1. **Harmonic Potential**  
   - Embeds a harmonic potential:  
     \[
     V(x) = V_0\frac{x^2}{a^2}
     \]  
   - Includes computation for eigenstates and wavefunctions with \( V_0 = 700e \).  

2. **Finite Square Well**  
   - Embeds a finite square well potential:  
     \[
     V(x) = 
     \begin{cases} 
     0 & -a/2 \leq x \leq +a/2 \\ 
     V_0 & |x| > a/2 
     \end{cases}
     \]  
   - Uses \( V_0 = 600e \) to calculate the lowest three eigenstates and their wavefunctions.  

---

## **Features**
- Numerical solutions to the Schrödinger equation using Python.  
- Visualization of wavefunctions and energy states for various potentials.  
- Extension to 3D quantum systems.  
- Flexible functions for analyzing arbitrary potential wells.  

