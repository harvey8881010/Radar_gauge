# Guide on code used in the research project: "Identifying Radar-Gauge Rainfall Discrepancy Using Machine Learning Algorithms" 

## Table of Contents
1. [Introduction](#introduction)
2. [Dependencies](#dependencies)
3. [Data Import](#data-import)
    - [Gauge Data](#gauge-data)
    - [Sonde Data](#sonde-data)
    - [Radar Data](#radar-data)
4. [Usage](#usage)
5. [Support](#support)

## Introduction
This repository contains the Python code and Jupyter Notebook used for data analysis in our meteorological study. This `README` guides you through the setup and data import steps.

## Dependencies

- **Python Version**: 3.9.13
- **Libraries**:
    - os
    - xarray (xr)
    - matplotlib.pyplot (plt)
    - numpy (np)
    - matplotlib.dates (mdates)
    - matplotlib.colors (ListedColormap)
    - pandas (pd)
    - netCDF4 (nc)
    - datetime
    - statsmodels.api (sm)
    - keras
        - Sequential, LSTM, Dense, Dropout, Conv2D, MaxPooling2D, Flatten
        - Optimizers: Adam
        - Callbacks: ReduceLROnPlateau, EarlyStopping, ModelCheckpoint
    - tensorflow.keras.utils (plot_model)

## Data Import

### Gauge Data

1. File format: `sgpprecipmetI10.b1.*.custom.nc`
2. Save the gauge data files in a folder.
3. In the Jupyter Notebook, update the `path` variable to point to your folder.
    ```python
    path = '/path/to/your/folder'
    ```

### Sonde Data

1. File format: `sgpinterpolatedsondeC1.c1.*.custom.nc`
2. Save the sonde data files in a folder.
3. In the Jupyter Notebook, update the `path_s` variable to point to your folder.
    ```python
    path_s = '/path/to/your/sonde/folder'
    ```

### Radar Data

1. File format: `st4_conus.*.01h.nc`
2. Save the radar data files in a folder.
3. In the Jupyter Notebook, navigate to the section titled "Radar Data" and update the `path_r` variable to point to your folder.
    ```python
    path_r = '/path/to/your/radar/folder'
    ```

## Usage

The code and results are structured in a Jupyter Notebook. The output for each code cell is already displayed in the notebook, so you don't need to rerun the cells to view the results.

## Support

For any issues or questions regarding the code and data import, please email: [anakin2013chan@gmail.com](mailto:anakin2013chan@gmail.com)
