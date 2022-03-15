# Netflix-Appetency
This dataset is a dataset from one of the KAGGLE Competetions. The output is to find probability of consumer willing to suscribe to the Netflix. We are given a data with 70k rows and 509 columns. This dataset contatins categorical, timeseries, object ,integer and float data values and has lot of NAN Values. A sample of dataset is given below
![image](https://user-images.githubusercontent.com/93844635/158296193-3a9e474f-76f8-46f3-baeb-c6ea5f185182.png)

PreProcessing

Careful Preprocessing is done to remove the useless columns which has less variance and columns with many NAN values is also reduced. Plus the feature engineering is done to extract the useful the time series columns. As this is a categorical dataset, label encoding is applied to object columns.

ML Model

XGBOOST MODEL is used for this dataset. The dataset is converted to XGBOOST API  and model tuning was done intesively to find the best parameters of the model. The metric used here is AUC as it is the proper metric for a Classification problem. Cross validation was done to find the useful hyperparameters. 

Submission

After training the model and submitting the predictions, the AUC Score i got was 0.78442 which is a decent score for this dataset which has lot of preprocessing and datacleaning to do.
![image](https://user-images.githubusercontent.com/93844635/158296883-008e1644-1ca2-4030-82d0-6b3223184715.png)
