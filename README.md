RAT (is an Analysis Tool), Public Edition
-----------------------------------------
RAT is a simulation and analysis package built with GEANT4, ROOT, and C++,
originally developed by S. Seibert for the Braidwood Collaboration. Versions
of RAT are now being used and developed by several particle physics
experiments.

RAT combines simulation and analysis into a single framework, which allows
analysis code to trivially access the same detector geometry and physics
parameters used in the detailed simulation.

RAT follows the "AMARA" principle: As Microphysical as Reasonably Achievable.
Each and every photon is tracked through an arbitrarily detailed detector
geometry, using standard GEANT4 or custom physics processes. PMTs are fully
modeled, and detected photons may be propagated to a simulation of front-end
electronics and DAQ.

This generic version is intended as a starting point for collaborations
looking for an easy-to-learn, extensible detector simulation and analysis
package that works out of the box. Once acquainted with RAT, it is easy to
customize the geometry elements, physics details, data structure, analysis
tools, etc., to suit your experiment's needs.


Usage Instructions (added by Deepak Samuel):
--------------------------------------------
- Required: ROOT 5.34 (with python, minuit and gsl_shared options enabled) & Geant4.10.01
- Make sure that thisroot.sh and geant4.sh are executed or paths to ROOT and Geant4 
are set correctly prior to running "rat".
- Install Scons in Ubuntu: sudo apt-get install scons
- After cloning this repository: cd rat-pac and do './configure' followed by 'env.sh'
- Now run 'scons'
- Once installation is completed, run 'rat'
