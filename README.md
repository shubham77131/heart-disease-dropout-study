# heart-disease-dropout-study
A comparative study using TensorFlow/Keras to analyze overfitting in neural networks. Features a side-by-side performance evaluation of Sequential models with and without Dropout regularization.

# Heart Disease Classification: A Dropout Study

This project implements a Deep Learning model to predict heart disease using clinical data. The primary focus is a comparative analysis of model generalization with and without **Dropout Regularization**.

## The Experiment
I built two Sequential Neural Networks to observe how regularization affects the learning curve over 130 epochs:
- **Model 1 (Regularized):** Includes Dropout layers (20% and 10%) to reduce dependency on specific neurons.
- **Model 2 (Baseline):** A standard fully connected network without dropout.


| Accuracy Without Dropout | Accuracy With Dropout |
| :---: | :---: |
| ![](/figs/accuracy_without_dropout.png) | ![](/figs/accuracy_with_dropout.png) |


## Key Features
- **Data Scaling:** Used `StandardScaler` to normalize feature ranges.
- **Exploratory Analysis:** Included a Correlation Heatmap to understand feature relationships.
- **Comparative Training:** Side-by-side Accuracy/Loss plots to visualize the "Overfitting Gap."

## Libraries requirement
- **Framework:** TensorFlow / Keras
- **Libraries:** Pandas, NumPy, Scikit-Learn, Seaborn, Matplotlib

## Analysis of Results
| Model | Generalization | Observation |
| :--- | :--- | :--- |
| **Without Dropout** | Lower | Training accuracy converges to ~100%, but validation lags. |
| **With Dropout** | Higher | More stable validation accuracy and smaller gap between curves. |

## 🏃 How to Use
The project is provided as a Jupyter Notebook. 
1. Install dependencies: `pip install tensorflow pandas seaborn scikit-learn`
2. Run the script to generate the comparison plots.
