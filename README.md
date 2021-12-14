# AWS-ML-Blackbelt-BankingFraud

## Results of Sagemaker Canvas Project

As an initial step to using the dataset and to set a benchmark for performance, I created a Sagemaker Canvas training job on the day that Canvas was released using the bank fraud data. 

We will use this Canvas Auto-ML job as a baseline for our modeling because it took about 10 minutes to start training.

Here is the confusion matrix:

![Sagemaker Canvas Confusion Matrix](./advanced_metrics.png)

Unfortunately we likely should have inverted positive and negative classes so that "positive" means "is fraud."  Simply inverting from this matrix we see 

TN = 1269953
TP = 1579
FN = 55
FP = 680

p = precision = TP/(TP+FP) = 0.699
r = recall = TP/(TP+FN) = 0.966

F1 = 2 / (1/p + 1/r) = 0.811



