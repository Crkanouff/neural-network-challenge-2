# neural-network-challenge-2
Module 19 Challenge

Overall, this project is an advanced exercise in neural network design, aiming to address complex HR analytical tasks by leveraging machine learning. The focus on a branched neural network underscores the model's ability to cater to multifaceted prediction tasks within a single architectural framework.

It is broken into 3 parts.  

Part 1: Preprocessing
Data Import and Initial Analysis: Begin by importing the dataset and examining the first few rows to understand the structure and type of data available. It involves identifying the uniqueness of values across columns to guide the feature selection process. Feature Selection and Data Preparation: Create a separate DataFrame (y_df) for the prediction targets, namely 'attrition' and 'department'. Select at least 10 columns as features for the model (X_df), excluding the target columns. The selection process is critical to ensure the model has relevant inputs for making predictions. Preprocess the features by converting them to numeric types and scaling them, which helps in improving model performance. Also, apply one-hot encoding to the categorical targets to prepare them for model training.

Part 2: Model Creation, Compilation, and Training
Building the Model: The model architecture is not sequential but branched, reflecting the dual output objectives. It begins with a shared input layer followed by several shared layers that process the input features. From these shared layers, two branches diverge: one for predicting attrition and another for predicting the best-suited department for each employee. Each branch has its hidden layer(s) and an output layer designed to suit the nature of its prediction target. Model Compilation and Training: After constructing the model, it is compiled and trained using the preprocessed data. This stage involves selecting appropriate loss functions, optimizers, and metrics, considering the dual objectives of the model. The model's performance is evaluated using testing data, with accuracy scores generated for both prediction targets.

Part 3: Summary and Evaluation
Reflective Analysis: The final part encourages reflection on the model's performance and the suitability of accuracy as a metric for this particular problem. It prompts considerations on the choice of activation functions for the output layers, driven by the type of prediction (binary/multi-class classification). The summary seeks to identify potential improvements to the model, which could involve data augmentation, hyperparameter tuning, or exploring alternative model architectures.
