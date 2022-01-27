=======================
CESM2-CMIP5 experiments
=======================

This repository contains the model code and case setups for the CESM2-CMIP5 Forcing Experiment. It also contains the namelists for the CESM1, CESM2 and CESM2-CMIP5 experiments to allow a comparison between them. 

.. contents::

Comparing namelists for CESM1, CESM2 and CESM2-CMIP5 experiments
================================================================

To obtain the namelists of the CESM1, CESM2 and CESM2-CMIP5 experiments, you need to do the following ::

      git clone https://github.com/NCAR/CESM2-CMIP5  --branch namelists  namelists
      
      
Model code to run the CESM2-CMIP5 experiments
=============================================

To obtain the CESM code you need to do the following:


1. Clone the repository ::

      git clone https://github.com/NCAR/CESM2-CMIP5 --branch cesm2-cmip5-tag  cesm2-cmip5-tag 
      
This will create a directory ``cesm2-cmip5-tag`` in your current working directory.

2. Go into the created directory and check out the externals  ::


      cd cesm2-cmip5-tag
      ./manage_externals/checkout_externals 
     
    
Case directories of the CESM2-CMIP5 experiments
===============================================

The case directories of the following CESM2-CMIP5 experiments are available ::

      b.e21.B1850.f09_g17.cesm2-cmip5.001: pi-control (500 years)
      b.e21.BHIST.f09_g17.cesm2-cmip5.001: historical (1850-2005)  
      b.e21.BRCP85.f09_g17.cesm2-cmip5.001: rcp85 (2006-2100)
      b.e21.BRCP85.f09_g17.cesm2-cmip5.101: rcp85 (2006-2100) with bugfix for num_a2

To obtain a specific case directory (for instance: b.e21.B1850.f09_g17.cesm2-cmip5.001), you need to do the following ::

      git clone https://github.com/NCAR/CESM2-CMIP5 \
      --branch b.e21.B1850.f09_g17.cesm2-cmip5.001  b.e21.B1850.f09_g17.cesm2-cmip5.001


More details about the setting of the B1850, BHIST and RCP85
==============================================

B1850
~~~~~

The pi_control ``b.e21.B1850.f09_g17.cesm2-cmip5.001`` starts as an hybrid run from:

- RUN_REFCASE=b.e21.B1850.f09_g17.CMIP6-piControl.001
- RUN_REFDATE=0501-01-01

The pi_control is 500 years.

BHIST
~~~~~

The ``b.e21.B1850.f09_g17.cesm2-cmip5.001`` starts as an hybrid run from the pi-control at year 250:

- RUN_REFCASE=b.e21.B1850.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=0250-01-01

Due to computational constraints, 

- only the first historical ensemble member b.e21.BHIST.f09_g17.cesm2-cmip5.001 runs from 1850-2005,
- the remaining members ``b.e21.BHIST.f09_g17.cesm2-cmip5.002``, ... ``b.e21.BHIST.f09_g17.cesm2-cmip5.010`` were started at 1920 from the first member with a ``pertlim`` perturbation.


RCP85
~~~~~

The ``b.e21.RCP85.f09_g17.cesm2-cmip5.001`` starts as an hybrid run from the historical run b.e21.BHIST.f09_g17.cesm2-cmip5.001 at year 2006:

- RUN_REFCASE=b.e21.BHIST.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=2006-01-01

Similarly, ensemble 2-10 starts from:

- ``b.e21.BHIST.f09_g17.cesm2-cmip5.002`` => ``b.e21.RCP85.f09_g17.cesm2-cmip5.002``
- ...
- ``b.e21.BHIST.f09_g17.cesm2-cmip5.010`` => ``b.e21.RCP85.f09_g17.cesm2-cmip5.010``


RCP85 + bugfix
~~~~~~~~~~~~~~

The ``b.e21.RCP85.f09_g17.cesm2-cmip5.101`` starts as an hybrid run from the historical run b.e21.BHIST.f09_g17.cesm2-cmip5.001 at year 2006:
- RUN_REFCASE=b.e21.BHIST.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=2006-01-01

This run is similar to b.e21.RCP85.f09_g17.cesm2-cmip5.001 but includes a bugfix for the ``_a2`` emissions aerosol emissions. The influence of the incorrect _a2 emissions on climate properties was found to be minimal.

