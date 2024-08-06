# Coastal EO Applications Workshop

This workshop contains a range of notebooks, broken down into sections.

## Requirements and environment setup

Tide data access for south east asia.

```bash
wget https://s3.ap-southeast-2.amazonaws.com/files.auspatious.com/coastlines/data/tide_models_vn_ph_2022.zip \
              -O /tmp/tide_models.zip && \
            unzip /tmp/tide_models.zip -d /tmp/tide_models_temp && \
            mv /tmp/tide_models_temp ~/tide_models
```

## Key links and references

* Element-84's Earth Search STAC Catalog: `https://earth-search.aws.element84.com/v1`


## Getting started with Sentinel-2

1. [Find, load and visualise Sentinel-2 data](notebooks/Sentinel-2_GettingStarted.ipynb)
2. [Basic cloud masking for Sentinel-2](notebooks/Sentinel-2_CloudMasking.ipynb)
3. [Combining Sentinel-2 with tide model](notebooks/Sentinel-2_TideFiltering.ipynb)
4. [High- and low-tide composites](notebooks/Sentinel-2_HighLowComposites.ipynb)

## Coastlines Modelling with Landsat

1. [Find, load and visualise Landsat data](notebooks/Landsat_GettingStarted.ipynb)
2. [Basic cloud masking for Landsat](notebooks/Landsat_CloudMasking.ipynb)
3. [Step-by-step coastlines algorithm](notebooks/Coastlines_StepByStep.ipynb)
4. [Intertidal elevation modelling](notebooks/Sentinel-2_Intertiday.ipynb)
