# Coastal EO Applications Workshop

This workshop contains a range of notebooks, broken down into sections.

## Requirements and environment setup

First, clone this repository: `git clone git@github.com:auspatious/coastal-applications-workshop.git`

Next, download tide model parameters for south east asia.

```bash
wget https://files.auspatious.com/coastlines/data/tide_models_vn_ph_2022.zip \
              -O /tmp/tide_models.zip && \
            unzip /tmp/tide_models.zip -d /tmp/tide_models_temp && \
            mv /tmp/tide_models_temp ~/tide_models
```

Finally, set up a custom Python environment  for the workshop.

```bash
MYENV=coastalapps 
python -m venv ~/venvs/$MYENV
realpath /env/lib/python3.10/site-packages > ~/venvs/$MYENV/lib/python3.10/site-packages/base_venv.pth
source ~/venvs/$MYENV/bin/activate
cd coastal-applications-workshop
pip install -r requirements.txt
python -m ipykernel install --user --name=$MYENV --display-name "Coastal Workshop"
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

[Worked example of intertidal elevation modelling](notebooks/examples/Intertidal_elevation_stac.ipynb)

### Sentinel-1 Water Detection

[Worked example using Sentinel-1 to detect water](notebooks/examples/Radar_water_detection.ipynb)
