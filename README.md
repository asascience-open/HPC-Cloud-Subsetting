# HPC-Cloud-Subsetting
Project tracking repository for the NOAA HPC Subsetting Model Data in the Cloud project


## Roadmap

### Software Development
- [ ] Create example subsetting notebooks for FVCOM and ROMS using NODD data
- [ ] Create python package for subsetting model data with their native grids using Xarray
- [ ] Create Xpublish plugin API to subset datasets on demand in the cloud
- [ ] Create custom Xpublish based server with docker including all required API needs (including the subsetting plugin)

### Software Infrastructure
- [ ] Dockerize the Xpublish server
- [ ] Create IaaC with Pulumi for reproducible deployment in the cloud
- [ ] Add Dask and Redis capabilities to deployment for faster processing and cacheing
- [ ] Deploy example service in the cloud
