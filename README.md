                            ------------INTRODUCTION------------------

we aimed in this challenge to underststand how to plot a DL model and to figure out the diffrence of using it comparing to the ML model for the same DATASET(problematique), and to know how to choose the best one for our case + how to avoid the cummon preblems that we usually face while working with DL model!


                           -------------METHODODLOGY--------------------

1. cleaning the dataset(hundling missing values)&
(converting categorical data)

2. creating a copy from the dataframe for:
-using standardscaling for Ml model while using Minmaxscaler for the Dl model to scale the data for each model dataset

3. try to feature engeneer the datasets(better to not add any thing in my case)

4. spliting the data

5. try to visualize the data to see its relations with the target

6. decresing the threshold to increase the recall 

7. plot the ML model and calculate its metrics at each time we plot new feature engeneering(we stop if we find the sweetspot between high recall and other good metrics) and we plot the confusion matrix

8. we plot the DL model by trying a spesific number of epochs at each iteration(30 to 100) and we calculate the model metrics at each iteration and we finely save the best number of epochs and then we plot the confusion matrix


                     --------------------RESULTS--------------------------
1. the ML model results :
Accuracy:  0.8152 (81.52%)*
Precision: 0.7656 (76.56%)*
Recall:    0.9608 (96.08%)*
F1-Score:  0.8522 (85.22%)*
2. the DL model results
Accuracy:  0.8260
Precision: 0.8254 
Recall:    0.9123 
F1-Score:  0.8667 


Criteria	            ML Model	   DL Model
Training time	        5 seconds      15 seconds
Overfitting behavior	slow            fast


                    ----------------------COMPARATIVE STUDY------------------

 DL model performs better than the ml model becaue :
1. it is more balanced between catching disease and avoiding false alarms
2. excellent recall at 91%

                    ----------------------ANSWERS-------------------------------

1. the dl models are not always better than the ml models :they are eazy to overfit on simple dataset comparing to ml models 
2. we use the ml models if we have few features &  small-medium tabular data and also if the features have  lineaire relation with target ,simple data(not text or image or audio), limited computer power


                    --------------------------Conclusion--------------------------

the strengh of our predictions depend on our choosing of the model type  depending on our data size and complexity