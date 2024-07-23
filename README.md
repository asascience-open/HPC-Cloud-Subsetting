# HPC-Cloud-Subsetting
Project tracking repository for the NOAA HPC Subsetting Model Data in the Cloud project

## Targets for End of Project
- [ ] `xarray_subset_grid` repository is fully functional for ROMS and FVCOM datasets, contains examples and tests that prove the subsettings method is accurate.
- [X] `xreds` subset API is capable of delivering subsets 500 MB and below as `netCDF`, and any size as zarr. 

## Roadmap
### Ingest
- [x] Ingest NFOGS2
   * Add `mesh_topology` to the zarr datasets so they can be loaded consistently with ugrid and cf
- [x] Ingest WCOFS

### Software Development
- [x] Create example subsetting notebooks for FVCOM and ROMS using NODD data with Xarray
    * [FVCOM](https://github.com/mpiannucci/ocean-notebooks/blob/main/ngofs2_best_subset.ipynb)
    * [ROMS](https://github.com/mpiannucci/ocean-notebooks/blob/main/wcofs_best_subset.ipynb)
- [x] Create python package for subsetting model data with their native grids using Xarray
    * https://github.com/asascience-open/xarray-subset-grid
- [x] Create Xpublish plugin API to subset datasets on demand in the cloud
- [x] Create custom Xpublish based service including all required API plugins (including the subsetting plugin)
- [x] Create simple GUI for creating spatiotemporal subsets using the service
- [x] Deploy demo functionality with existing XREDS service
    * https://nextgen-dev.ioos.us/xreds/subset_export
- [x] Create example workflow scripts and notebooks utilizing the service
- [ ] Create API for reusing slicing logic
- [ ] Create test and validation suites for python package
- [ ] Benchmark subetting performance using test and validation cases
- [ ] Create full package documentation using python best practices
- [x] Add CI-CD
- [ ] Vertical Subset API
    - [x] Subset Level and Levels
    - [ ] Top Vertical Accessor
    - [ ] Bottom Vertical Accessor
    - [ ] Surface Vertical Accessor
- [ ] Add python package deployment integration with github with deployment to pypi
- [x] Optimize performance in subsetting package
    * Dataset subsetting methodology and algorithm performance
- [ ] Expand to other grid types
    - [x] ADCIRC
    - [ ] SELFE (Untested, but should work, CREOFS)
    - [X] SCHISM
    - [ ] HYCOM (RTOFS)
    - [X] Regular Grid (Test with GFS NOMADS OpenDAP)
    - [X] 2D Grid (Test with NAM Conus OpenDAP)
