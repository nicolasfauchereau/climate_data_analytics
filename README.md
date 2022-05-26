# University of Otago Climate Data and Analytics Workshop (26 May 2022)

This github repository contains material for an introductory workshop on using 
the Python scientific 'ecosystem' to access and analyse climate data, given for the 
He Kaupapa Hononga and Otago Climate Change Postgraduate Network (OCCPN). 

The introductory slides can be found [here](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/slides/climate_data_workshop.pdf) 

In the [notebooks](https://github.com/nicolasfauchereau/climate_data_analytics/tree/main/notebooks) folder, you will find 6 [Jupyter notebooks](https://jupyter.org/): 

- [Jupyter_notebooks.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/Jupyter_notebooks.ipynb) provides a very brief overview of the Jupyter notebook (and [Jupyter lab](https://jupyter.org/)) development environment  
- [Pandas_NZ_station_data.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/Pandas_NZ_station_data.ipynb)   shows how to read a csv file using [pandas](https://pandas.pydata.org/) and perform some basic operations on pandas's [DataFrames](https://pandas.pydata.org/docs/reference/api/pandas.DataFrame.html)  
- [reanalyses.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/reanalyses.ipynb) shows how to access NCEP/NCAR and ERA5 reanalysis data 'remotely' (i.e. without having to download the data) using [xarray](http://www.xarray.pydata.org)  
- [global_average_temp_NCEP.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/global_average_temp_NCEP.ipynb) shows how to calculate global area-weigthed temperature anomalies, using the NCEP/NCAR reanalysis product (1948-2021)  
- [CMIP6_in_the_cloud.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/CMIP6_in_the_cloud.ipynb) shows how to access a subset of the CMIP6 climate change model's simulations on the Google cloud  
- [downscaled_CMIP6.ipynb](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/downscaled_CMIP6.ipynb) provides some pointers towards bias-corrected and downscaled CMIP6 global datasets  

---- 
### creating a Python environment with the required packages 

The first step is to download and install either the [anaconda](https://www.anaconda.com/) or the [mambaforge](https://github.com/conda-forge/miniforge#mambaforge) Python distribution.

You can then download (or git clone) the content of this repository (e.g. 'code / Download ZIP` in the upper right)

The [environment.yml](https://github.com/nicolasfauchereau/climate_data_analytics/blob/main/notebooks/Pandas_NZ_station_data.ipynb) file provides the list of packages used or relied upon for this workshop. 

You can create a `climatedata` environment using [conda](https://docs.conda.io/en/latest/) or [mamba](https://mamba.readthedocs.io/en/latest/) by typing: 

```
conda env create -f environment.yml
```

or 

```
mamba env create -f environment.yml​
```

in a terminal 

The environment is activated using  

```
conda activate climatedata
```

or 

```
mamba activate climatedata 
```

Then navigate to the `notebooks` folder and type 


```
jupyter notebook
```

for the classic notebook interface, or 

```
jupyter lab
```

For jupyterlab 


Any questions: [Nicolas Fauchereau](mailto:Nicolas.Fauchereau@niwa.co.nz)
