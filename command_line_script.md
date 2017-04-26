---
title: Writing a command-line simulation script (advanced)
category: demonstration
position: 1
---

At some point after figuring out how to set up your reaction-diffusion system, you might want to run a lot of instances of a simulation and then gather the results. Examples might be:
- Determine the average value of an observable
- Get an observed value as a function of input parameters, e.g. run every simulation with another diffusion constant for a certain particle type

While you can do this within one python script or notebook, this tutorial will demonstrate to write a proper __command-line__ script with your custom arguments. This comes in handy when each of the above mentioned simulations runs as a single job on a node of a compute-cluster. The goal is to have a runnable script which can be called like

```bash
$ ./run_simulation.py --diffusion 0.42 --number-time-steps 1000
```
The above starts a simulation with 1000 time-steps where particles have a diffusion constant of 0.42.

# Separate system configuration
When writing a simulation script, it will be convenient to separate the configuration of your system, that is, particle-species, potentials, reactions, system-size and initial positions of particles.

# Parse input arguments

# Where data will be written
