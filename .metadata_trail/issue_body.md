### -> submitter ORCID (or name)

0000-0002-2207-6837

### -> slug

sandifordcraig-2023-subduction

### -> license

CC-BY-4.0

### -> alternative license URL

_No response_

### -> model category

model published in study, forward model

### -> model status

None

### -> associated publication DOI

https://doi.org/10.1093/gji/ggad230

### -> model creators

_No response_

### -> title

_No response_

### -> description

Tectonic plates are recycled into the mantle through subduction, where they bend and deform in various ways, such as brittle failure. This process creates deep sea trenches and results in characteristic earthquake patterns and gravity anomalies. In this study, we used a numerical model to investigate plate bending dynamics, complementing simpler approaches like flexural yield strength envelopes. We focused on the competition between bending stress and sources of net in-plane stress, such as slab pull, which influences the plate's neutral plane depth. It is difficult to reconcile the 'apparent' neutral plane depth with a net slab pull force greater than about 2 TN/m. Deviatoric compression in subducting plates more easily explains reverse earthquakes at depths of 20-50 km in the bending plate.

### -> abstract

_No response_

### -> scientific keywords

Dynamics of lithosphere, Lithospheric flexure, Subduction, Earthquakes

### -> funder

https://ror.org/05mmh0f86, DP150102887
https://ror.org/03wnrjx87, URF\R1\180088
https://ror.org/02b5d8509

### -> model embargo?

_No response_

### -> include model code ?

- [X] yes

### -> model code/inputs DOI

https://github.com/dansand/subduction_GJI2022

### -> model code/inputs notes

Model setup is provided by an ASPECT input file and a WorldBuilder file (https://github.com/GeodynamicWorldBuilder/WorldBuilder). Minor modifications to the ASPECT source code were implemented and are discussed in the associated publication as well as the `model_code_inputs/README.md` directory. 

### -> include model output data?

- [X] yes

### -> data creators

_No response_

### -> model output data DOI

_No response_

### -> model output data notes

Computations were done using the ASPECT code version 2.4.0. ASPECT output data from 2 simulations are included with this model. The reference model is the same model setup/data described in Sandiford and Craig, (2023). An alternative model is included in which the over-riding plate is welded to the left sidewall at the start of the simulation (whereas the initial temperature field in the reference model has a ridge). Note that both simulations develop a short-wavelength instability in the free surface of the over-riding plate, which begins approximately 3 Ma after the start of the simulation. The top level directories contains typical ASPECT output files, including log.txt and restart files. The primary output data consists of:

-  plain text files representing model topography (e.g. topography.00000)
- a range of "field" data, in .vtu format in the `./solution` sub-directory (e.g. solution-00000.0000.vtu). At each output step, there are 48 vtu files written. These can be opened with Paraview using the solution.pvd file in the top level. Quantities generally have SI units. Velocities are output as meters/year. 
-  particle information stored as .vtu files (16 per timestep). Particles were used to track the 2-km-thick weak entrained layer that facilitates the plate interface decoupling zone.  

### -> model output data size

47 Gb

### -> software framework DOI/URI

https://doi.org/10.5281/zenodo.6903424

### -> software framework source repository

https://github.com/geodynamics/aspect

### -> name of primary software framework (e.g. Underworld, ASPECT, Badlands, OpenFOAM)

_No response_

### -> software framework authors

https://orcid.org/0000-0003-2311-9402
https://orcid.org/0000-0003-0357-7115
https://orcid.org/0000-0003-0035-7723
https://orcid.org/0000-0001-7098-8198
https://orcid.org/0000-0002-9481-1749
https://orcid.org/0000-0002-8137-3903
https://orcid.org/0000-0001-9489-5236
https://orcid.org/0000-0002-5697-7203


### -> software & algorithm keywords

C++, finite-element, adaptive-mesh-refinement, particles

### -> computer URI/DOI

https://dx.doi.org/10.25914/608bfd1838db2

### -> add landing page image and caption

![res_fig_final_ann](https://github.com/ModelAtlasofTheEarth/model_submission/assets/10967872/dfdd5e1a-2f8a-4a0a-b289-6b6b33dbf033)
Downdip component of strain rate tensor and resolved stress difference from the numerical model, focusing on features within the plate/slab. The resolved stress difference is defined as ($\sigma_{s} - \sigma_{z}$), where $\hat{s}$, and $\hat{z}$ are unit vectors in the downdip and slab normal directions. The fields show, for example, shortening/extension in the downdip direction. Stress profiles at four locations are shown. The blue line ($x_0$) is the first zero crossing based on analysis of the flexural component of the topography. The black line is the location of maximum bending moment.


### -> add an animation (if relevant)

https://github.com/ModelAtlasofTheEarth/model_submission/assets/10967872/f9e647c5-3341-400c-bac3-d5546f1d7226
Animation shows the model domain at 2x vertical exaggeration. The scalar field is the effective strain rate, i.e. $\dot\epsilon_{II} =  \sqrt{J2} = \sqrt{0.5(\dot\epsilon_{i,j}: \epsilon_{i,j})}$. Upper panel shows the evolution of the model topography (a true free surface). The topographic profile reveals the long-wavelength isostatic thermal subsidence, as well as the flexural topography associated with the subduction zone. The model exhibits a very short-wavelength instability in the free surface of the over-riding plate, which begins approximately 3 Ma after the start of the simulation. 


### -> add a graphic abstract figure (if relevant)

![gpe_fm26](https://github.com/ModelAtlasofTheEarth/model_submission/assets/10967872/59192612-c943-40d0-8c6c-e129457d833f)
The main panel shows the variation in terms that arise in a 2D "vertically integrated" form of the force balance (or stress equilibrium) equations. Assuming a traction-free surface, the force balance states that across a horizontal section of the lithosphere, the following terms must sum to zero: 1) integrated basal shear traction, 2) the difference in the vertically-integrated deviatoric stress and 3), the difference in the vertically-integrated vertical normal stress (often called the GPE). In the figure, the overbar symbols represent vertical integration across the lithosphere. Specifically, integration from a reference height, (taken here as the mean ridge height) down to a reference depth (taken here as 150 km beneath the reference height). In the main panel, the black line shows the horizontal variation in the vertically integrated deviatoric stress difference ($\tau_{xx} - \tau_{zz}$).  Positive values indicate a state of deviatoric tension. The dashed blue line shows the horizontal variation in the vertically integrated vertical normal stress ($\sigma_{yy}$)  (or the GPE). Strictly speaking, this quantity is only equal to the GPE when the vertical normal stress is lithostatic, but the term is retained in this study due to convention. The upper panel shows the subducting plate topography at 2 different scales.  

