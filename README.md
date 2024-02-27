# HPC-Cloud-Subsetting
Project tracking repository for the NOAA HPC Subsetting Model Data in the Cloud project


## Roadmap
### Ingest
- [x] Ingest NFOGS2
- [x] Ingest WCOFS

### Software Development
- [ ] Create example subsetting notebooks for FVCOM and ROMS using NODD data with Xarray
    * [FVCOM](https://github.com/mpiannucci/ocean-notebooks/blob/main/ngofs2_best_subset.ipynb)
- [ ] Create python package for subsetting model data with their native grids using Xarray
    * https://github.com/asascience-open/xarray-subset-grid
- [ ] Create Xpublish plugin API to subset datasets on demand in the cloud
- [ ] Create custom Xpublish based service including all required API plugins (including the subsetting plugin)
- [ ] Create example workflow scripts and notebooks utilizing the service

### Software Infrastructure
- [ ] Dockerize the Xpublish service
- [ ] Create IaaC with Pulumi for reproducible deployment in the cloud
- [ ] Add Dask and Redis capabilities to deployment for faster processing and cacheing
- [ ] Deploy example service in the cloud
- [ ] Benchmarking and performance tuning
