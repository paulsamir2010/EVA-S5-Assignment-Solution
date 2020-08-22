Dataset = MNIST

Target is to use CNN using Pytorch to obtain the following (within the constraints mentioned). 

99.4% Test Accuracy
Less than or equal to 15 Epochs
Less than 10000 Parameters

Above has to be achieved in 4 steps. So 4 iterations was done , respective file names are

Step 1.ipynb
Step 2.ipynb
Step 3.ipynb
Step 4.ipynb

Target, Result and Analysis of above iterations are stated below

Step 1
===========
Setup and skeleton
Target:
1.	Get the set-up right
2.	Set Transforms
3.	Set Data Loader
4.	Set Basic Working Code
5.	Set Basic Training  & Test Loop

Results:
1.	Parameters: 10,790
2.	Best Training Accuracy: 100
3.	Best Test Accuracy: 98.6

Analysis:
Test Accuracy is low
Model is over-fitting.

2)Batch Normalization 
Add Batch-norm to increase model efficiency.

Step 2
==========
Target:
Add Batch-normalization to increase model efficiency.
Results:
Parameters: 10,790
Best Training Accuracy: 100
Best Test Accuracy: 99.1

Analysis:
Model is over-fitting, but we are changing our model in the next step
 	Test Accuracy increased to 99.1 but below target 99.4
Parameters are more than target of 10000

Step 3
========
Add Dropout for reducing overfitting and Average Pooling

Target:
•	Reduce the overfitting by using Dropout

•	Reduce the parameters by using Avg Pooling. Also best practice is to use Avg Pooling before using FC layer

Results:
Parameters: 9990
Best Training Accuracy: 98.3
Best Test Accuracy: 98.7

Analysis:
Overfitting Problem is resolved 
	Test Accuracy dropped to 98.7 with 9990 parameters

Step 4
=============
Add Image Augmentation

Target:
•	Improve the Test accuracy from 98.7 to target 99.4

•	Add Image Augmentation (rotation) , adjust batch size, learning rate, number of parameters

Results:
•	Parameters: 9990
•	Best Training Accuracy: 98.6
•	Best Test Accuracy: 99.1

Analysis:
•	Model is not overfitting. 
•	However, Test accuracy stays at 99.1 even with Image rotation,  LR updates and update to parameters




