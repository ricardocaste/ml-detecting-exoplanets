# Detecting Exoplanets from NASA Kepler Data  

**Machine Learning Engineer Nanodegree**  
**Capstone Proposal**  
Ricardo Castellanos 
January 8, 2021  


### Setup
The included Jupyter Notebook was run under a Amazon Sagemaker instance. I set up an Amazon Elastic Compute Cloud (EC2) instance on AWS to run Jupyter Notebook on GPU. I have increased service limits for p2.xlarge instance type (by default it’s 0).

This instance included CUDA support. If you are not using GPUs you will need to replace the `CuDNNLSTM` calls with basic LSTM calls.

### Libraries
The code runs with kernel conda_tensorflow_p27, and requires the following libraries, in no particular order
```
tensorflow
keras
numpy
scipy
scikit-learn
matplotlib
```

### Data

Data files required to run the code are the `exoTest` and `exoTrain` labelled time-series datasets from https://www.kaggle.com/keplersmachines/kepler-labelled-time-series-data.

or download the compressed csv from the repo `exoTest.csv.zip` and `exoTrain`
