Surge Tank Lab
A single-file, browser-based teaching simulator for a solvent surge/buffer tank.
Model used
- Dynamic balance: A * dh/dt = Fin - Fout
- Fixed gravity outlet: Fout = Cv * sqrt(h)
- Open-loop inlet: Fin = nominal inlet + pump surge
- PI feedback: the PI controller adjusts the inlet pump flow; the outlet valve remains fixed.
- Bottom gauge pressure: P = rho * g * h
The simulation uses fourth-order Runge–Kutta integration with a 0.02-minute time step. A simple pump-flow limit and anti-windup behavior are included in PI mode.
Important assumptions
This is an ideal educational model. It assumes a vertical tank with constant cross-sectional area, incompressible liquid, constant density during a run, a fixed Torricelli-type outlet coefficient at a specified valve opening, and atmospheric pressure downstream of the outlet. It is not a detailed mechanical design or a substitute for plant-specific control design.
