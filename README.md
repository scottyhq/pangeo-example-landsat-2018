# pangeo-example-landsat-2018
A new example notebook for the pangeo project - cloud-native computation of NDVI

More about the awesome Pangeo Project: http://pangeo-data.org 

Coming soon:
- deploy this notebook easily with pangeo-binder!


## Landsat 8 NDVI Analysis on the Cloud

This notebook demonstrates how to run a distributed calculation of NDVI using Landsat8 data stored on AWS S3. **What is unique about this workflow is that no data is downloaded!** All calculations are performed in memory across many distributed machines on the AWS Cloud. This is possible because the Landsat 8 data is stored in [Cloud-Optimized Geotiff](http://www.cogeo.org) format, which can be accessed remotely via [xarray](http://xarray.pydata.org/en/stable/) and [rasterio](https://rasterio.readthedocs.io/en/latest/) Python libraries. Distributed computing is enabled through a [Pangeo](http://pangeo-data.org) JupyterHub deployment with [Dask Kubernetes](https://github.com/dask/dask-kubernetes).

About Landsat 8:
https://landsat.usgs.gov/landsat-8

About the AWS Landsat archive:
https://registry.opendata.aws/landsat-8/

A nice way to query this archive on S3 is the sat-search tool:
https://github.com/sat-utils/sat-search

Date: August 15, 2018

Creators:
Scott Henderson, Daniel Rothenberg, and other Pangeo Sprint participants!
