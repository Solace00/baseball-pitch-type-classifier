# baseball-pitch-type-classifier

This repository contains a baseball pitch-type classifier that uses both linear and nonlinear models, fine-tuned with Optuna for optimized hyperparameter selection. The classifier achieves high accuracy in pitch-type classification.

## Features
- Supports linear and nonlinear models for pitch type classification.
- Uses Optuna for hyperparameter optimization and fine-tuning.
- High classification accuracy.

## Data
- **Data Sources**: Data was downloaded from baseball Savant (https://baseballsavant.mlb.com/) using pybaseball.

## Models
- **Linear Model**: for the linear model, we used logistic regression which is a statistical model that uses math to find relationships between two data factors. This model is often used for classification and predictive analytics.

- **NonLinear Model**: for the nonlinear model, we used Random Forest Classifier which is an ensemble classifier that produces multiple decision trees, using a randomly selected subset of training samples and variables. This Model produced about 81% accuracy, with a log loss of 34.07.


## Fine-tuning
- **Optuna**: Optuna is an automatic hyperparameter optimization software framework. We used Optuna to fine-tune Random forest Classifier model. The accuracy improvements are very modest, but with different parameters to tune over (we only tuned over n_estimators and max_features) or a different model type (e.g. GBM, SVM) or even more features (release point, balls + strikes, etc), we could further improve our model accuracy.

## Results
- **Linear Model**: This Model produced about 44% accuracy, with a log loss of 10.19.
- **NonLinear Model**: This Model produced about 81.5% accuracy, with a log loss of 34.07.

- **Fine-tuned NonLinear Model**: This Model produced about 81.6% accuracy, with a log loss of 33.5.
