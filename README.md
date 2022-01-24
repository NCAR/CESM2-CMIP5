# Case directory for the CESM2-CMIP5 forcing RCP85 runs

This is the case directory for **b.e21.RCP85.f09_g17.cesm2-cmip5.101**

The b.e21.BRCP85.f09_g17.cesm2-cmip5.101 starts as an hybrid run from the historical run b.e21.BHIST.f09_g17.cesm2-cmip5.001 at year 2006:
- RUN_REFCASE=b.e21.BHIST.f09_g17.cesm2-cmip5.001
- RUN_REFDATE=2006-01-01

This run is similar to b.e21.BRCP85.f09_g17.cesm2-cmip5.001 but includes a bugfix for the _a2 emissions aerosol emissions. The influence of the incorrect _a2 emissions on climate properties was found to be minimal.

This directory contains all the information to reproduce b.e21.BRCP85.f09_g17.cesm2-cmip5.101 including:
- namelist changes
- SourceMods
