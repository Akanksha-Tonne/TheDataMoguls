 <h2>The Data Moguls<h2> 
<h4> Data Analytics Project 2019: Microsoft Malware Prediction </h4> 
<ul><li><b>Step 1 : Pre-Processing </b> { Refer to file Final/TheDataMoguls_Stage1.ipynb } <br>
This file contains code for 
 <ol><li>preprocessing
     <li>model fitting 
     <li><b>LGBM classifier</b>: obtained the AUC of 0.72
     <li>feature extraction 
     <li>visualization. </ol><br>
Since the dataset is large, running this file takes around 15 minutes.<br>
 
 <li> <b>Step 2: Data Preparation</b> {Refer to file Final/TheDataMoguls_DataPreparation.ipynb} <br>
 This file contains code for merging the original dataset with the external data provided at the kaggle notebook (https://www.kaggle.com/cdeotte/external-data-malware-0-50).<br>
 
 <li><b>Step 3:LSTM Classifier</b> {Refer to Final/TheDataMoguls_LSTM.ipynb} <br>
 This file contains code the LSTM model applied to the combined dataset. The accuracy obtained was 50%.
 <br>
 
 
 <li><b>Step 4:Adaboost Classifier </b>{Refer to file Final/TheDataMoguls_Adaboost.ipynb} <br>
 This file contains code for the Adaboost Classifier applied to the combined dataset. The accuracy obtained was 55%.
 <br>
 
 <li><b>Step 5:LightGBM Classifer {}</b> {Refer to file Final/TheDataMoguls_LightGBM.ipynb} <br>
 The lightGBM model was applied to the combined data. The AUC obtained was 0.57.
 <br>
 </ul>
 <b>Conclusion</b>
Adaboost Classifier and LSTM do not give a good accuracy for combined data. Changing parameters do not affect the results. Low accuracy indicates that the merging the datasets may not have captured the essence of the actual classification problem. <br>
Light GBM does not require categorical features to be encoded and for a time dependent classification it suits well. It is fast when applied to large datasets.
/
