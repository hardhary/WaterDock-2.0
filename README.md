# WaterDock2.0
# This is an updated to Python3 version of WaterDock2.0 (conversion by Phil Biggin) https://github.com/bigginlab/
# If you still need the  python2 version, you should visit:  https://github.com/akshay-sridhar/WaterDock2.0

Original Python2 version of WaterDock2.0 written by Akshay Sridhar (https://doi.org/10.1371/journal.pone.0172743)
based on the original WaterDock method developed by Greg Ross (https://doi.org/10.1371/journal.pone.0032036) 
Comments and queuries should be address to philip.biggin@bioch.ox.ac.uk 

This is a Command line interface of WaterDock2.0 now updated to work with python 

To run

python waterdock2.py proteinfile.pdbqt ligandfile.pdb

This will output a single file called "predictedwaters.pdb", which contains the predictions of the oxygen positions.


Dependencies

-- MDAnalysis (version >= 0.13)

-- numpy (any version compatible with your MDAnalysis build)

-- scipy (version does not matter)


FILE FORMATS

Protein File -- *pdbqt*

Ligand File -- *pdb/mol2*

Examples/Tests

An example protein (example-protein.pdbqt) and an example ligand are provide (example-ligand.pdb)

python waterdock2.py example-protein.pdbqt example-ligand.pdb 

will generate predictedwaters.pdb which should contain 3 predicted water molecule locations.

You can check the result of the prediction in pymol

