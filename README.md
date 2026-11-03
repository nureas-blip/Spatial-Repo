# :artificial_satellite: Spatial Module

[![Reproducibility Check](https://github.com/nureas-blip/Spatial-Repo/actions/workflows/main.yml/badge.svg)](https://github.com/nureas-blip/Spatial-Repo/actions/workflows/main.yml)

## Team Members

🦸 Channureas Tan

## Overview

This repository tests whether the legacy of 1930s redlining is still visible in the vegetation of three American cities: New Haven, Oakland and Baltimore. The notebook reads the Mapping Inequality HOLC maps with ibis and DuckDB, computes NDVI from cloud-masked Sentinel-2 imagery found through a STAC catalog, and averages NDVI within each historical neighborhood. In all three cities, neighborhoods graded D in the 1930s have less vegetation today than those graded A, reproducing the pattern in Figure 2 of [Schell et al. 2020](https://doi.org/10.1126/science.aay4497).

## Interactive maps

Click a neighborhood to see its HOLC grade and mean NDVI.

- [New Haven](https://nureas-blip.github.io/Spatial-Repo/new_haven_ndvi.html)
- [Oakland](https://nureas-blip.github.io/Spatial-Repo/oakland_ndvi.html)
- [Baltimore](https://nureas-blip.github.io/Spatial-Repo/baltimore_ndvi.html)

## Contents

- [notebook.ipynb](notebook.ipynb): the full analysis
- `ndvi/`: NDVI rasters for each city (Cloud-Optimized GeoTIFFs)
- `web/`: the interactive map pages
- [rubric.md](rubric.md): assignment rubric

## Tools used

Python with ibis, DuckDB, geopandas, pystac-client, odc-stac, rioxarray, exactextract, plotnine and leafmap; Kilo Code (deepseek-v4-flash) in code mode; and Claude for guidance and checking.

## Links

[🌐 Course Website](https://espm-157.carlboettiger.info/)
