============
CESM2-CMIP5
============

This repository contains the model code and case setups for the CESM2-CMIP5 Forcing Experiment


Model code to run the CESM2-CMIP5 experiments
=============================================

To obtain the CESM code you need to do the following:

#. Clone the repository. ::

      git clone https://github.com/NCAR/CESM2-CMIP5 --branch cesm2-cmip5-tag  cesm2-cmip5-tag 
      
   This will create a directory ``cesm2-cmip5-tag`` in your current working directory.

#. Go into the created directory and check out the externals . ::

      cd cesm2-cmip5-tag
      ./manage_externals/checkout_externals 


Case directories of the CESM2-CMIP5 experiments
===============================================

The case directories of the CESM2-CMIP5 experiments are available at: 
    
      `https://github.com/NCAR/CESM2-CMIP5/tags`

To obtain a specific case directory (for instance: b.e21.B1850.f09_g17.cesm2-cmip5.001), you need to do the following ::

      git clone https://github.com/NCAR/CESM2-CMIP5 \
      --branch b.e21.B1850.f09_g17.cesm2-cmip5.001  b.e21.B1850.f09_g17.cesm2-cmip5.001


Comparing namelists for CESM1, CESM2 and CESM2-CMIP5 experiments
================================================================

To obtain the namelists of the CESM1, CESM2 and CESM2-CMIP5 experiments, you need to do the following ::

      git clone https://github.com/cecilehannay/CESM2-CMIP5  --branch namelists  namelists

