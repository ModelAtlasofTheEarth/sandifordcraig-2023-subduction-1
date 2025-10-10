# Model Output Data

**Note Output Data will often be too large to host on Github.** 

To access output data for this model, check the M@TE collection on NCI (http://dx.doi.org/10.25914/yrzp-g882), or refer to this model on the M@TE website (http://mate.science)


## Notes:
Computations were done using the ASPECT code version 2.4.0. ASPECT output data from 2 simulations are included with this model. The reference model is the same model setup/data described in Sandiford and Craig, (2023). An alternative model is included in which the over-riding plate is welded to the left sidewall at the start of the simulation (whereas the initial temperature field in the reference model has a ridge). Note that both simulations develop a short-wavelength instability in the free surface of the over-riding plate, which begins approximately 3 Ma after the start of the simulation. The top level directories contains typical ASPECT output files, including log.txt and restart files. The primary output data consists of:

-  plain text files representing model topography (e.g. topography.00000)
- a range of "field" data, in .vtu format in the `./solution` sub-directory (e.g. solution-00000.0000.vtu). At each output step, there are 48 vtu files written. These can be opened with Paraview using the solution.pvd file in the top level. Quantities generally have SI units. Velocities are output as meters/year. 
-  particle information stored as .vtu files (16 per timestep). Particles were used to track the 2-km-thick weak entrained layer that facilitates the plate interface decoupling zone.