# LoLPredictionML
Comparison of machine learning models to predict the victory of a League of Legends game with stadistics of the first 10 minutes.

## Preparation
Data clean up was performed and feature selection was made based on the context of the game.

Size of data: 9770 records.

Features  `[blueTowersDestroyed, blueTotalMinionsKilled, blueKills]` 

Target variable: `blueWins`

## Implementation

| Model | Precision | Confusion matrix | MAE & RMSE[^1] |
| :---: | :-------: | ---------------- | ---------- |
| [Logistic Regression 1](/Regresión_Logistica.ipynb)<br/> 80% train - 20% test | 68.62% | [ 35.11%  15.15%<br/>&nbsp; 16.22%  33.52% ] | 0.3137 <br> 0.5601 |
| [Logistic Regression 2](/Regresión_Logistica.ipynb)<br/> 66% train - 33% test | 67.96% | [ 35.22%  15.91%<br/>&nbsp; 16.12%  32.74% ] | 0.3203 <br> 0.5659 |
| [Linear SVM 1](/SVM.ipynb)<br/> 80% train - 20% test | 68.83% | [ 35.47%  14.79%<br/>&nbsp; 16.38%  33.37% ] | 0.3116 <br> 0.5582 |
| [Poly SVM 1 (k = 4)](/SVM.ipynb)<br/> 80% train - 20% test | 68.37% | [ 37.87%  12.38%<br/>&nbsp; 19.24%  30.50% ] | 0.3162 <br> 0.5623 |
| [Gaussian SVM 1](/SVM.ipynb)<br/> 80% train - 20% test | 67.71% | [ 35.06%  15.20%<br/>&nbsp; 17.09%  32.65% ] | 0.3229 <br> 0.5682 |
| [Sigmoid SVM 1](/SVM.ipynb)<br/> 80% train - 20% test | 41.15% | [ 20.27%  29.99%<br/>&nbsp; 28.86%  20.88% ] | 0.5885 <br> 0.7671 |
| [Linear SVM 2](/SVM.ipynb)<br/> 66% train - 33% test | 68.22% | [ 35.55%  15.63%<br/>&nbsp; 16.15%  32.67% ] | 0.3177 <br> 0.5637 |


[^1]:  MAE stand for Mean Absolute Error <br/> RMSE stand for Root Mean Square Error
	
