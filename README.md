# Case directory for the CESM2-CMIP5 forcing historical runs

This is the case directory for **b.e21.BHIST.f09_g17.cesm2-cmip5.001**

The b.e21.B1850.f09_g17.cesm2-cmip5.001 starts as an hybrid run from the pi-control at year 250:
- RUN_REFCASE=b.e21.B1850.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=0250-01-01

This directory contains all the information to reproduce b.e21.BHIST.f09_g17.cesm2-cmip5.001 including:
- namelist changes
- SourceMods

Due to computational constraints, 
- only a single historical ensemble member **b.e21.BHIST.f09_g17.cesm2-cmip5.001** runs from 1850-2005, 
- the remaining members **b.e21.BHIST.f09_g17.cesm2-cmip5.002**, ... **b.e21.BHIST.f09_g17.cesm2-cmip5.010** were started at 1920 from the first member with a pertlim perturbation.
