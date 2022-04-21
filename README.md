# movierecs Project
# Author: Joao Henrique Bessa Gomes

- This R project reads the movielens dataset (https://grouplens.org/datasets/movielens/10m/) containing ratings for several movies. 
- The data is parsed and split into a validation set (10% of all data entries) and a modelling set (remaining 90%).
- The modelling set is then partitioned into a training and a test set
- The model used for prediction is a penalized least squares approach, which defines a movie effect parameter (b_i), an user effect parameter (b_u) and a regularization parameter (lambda).
- The parameters are adjusted in order to minimize the root mean square error (RMSE) between the prediction and the actual test set ratings.
- The optimal set of parameters is then applied on the validation set and the RMSE between prediction and actual ratings is obtained.