### -> add a model setup figure (if relevant)

![s1a](https://github.com/ModelAtlasofTheEarth/model_submission/assets/10967872/0ac0b429-cd65-4aff-afad-39c5e7c1a980)
The main panel shows the full model domain and initial temperature field. The texture is generated with a line integral convolution of the velocity field. Contours show evolution of the slab during the 10 Myr simulation. Velocity arrows show convergence rates at 5 Myr into the simulation. Inset panels show details of the adaptive mesh refinement during the simulation. 

### -> add a description of your model setup

The subduction model comprises a rectangular domain with a depth of 2900 km, and an aspect ratio of 4. The initial conditions comprise an adiabatic mantle with a potential temperature of 1350 C and two plates, whose age and thermal structure follows the cooling 1d cooling profile for a half-space (infinite in the depth direction). One of these plates is attached to a slab that extends to 660 km depth, and has an age of 100 Myr at the trench. The upper plate is modelled with a younger thermal age, 25 Myr at the trench. Imposing an initial slab that reaches the transition zone was found to be a more stable initial configuration in terms of instabilities of the free surface. 7 levels of mesh refinement were used, with the largest (Q2) elements having an edge length of 45 km, and the smallest elements have an edge length of ∼ 700 m. The interface is modelled through an entrained weak layer approach. A thin layer (here 2 km thick) represented by a separate composition is imposed on the top of the subducting plate, as well as between the subducting slab and upper plate. This composition has a low coefficient of friction, providing a shear stress that varies between between about 10 - 20 MPa throughout the plate interface domain. See the included model input file (.prm) for further details. 

### Please provide any feedback on the model submission process?

_No response_