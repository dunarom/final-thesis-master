Atemp mechanism shift experiments

This notebook builds a controlled mechanism shift experiment on the Bike Sharing Dataset daily aggregation.
The shift modifies the feels like temperature variable atemp and propagates the change to the outcome casual on the held out split.

Contents
  experiment_atem_shift.ipynb

Input data
  day.csv from the UCI Bike Sharing Dataset

Dependencies (found in requirements.txt)
  numpy
  pandas
  matplotlib
  scikit learn

How to run
  1. Create a Python environment and install dependencies
  2. Place day.csv where the notebook expects it, or update the data path in the notebook
  3. Run the notebook top to bottom to reproduce the shift construction and the evaluation results

Outputs
  Diagnostic plots comparing original and shifted distributions and model performance under both environments

Reproducibility notes
  Models are trained only on the original training split
  The shifted dataset is generated only for the held out split
  A fixed random seed is used for shifted outcome sampling
