# z2_matter_qc/simulation_main

The Jupyter notebook `Z2_Simulation_Main.ipynb` runs the latest version of our computation on an IBMQ provider backend (can be simulator or real machine).
Eventually, this notebook should be ported to a Python script that will be run through the command line,
in which case the `bash/zsh` script that automatically submits multiple jobs (to be written) will also live here. 

The program `Z2_Simulation_Main.ipynb` 
- gets simulation inputs from `yaml` files in the `./inputs` folder,
- uses functions defined in the Python scripts in the `./modules` folder, and 
- saves the input, and output `json` files to the `./json` folder. 

The Jupyter notebook `State_Prep_Tests.ipynb` time evolves all gauge-invariant vacuum and meson (= fermion + antifermion) states for 2- and 4-site lattices using the same Trotterization code as in `Z2_Simulation_Main.ipynb`.
