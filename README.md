# Scale up Data Science Work Flow using Dask

As a Data Scientist, we encounter few major challenges while dealing with large volume of data: 

1. Popular libraries like Numpy, Pandas are not designed to scale beyond a single core/processor.
2. Numpy, Pandas, Scikit-Learn are not designed to scale beyond a single machine (Scikit-Learn can utilize multiple cores).
3. For a laptop or workstation, RAM is often limited to 16 or 32 GB. For Numpy, Pandas, Scikit-Learn, data needs to be loaded into RAM. So, if size of the data exceeds size of the main memory, these libraries can't be used.

In this presentation, I discuss how these challenges can be addressed using open source, parallel computation library **Dask**.

Accompanying presentation can be found at https://speakerdeck.com/arnabbiswas1/scale-up-your-data-science-work-flow-using-dask

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
