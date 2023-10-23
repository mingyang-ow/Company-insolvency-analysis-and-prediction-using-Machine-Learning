## <strong>Bankcruptcy Predition</strong>
This notebook is designed for the examination of financial data from 6819 Taiwan companies. Its primary objective is to assess and predict if a company will bankcrupt in the long run using the financial data.<br>
As the dataset is imbalanced, upsampling of the dataset using SMOTETomek was applied and a model was trained using machine learning and the model was assessed with the best parameters. <br>
This comparison was done to gauge the model's effectiveness in predicting bankcrupty possibility. <br>

Before Upsampling using SMOTETomek
f1-score: 0.49350167099888603
1329 True Negative, 0, False Positive, 35 False Negative ,0 True Positive. <br>

After Upsampling using SMOTETomek
f1-score: 0.7252864782276547
1280 True Negative, 31 False Positive, 27 False Negative, 26 True Positive.<br>
Reduction in number of False Negative and increase in True Positive infered that the Upsampling of the data was successful in the Model Creation. <br>
