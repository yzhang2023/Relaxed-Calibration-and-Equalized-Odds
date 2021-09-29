# Relaxed-Calibration-and-Equalized-Odds
In this project, we are aiming at post-processing a given dataset so that it achieves a balance in equalized odds and calibration. 
Equalized odds ensures that both the false positive rates and the false negative rates are the same in the protected groups, or in other words, no error rate will disproportionally affect any protected group. 
While maintaining calibration ensures that the predicted values of the algorithm evaluates the real probability, and failure in doing so leads to decreasing credibility on the algorithm. 

In order to achieve the goal of non-discrimination, both equalized odds and calibration must be enforced. 
However, it is proposed that these two characteristics are inherently conflicted, and perfectly achieving both would be impossible. 
As a result, we would like to achieve a relaxed version of both characteristics, and find the most satisfactory result under the constraints. 
Our algorithm can post-process a given dataset when given the constraints for calibration and equalized odds. 

## How to use
The file `Calibration_Eq_odds.py` contains the code for the post-processing methods for achieving the relaxed notions of equalized odds and calibration. 
It expects a file input of a dataset of predictions, protected group labelings, and ground-truth labels from an existing model. 
And as the two constraints are also inputed, the algorithm can post-process the data and give out a result that satisfy the two constraints if the constraints are not conflicted. 
See the demos in the file for example usage. 


