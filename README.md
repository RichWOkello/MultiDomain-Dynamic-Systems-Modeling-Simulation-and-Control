# Multi-Domain Dynamic Systems Modeling, Simulation and Control

A comprehensive Jupyter-based project for mathematical modeling, simulation, stability analysis, controller design, and multi-domain integration of **mechanical, electrical, pneumatic, and hydraulic systems**.

The project demonstrates how different physical systems can be described using differential equations, transfer functions, state-space models, numerical simulation, and modern control techniques.

---

## Project Objectives

The project aims to:

- derive mathematical models from physical laws;
- simulate dynamic system behavior;
- classify damping and stability automatically;
- analyze systems in the time and frequency domains;
- design classical and state-space controllers;
- investigate nonlinearities and uncertainty;
- introduce digital control concepts;
- model realistic pneumatic and hydraulic actuator behavior;
- integrate electrical, mechanical, pneumatic, and hydraulic subsystems into complete control loops.

---

## Repository Structure

```text
MultiDomain_Dynamic_Systems_Modeling_Simulation_and_Control/
│
├── 01_Mechanical_Systems_Modeling_Simulation_and_Control.ipynb
├── 02_Electrical_Systems_Modeling_Simulation_and_Control.ipynb
├── 03_Pneumatic_Systems_Modeling_Simulation_and_Control.ipynb
├── 04_Hydraulic_Systems_Modeling_Simulation_and_Control.ipynb
├── 05_MultiDomain_Dynamic_Systems_Modeling_Simulation_and_Control.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

---

## 1. Mechanical Systems

The mechanical notebook includes:

- mass-spring-damper modeling;
- rotational systems;
- gear reflected inertia;
- coupled multi-degree-of-freedom systems;
- natural-frequency and damping-ratio calculations;
- automatic underdamped, critically damped, overdamped, undamped, and unstable classification;
- transfer functions;
- state-space models;
- pole-zero analysis;
- step, impulse, and ramp responses;
- Routh-Hurwitz stability;
- root locus;
- Bode, Nyquist, and Nichols analysis;
- gain and phase margins;
- lead, lag, and lead-lag compensation;
- PID control;
- anti-windup;
- feedforward and cascade control;
- sensitivity analysis;
- controllability and observability;
- state feedback;
- Luenberger observers;
- LQR;
- Kalman filtering and LQG concepts;
- digital control and Jury stability;
- nonlinear friction, backlash, deadband, and saturation;
- phase-plane and Jacobian analysis.

---

## 2. Electrical Systems

The electrical notebook covers:

- RC, RL, and RLC systems;
- transient-response analysis;
- RLC damping and resonance;
- transfer-function and state-space representations;
- classical control analysis;
- PID and compensator design;
- DC motor modeling;
- electrical-mechanical coupling;
- state feedback and observers;
- LQR and Kalman filtering;
- transformer calculations;
- three-phase power;
- synchronous-generator swing dynamics;
- simplified induction-motor torque-slip behavior;
- buck converter;
- boost converter;
- PWM inverter concepts;
- discrete-time control;
- parameter uncertainty and robustness.

---

## 3. Pneumatic Systems

The pneumatic notebook includes both linearized and nonlinear actuator models.

Topics include:

- pneumatic-cylinder motion;
- pressure dynamics;
- compressible-air modeling;
- absolute chamber pressure;
- variable chamber volume;
- dead volume;
- choked and subsonic valve-flow approximations;
- valve spool dynamics;
- leakage;
- asymmetric piston areas;
- load forces;
- Coulomb-friction approximation;
- stroke limits;
- PID control with anti-windup;
- stability and modal damping;
- pole-zero and frequency-domain analysis;
- controllability and observability;
- state feedback and observers;
- LQR;
- digital control;
- Jacobian linearization;
- uncertainty analysis.

---

## 4. Hydraulic Systems

The hydraulic notebook includes:

- cylinder-force modeling;
- fluid compressibility;
- bulk modulus;
- pressure dynamics;
- nonlinear valve-orifice flow;
- asymmetric cylinder geometry;
- supply and return pressure;
- leakage;
- valve spool dynamics;
- relief-pressure approximation;
- cavitation warning logic;
- accumulator behavior;
- friction and stroke constraints;
- PID control with anti-windup;
- classical stability analysis;
- frequency-domain analysis;
- state feedback and observers;
- LQR;
- digital control;
- Jacobian analysis;
- parameter uncertainty.

---

## 5. Multi-Domain Dynamic Systems Modeling, Simulation and Control

The final notebook combines physical domains into integrated control systems.

Examples include:

### Electromechanical system

```text
Electrical Supply
      ↓
