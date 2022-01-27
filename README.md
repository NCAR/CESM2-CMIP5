# Case directories for the CESM2-CMIP5 forcing 

## b.e21.B1850.f09_g17.cesm2-cmip5.001

The pi_control b.e21.B1850.f09_g17.cesm2-cmip5.001 starts as an hybrid run from:

- RUN_REFCASE=b.e21.B1850.f09_g17.CMIP6-piControl.001
- RUN_REFDATE=0501-01-01

This directory contains all the information to reproduce b.e21.B1850.f09_g17.cesm2-cmip5.001 including:

- namelist changes
- SourceMods

## b.e21.BHIST.f09_g17.cesm2-cmip5.001

The b.e21.B1850.f09_g17.cesm2-cmip5.001 starts as an hybrid run from the pi-control at year 250:

- RUN_REFCASE=b.e21.B1850.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=0250-01-01

This directory contains all the information to reproduce b.e21.BHIST.f09_g17.cesm2-cmip5.001 including:

- namelist changes
- SourceMods

Due to computational constraints, only a single historical ensemble member b.e21.BHIST.f09_g17.cesm2-cmip5.001 runs from 1850-2005,

the remaining members b.e21.BHIST.f09_g17.cesm2-cmip5.002, ... b.e21.BHIST.f09_g17.cesm2-cmip5.010 were started at 1920 from the first member with a pertlim perturbation.


## b.e21.RCP85.f09_g17.cesm2-cmip5.001

The b.e21.BRCP85.f09_g17.cesm2-cmip5.001 starts as an hybrid run from the historical run b.e21.BHIST.f09_g17.cesm2-cmip5.001 at year 2006:

- RUN_REFCASE=b.e21.BHIST.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=2006-01-01

This directory contains all the information to reproduce b.e21.BRCP85.f09_g17.cesm2-cmip5.001 including:

- namelist changes
- SourceMods

Similarly, ensemble 2-10 starts from:

- b.e21.BHIST.f09_g17.cesm2-cmip5.002 => b.e21.BRCP85.f09_g17.cesm2-cmip5.002
- ...
- b.e21.BHIST.f09_g17.cesm2-cmip5.010 => b.e21.BRCP85.f09_g17.cesm2-cmip5.010


## b.e21.RCP85.f09_g17.cesm2-cmip5.101

The b.e21.BRCP85.f09_g17.cesm2-cmip5.101 starts as an hybrid run from the historical run b.e21.BHIST.f09_g17.cesm2-cmip5.001 at year 2006:
- RUN_REFCASE=b.e21.BHIST.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=2006-01-01

This run is similar to b.e21.BRCP85.f09_g17.cesm2-cmip5.001 but includes a bugfix for the _a2 emissions aerosol emissions. The influence of the incorrect _a2 emissions on climate properties was found to be minimal.

This directory contains all the information to reproduce b.e21.BRCP85.f09_g17.cesm2-cmip5.101 including:
- namelist changes
- SourceMods
