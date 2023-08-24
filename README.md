# LogisticRegression
# Linear Regression From Scratch
- step 1: initialize learning rate(lr) number of iterations(n_iters)(epochs), weights and bias 
- step 2: Fit Function:
    - extract number of rows and number of columns from the given training data passed to fit function.
    - weights -> 0 , bias -> 0
    - initialize y_hat = wx + b
    - loop to update the value of weights and bias using the formula
        - dw = (1/n) ∑(y - y_hat) * X
        - db = (1/n) ∑(y - y_hat)
        - weight(new) = weight(old) + lr * dw
        - bias(new) = bias(old) + lr * db

- step 3: Predict Funciton: 
    - y_hat  = WX + b and return y_hat



# Logistic Regression From Scratch
- step 1: initialize learning rate(lr) number of iterations(n_iters)(epochs), weights and bias 
- step 2: Fit Function:
    - extract number of rows and number of columns from the given training data passed to fit function.
    - weights -> 0 , bias -> 0
    - initialize y_hat = wx + b and pass the obtained output to sigmoid function
        - sigmoid function: 
            - S(x)= 1/ 1+e^(-x)

    - loop to update the value of weights and bias using the formula
        - dw = (1/n) ∑(y - y_hat) * X
        - db = (1/n) ∑(y - y_hat)
        - weight(new) = weight(old) + lr * dw
        - biad(new) = bias(old) + lr * db

- step 3: Predict Funciton: 
    - prediction = WX + b and pass the obtained output to sigmoid function. Return 0 if the output of sigmoid function is <= 0.5 and 1 if > 0.5