Controller
      ↓
DC Motor
      ↓
Mechanical Load
      ↓
Position / Speed Sensor
      ↓
Feedback
```

### Electro-pneumatic system

```text
Electrical Controller
      ↓
Solenoid / Servo Valve
      ↓
Compressed Air
      ↓
Pneumatic Cylinder
      ↓
Mechanical Load
      ↓
Position Feedback
```

### Electro-hydraulic system

```text
Electronic Controller
      ↓
Servo Valve
      ↓
Hydraulic Flow
      ↓
Cylinder Pressure
      ↓
Mechanical Motion
      ↓
Position Feedback
```

The notebook also includes interactive:

- plant parameters;
- controller gains;
- actuator dynamics;
- sensor dynamics;
- reference values;
- disturbances;
- measurement noise;
- saturation;
- cascade-loop gains;
- feedforward gain;
- stability parameters;
- simulation time;
- frequency-analysis ranges.

---

## Interactive Simulation

The project uses `ipywidgets` so system parameters can be adjusted directly from the notebook.

Changing slider values automatically updates:

- simulation results;
- transient-response plots;
- pressure or current plots;
- pole locations;
- stability classification;
- damping classification;
- frequency-response plots.

---

## Core Mathematical Workflow

The project follows the general engineering workflow:

```text
Physical System
      ↓
Governing Physical Laws
      ↓
Differential Equations
      ↓
Transfer Function / State Space
      ↓
Simulation
      ↓
Stability Analysis
      ↓
Controller Design
      ↓
Closed-Loop Evaluation
```

---

## Installation

Clone the repository:

```bash
git clone https://github.com/RichWOkello/MultiDomain_Dynamic_Systems_Modeling_Simulation_and_Control.git
```

Enter the repository:

```bash
cd MultiDomain_Dynamic_Systems_Modeling_Simulation_and_Control
```

Create a virtual environment:

```bash
python -m venv venv
```

Activate it on Windows:

```bash
venv\Scripts\activate
```

Activate it on Linux/macOS:

```bash
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Start JupyterLab:

```bash
jupyter lab
```

or:

```bash
jupyter notebook
```

Open any notebook and run the cells from top to bottom.

---

## Main Python Libraries

- NumPy
- SciPy
- Matplotlib
- ipywidgets
- python-control
- Jupyter

---

## MATLAB / Simulink Comparison

The project reproduces many capabilities commonly used in MATLAB Control System Toolbox, including:

- transfer-function analysis;
- state-space analysis;
- pole-zero analysis;
- root locus;
- Bode, Nyquist, and Nichols plots;
- stability margins;
- PID control;
- state feedback;
- observers;
- LQR;
- Kalman filtering;
- digital control;
- nonlinear simulation.

It does **not** attempt to reproduce the full graphical block-diagram and component-library functionality of Simulink or Simscape.

---

## Engineering Note

The nonlinear pneumatic and hydraulic models are educational lumped-parameter models intended for modeling and control-system study. They are not certified industrial component models and should not be used directly for safety-critical equipment design without appropriate validation.

---

## Future Extensions

Possible future improvements include:

- model predictive control;
- \(H_\infty\) robust control;
- adaptive control;
- system identification from experimental data;
- hardware-in-the-loop simulation;
- real sensor and actuator interfaces;
- PLC integration;
- graphical block-diagram simulation;
- real-time control deployment.

---

## Author

**Richard Okello**

Control and Instrumentation / Data Science

---

## License

This project is provided for educational and engineering-learning purposes.
