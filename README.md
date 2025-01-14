# HEadLine-Generator-ML-model
A model to generate headlines for given article
This is Raw code for google collaborator,
Yet to be deployed on hugging face.





                                                                                                                                                                   
#Source of Dataset                                                                                                                                              
LABELLED_TRAIN.csv: Contains labeled data for training.        
LABELLED_DEV.csv: Contains labeled data for validation.   


#Dataset Size     
The number of rows and columns in  LABELLED_TRAIN.csv dataset is 3001 and 3 respectively      
The number of rows and columns in  LABELLED_DEV.csv dataset is 1001 and 3 respectively   

#Objective  
For help in the creation of Headline for the articles for different publisher  

#Hyperparameter and tuning   
Key Hyperparameters:-     
   Learning Rate: 5e-5  
   Batch Size: 8   
   max Input Length: 512 tokens   
Scheduler:-   
   CosineAnnealingLR (T_max aligned with total steps, eta_min=1e-6)   

#Training process    
Pipeline:-    
Training-validation split: 80-20 ratio.   
Metrics: ROUGE-L for evaluating summarization quality.   
Training Epochs:-    
Monitored loss and ROUGE-L after each epoch.    
Best model saved based on validation ROUGE-L score.   
Visualization:-   
Plots of training/validation loss and ROUGE-L scores over epochs.   

#OutPut  
Output results for UNLABELLED_TEST.csv are present in Output_Predictions.csv
