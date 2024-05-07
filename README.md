# HPC-Cloud-Subsetting
Project tracking repository for the NOAA HPC Subsetting Model Data in the Cloud project


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
- [ ] Create example workflow scripts and notebooks utilizing the service
- [ ] Create test and validation suites for python package
- [ ] Expand to other grid types
    * ADCIRC
    * HYCOM
    * Regular Grid
    * 2D Grid

### Software Infrastructure
- [ ] Dockerize the Xpublish service
- [ ] Create IaaC with Pulumi for reproducible deployment in the cloud
- [ ] Add Dask and Redis capabilities to deployment for faster processing and cacheing
- [ ] Deploy example service in the cloud
- [ ] Benchmarking and performance tuning
