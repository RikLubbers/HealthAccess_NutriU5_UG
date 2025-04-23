# Data Overview

| ID | Layer                        | Data                                  | Type          | Projection          | Source                                                                                   |
|----|------------------------------|---------------------------------------|---------------|---------------------|------------------------------------------------------------------------------------------|
| 1  | Landcover (scheme 1)        | Regional Centre For Mapping Of Resources For Development  | Raster        | Arc_1960_UTM_Zone_35N | [Link](http://geoportal.rcmrd.org/layers/servir%3Auganda_sentinel2_lulc2016)         |
| 2  | DEM                          | Opendata RCMRD                        | Raster        | Arc_1960_UTM_Zone_35N | [Link](https://opendata.rcmrd.org/datasets/uganda-srtm-dem-30-meters)                |
| 3  | Health centers               | Sub-Saharan public healthcare facilities dataset | Vector points | Arc_1960_UTM_Zone_35N | [Link](https://doi.org/10.1038/s41597-019-0142-2)                                    |
| 4  | Roads                        | OpenStreetMap                         | Vector lines  | Arc_1960_UTM_Zone_35N | [Link](https://data.humdata.org/dataset/hotosm_uga_roads)                              |
| 5  | Administrative boundaries    | Administrative boundaries             | Vector polygons | Arc_1960_UTM_Zone_35N | [Link](https://data.humdata.org/dataset/cod-ab-uga?)                                  |
| 7  | DHS                          | Household clusters                    | Vector points | Arc_1960_UTM_Zone_35N | [Link](https://dhsprogram.com/pubs/pdf/FR333/FR333.pdf)                                |
| 8  | Water bodies                 | Water bodies                          | Polygons      | Arc_1960_UTM_Zone_35N | [Link](https://geoportal.icpac.net/layers/geonode:uga_water_areas_dcw)                |
| 9  | Travel Time                  | Self-created                          | Odt. file/raster        | Arc_1960_UTM_Zone_35N | [odt_file](https://github.com/RikLubbers/HealthAccess_NutriU5_UG/blob/main/Data_and_Documentation/Travel_time.ods) or 10.5281/zenodo.11240433 for .odt and raster file|

## Data Usage

- **Landcover (scheme 1)**: Used to assess land cover types and to determine travel speed.

- **DEM (Digital Elevation Model)**: Utilized to make travel speed slope-dependent.

- **Health centers**: Locations of public healthcare facilities to calculate travel time from point A to B.

- **Roads**: Road network data to assign travel speed to each road segment.

- **Administrative boundaries**: No specific use in this study, but used for general reference.

- **DHS (Demographic and Health Survey)**: Household clusters to calculate travel time from point A to B.

- **Water bodies**: Information on water bodies to exclude from travel time calculations.

- **Travel Time**: Self-created raster layer representing travel times to healthcare facilities, used in linear regression analyses.

## Travel Speed by Land Cover Type

| Landcover                                            | Speed (km/hr.) |
|------------------------------------------------------|----------------|
| Primary road                                         | 5              |
| Secondary road                                       | 5              |
| Tertiary road                                       | 5              |
| Forests                                              | 1.67           |
| Shrublands                                           | 2.5            |
| Grassland                                            | 1.67           |
| Cropland                                             | 1.67           |
| Bare areas                                           | 2.5            |
| Sparse vegetation                                    | 2.5            |
| Built up areas                                       | 5              |
| Regularly flooded areas or aquatic vegetation       | 1              |
| Open Water                                           | 0              |
