============
CESM2-CMIP5
============

This repository contains the model code and case setups for the CESM2-CMIP5 Forcing Experiment


Obtaining the model code to run the CESM2-CMIP5 experiments
===========================================================

To obtain the CESM code you need to do the following:

#. Clone the repository. ::

      git clone -b cesm2.1.3_cmip5.n03_release-clm5.0.30 https://github.com/NCAR/CESM2-CMIP5.git my_cesm_sandbox
      
   This will create a directory ``my_cesm_sandbox`` in your current working directory.

#. Go into the created directory and check out the externals . ::

      cd my_cesm_sandbox
      ./manage_externals/checkout_externals 

