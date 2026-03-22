Linear Regression is a supervised learning algorithm used to predict a continuous output variable based on input features. In this experiment, I have used fish measurements such as length, height, and width to predict the weight of the fish.

The dataset is first loaded using pandas. The input features (Length1, Length2, Length3, Height, Width) are separated from the target variable (Weight).

The dataset is divided into training and testing sets using train_test_split to evaluate model performance on unseen data.

Feature scaling is performed using StandardScaler to normalize the data. This ensures that all features contribute equally to the model and improves convergence during training.

The data is then converted into PyTorch tensors since PyTorch models operate on tensors.

A Linear Regression model is defined using nn.Linear, which represents a linear equation of the form:

y = w₁x₁ + w₂x₂ + ... + b

The model is trained using Mean Squared Error (MSE) as the loss function and Stochastic Gradient Descent (SGD) as the optimizer.

During training:

-Predictions are made
-Error is calculated
-Gradients are computed
-Weights are updated

After training, the model is evaluated using metrics such as MAE, MSE, and R² score.

The results show how well the model predicts fish weight based on physical measurements.
