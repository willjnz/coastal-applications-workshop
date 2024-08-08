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

## Notebooks

### Getting started with Sentinel-2

[Find, load and visualise Sentinel-2 data](notebooks/Sentinel-2_GettingStarted.ipynb)

### High- and Low-Tide Composites with Sentinel-2

[High- and low-tide composites](notebooks/Sentinel-2_HighLowComposites.ipynb)

### Getting started with Landsat

[Find, load and visualise Landsat data](notebooks/Landsat_GettingStarted.ipynb)

### Coastline Extraction with Landsat 

[Step-by-step coastlines algorithm](notebooks/Landsat_CoastalChange.ipynb)

### Intertidal elevation modelling

TODO: adapt https://github.com/GeoscienceAustralia/dea-intertidal/blob/rbt/notebooks/Intertidal_elevation_stac.ipynb

<!-- [Intertidal elevation modelling](notebooks/Sentinel-2_Intertidal.ipynb) -->


### Mangroves

For another example, we could use global mangrove watch to identify/quantify mangroves.
