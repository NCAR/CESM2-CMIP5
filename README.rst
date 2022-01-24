============
CESM2-CMIP5
============

This repository contains the model code and case setups for the CESM2-CMIP5 Forcing Experiment


Obtaining the model code to run the CESM2-CMIP5 experiments
===========================================================

To obtain the CESM code you need to do the following:

#. Clone the repository. ::

      git clone -b cesm2-cmip5-tag https://github.com/NCAR/CESM2-CMIP5.git my_cesm_sandbox 
      
   This will create a directory ``my_cesm_sandbox`` in your current working directory.

#. Go into the created directory and check out the externals . ::

      cd my_cesm_sandbox
      ./manage_externals/checkout_externals 


Case directories of the CESM2-CMIP5 experiments
===============================================

The case directories of the CESM2-CMIP5 experiments are available at: 
    
    https://github.com/NCAR/CESM2-CMIP5/tags

To obtain a specific case directory (for instance: b.e21.B1850.f09_g17.cesm2-cmip5.001), you need to do the following ::

      git clone --branch b.e21.B1850.f09_g17.cesm2-cmip5.001 https://github.com/NCAR/CESM2-CMIP5 b.e21.B1850.f09_g17.cesm2-cmip5.001
