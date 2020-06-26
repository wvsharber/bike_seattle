# Bike Seattle!

Seattle often tops lists of the most bike friendly cities in the U.S., with many miles of dedicated bike trails, bike lanes, and other bike-friendly infrastructure. The City of Seattle set a goal in 2014 to quadruple ridership by 2030. As part of that effort, the city collects data on the number of bike riders who utilize various bike infrastructure in Seattle. Three of these bike counters record hourly data 24/7/365, which is uploaded daily to data.seattle.gov. 

Using bike ridership data from the City of Seattle and weather data from the Night Sky API, I use regression techniques to create a predictive model for the number of bicyclists per day based on weather and date features. 

## Repo Setup and Guide

### Setup

To utilize this repo, first fork and clone the repo. The conda environment in `environment.yml` includes the Python packages necessary to run the code in the repo. Use the following steps to complete the installation of the environment and make code stored in src available as a package.

After cloning the repo, navigate into the repo and run:

```
# create the conda environment
conda env create -f environment.yml

# activate the conda environment
conda activate bike-env

# make this conda environment available as a kernel in jupyter
python -m ipykernel install --user --name bike-env --display-name "bike-env"
```
### Guide

The repo contains data, exploratory code, and final reports in distinct directories. The `data/` directory stores both raw and processed data and includes instructions to download the data. The `notebooks/` directory holds Jupyter notebooks with exploratory code and analyses, and a final, report-like notebook. The `src/` directory holds some code needed to utilize the notebooks.