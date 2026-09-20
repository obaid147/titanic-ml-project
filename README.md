# Titanic Survival Prediction

## Overview
This project uses the classic Titanic dataset to predict whether a passenger survived, based on features like class, age, sex, fare, and family size.

## Approach
1. **Data Cleaning** — handled missing values in `Age` and `Embarked`, dropped `Cabin` (too many missing values)
2. **Feature Encoding** — converted categorical features (`Sex`, `Embarked`) into numeric form
3. **Train/Test Split** — 80% train, 20% test
4. **Models Trained:**
   - Logistic Regression
   - Random Forest
   - Neural Network (TensorFlow/Keras)

## Results

   Model                Single Split     5-Fold CV Mean 
| Logistic Regression   | 0.81 |          | 0.79 |
| Random Forest         | 0.80 |          | 0.81 |
| Neural Network        | 0.82 |          |   —  |

## Cross-Validation
A single train/test split can be misleading on a small dataset, so 5-fold cross-validation was used to get a more reliable comparison between Logistic Regression and Random Forest. Results show Random Forest performs slightly better on average (0.81 vs 0.79), despite Logistic Regression scoring higher on the original single split, a good reminder that one split alone isn't enough to judge a model.

## Tech Stack
- Python, Pandas, NumPy
- scikit-learn
- TensorFlow / Keras
- Google Colab

## Dataset
[Titanic dataset](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)
