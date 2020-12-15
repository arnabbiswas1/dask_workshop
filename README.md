# Speed up Data Science Work Flow using Dask


### How to setup the Python Environment?

```
conda env create -f environment.yml
conda activate dask-tutorial
jupyter labextension install dask-labextension
jupyter serverextension enable dask_labextension
```


### How to get the data?

Data used in this project is from the Kaggle Competition "INGV - Volcanic Eruption Prediction"(https://www.kaggle.com/c/predict-volcanic-eruptions-ingv-oe). Please download the data from Kaggle and place into the `data` directory. Once done, the content of the `data` directory should have the following files & directories:

```
sample_submission.csv  
test/                  
train/                 
train.csv
```