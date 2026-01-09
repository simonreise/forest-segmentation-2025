# Data for "_Characterizing long-term boreal forest ecosystems dynamics in Khanty-Mansi Autonomous Okrug (Western Siberia) using time series remote sensing data and deep learning methods_"

## Paper

Paper is published at ISPRS Journal of Photogrammetry and Remote Sensing and is available at (link here)

## Jupyter notebooks

The root directory of this repo contains Jupyter notebooks with Python code that was used to process the data, train the models and generate maps.

- `1_Landsat_preprocess` - preprocessing Landsat imagery
- `2_indices` - calculating NDVI and NBR
- `3_DEM_preprocess` - preprocessing FABDEM and calculating slope, aspect and curvature
- `4_climate_preprocess` - preprocessing CHELSA climatologies and ESA WorldCover landcover data
- `5_forestry_preprocess` - preprocessing and cleaning forest inventory data
- `6_create_datasets` - generating ML-ready datasets
- `7_training` - training and testing the models
- `8_mapping` - generating maps from models predictions
- `9_analysis` - analyzing data and creating figures and tables
- `delta_nbr` - calculating dNBR for forestry data cleanup

## Statistics

`statistics` directory contains CSV files with statistical summaries that describe how the area of each class (for semantic segmentation models) or mean value and proportion of values in specific ranges (for regression models) changed over years.

File suffixes:
- No suffix - statistics for the whole region area
- `_0` - Ket-Vakh middle taiga plain
- `_1` - Konda-Vakh middle- and southern-taiga lake-and-mire lowlands
- `_2` - Ob-Yenisei alternating uplands and lowlands of the northern taiga subzone
- `_3` - Ob-Irtysh floodplain-terrace meadow-mire-forest intrazonal region
- `_4` - Ob-Irtysh poorly drained taiga terraced plains
- `_5` - Pre-Yenisei elevated dissected middle-taiga plains
- `_6` - Subpolar Urals
- `_7` - Northern Urals
- `_8` - Siberian Uvaly elevated middle-taiga plains
- `_9` - Ural-Ob elevated and valley-lowland northern and middle-taiga

## Model logs

`model_logs` directory contains model logging data in CSV and TensorBoard format that show how different model metrics changed while training and validating the model.

## Google Earth Engine scripts

[LandTrendr data download](https://code.earthengine.google.com/4c60447c34dc82beaad137a0af9059dc)

[FabDEM data download](https://code.earthengine.google.com/8ce380e1cfb2396770c355e43428763d)

## Model checkpoints

Model checkpoints are stored on [HuggingFace Hub](https://huggingface.co/simonreise/forest-segmentation-2025)

## Maps

Yearly maps of forest parameters are stored on [Zenodo](https://doi.org/10.5281/zenodo.18054578)




