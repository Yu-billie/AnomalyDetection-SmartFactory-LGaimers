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

- 02/21/2023(TUE): 
  - params tuning: OPTUNA 
  - XGBClassifier (predict directly Y_Class)
  
- 02/24/2023(FRI): SCORE 0.72765!!!!!
  - DL: Sequential model + catBoostClassifier + optuna params optimization  
  - 03/07 code & PPT submission  
  
- 02/25/2023(SAT): best output is not recalled 
  - sequential model: 
    - input layer, output layer(#neuron=#label)
    - num of hidden layers = 0 --> only capable of representing linear separable functions or decisions
      - when features are linearly correlated, it can be done by using ML.
      - but even in linear correlation, if neural networks are used, there is no need for any hidden layer   
      
- 02/26/2023(SUN): Tensorflow.Keras NN MLP (Sequential model) is not reproductable 
  - sequential model + optuna
    - Tensorflow.keras: random --> familiar BUT not recalled
    - Torch: unfamiliar AND output is expected to be same 
  - catBoost + GBC + voting classifier + optuna
  
- 02/27/2023(MON): focusing on ML ensemble
  - catBoost + randomizedSearch + stacking ensemble 
  - tried sequential model finally (CPU setting + seed fixing) but not recallable
- 02/28/2023(TUE): FINISHED
  - VotingClassifier 
  - based on each basic model's performance    
- RESULT
  - overfitting, CV
  
- 03/01/2023(WED): feature distribution (DATA ANALYSIS), MLP in torch 
  - feature distribution: imbalanced --> MinMaxScaler 
  - MLP: code in torch 
    - BUT still results are random 
  - FEEDBACK: 
    - tensorBoard --> automatical logging tool for parameters experiments etc. 
    - decrease # neuron slowly 
    - deep layers to make training hard --> prevent OVERFITTING 
- 03/04~03/06: PPT 
- 03/07: CODE & PPT Final Check     

