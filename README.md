# smartFactory-LGaimers-Dacon

* LG Aimers Hackathon - Smart Factory Classification 
* code, csv files, related materials 

* 02/17/2023(FRI): 
  * preprocessing + GradientBoostingRegressor + GradientBoostingClassifier (X)
  * NO preprocessing + LGBM 
* 02/18/2023(SAT): 
  * preprocessing: fillna with feature's column mean 
  * append data for solving data imbalance 
  * further Ensemble modeling is needed 
  * Smart Factory Controling System: company's focus 
  
* 02/20/2023(MON):
  * preprocessing: fillna(0) + SMOTE oversampling  
  * train_test set split
  * f1_score macro avg 
  * Y_Quality ---> Y_Class prediction : f1_score not good 
    * directly predicts Y_Class
  * DL: TabNet techniques 
    * TabNetCalssifier modeling gets in stucked [ON GOING]
  - Ensemble Modeling 
    - 2 level stacking 
