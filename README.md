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

   Model               Accuracy 
| Logistic Regression | 0.81 |
| Random Forest       | 0.80 |
| Neural Network      | 0.82 |

## Tech Stack
- Python, Pandas, NumPy
- scikit-learn
- TensorFlow / Keras
- Google Colab

## Dataset
[Titanic dataset](https://raw.githubusercontent.com/datasciencedojo/datasets/master/titanic.csv)
