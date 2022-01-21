# MOZF-ml-accuracy-maximisation
Five selected ml classifiers maximisation for done on some financial data. 

1.Random forest boosting (eXtreme Gradient Boosting Training) 
	- trafność: 90.67%
	- parameters: [booster = "gbtree", objective = "binary:logistic", eta=0.39, gamma=0, max_depth=7, min_child_weight=5, subsample=1, colsample_bytree=1, nrounds = 25, early.stop.round = 20, maximize = F , eval_metric = "error"] 
	- functions: [xgb.cv, xgb.train]
2.Logit model classifier (stats)
	- trafność: 86%
	- features: W3 + W7 + W8 + W9 + W14 + W15
	- functions: [glm]
3.Support Vector Machines (e1071)
- trafność: 85.67%
- features: W1 + W3 + W4 + W7 + W15
	- functions: [svm]
4.Naive Bayes Classifier (e1071)
	- trafność: 85%
	- features: W1 + W3 + W4 + W7 + W9 + W11 + W14
	- functions: [naiveBayes]
5.Simple Neural Network (neuralnet)
	- trafność: 51%
	- features: W1 + W3 + W4 + W7 + W8 + W9 + W11 + W13 + W14 + W15 
	- parameters: [hidden=1,act.fct = "tanh",rep=1]
	- functions: [neuralnet]
