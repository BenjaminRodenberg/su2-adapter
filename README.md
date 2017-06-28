
preCICE-adapter for SU2 - "Stanford University Unstructured"
----------------------------------------------------
The adapter for the CFD-Code was developed in the scope of the [bachelor's thesis of Alexander Rusch](https://www5.in.tum.de/pub/Rusch2016_BA.pdf).
All steps for integrating the adapter into SU2 are described in detail in the appendices of the thesis.
The most important parts of these appendices can be found in this directory as excerpts (in PDF-format).
The adapter was tested with the SU2 version 4.3.0 "Cardinal".

1. Adapting solver routines of SU2:
-----------------------------------
In order to run SU2 with the preCICE adapter, some SU2 native solver routines need to be changed slightly.
The changes are explained in ChangeSU2SolverRoutines.pdf

2. Building SU2 with the adapter:
---------------------------------
For building SU2 with the coupling adapter, the adapter files precice.cpp and precice.hpp need to be included in SU2 and compiled with it, while the static preCICE-library needs to be linked in addition.
All necessary changes to the SU2 makefiles and building options are described in BuildingSU2WithPreCICE.pdf
