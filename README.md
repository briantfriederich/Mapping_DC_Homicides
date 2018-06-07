# Mapping_DC_Homicides

In this project, I predicted the likelihood each street segment in DC (portions of a street between two intersections or end of a street)  experienced a homicide between 1 January 2007 and 31 October 2017, based on f1 score, through a boosted tree classification model using XGBoost based on neighborhood characteristics such as zoning and median property values. I further simplified the model by turning homicide incidence into a Boolean feature instead of a continuous feature and running an XGBoost classification, although an XGBoosted tree regression could easily be used on raw homicide counts per street for a more granular prediction of how many homicides a given street is predicted to have experienced. Finally, I will visualized the results on map using QGIS.

## Getting Started
### Prerequisites
The following project requires the following packages are installed:
* Numpy
* Pandas
* Scikit-Learn
* XGBoost
* Seaborn
* Graphviz

### Installing
Once the required packages are installed and updated, please execute the following steps to load the `homicides` environment:
```
$ cd ~/Predicting_DC_Homicides
$ conda env create -f homicides.yml
```
Once the environment is loaded, execute the following to activate the new environment:
* Windows: `$ activate homicides`
* macOS and Linux: `$ source activate homicides`

Now, check that the environment was installed correctly by running:
```
$ conda list
```
The homicides environment should appear in the list and should have an asterix next to it in the far left.

### Launching the Notebook
Execute the following to launch the Jupyter Notebook, and proceed through the notebook to run the model on the data:
```
$ Jupyter Notebook
```
## Repository Contents
The repository includes:
* Environment .yml file
* Data `FINAL_DATASET` in csv format
* Metadata *-explains the features and label in* `FINAL_DATASET` 
* Jupyter Notebook
* A PDF finalized report ***Predicting DC Homicides***
* MIT License
* README.md file

## License
This project is licensed under the MIT License


