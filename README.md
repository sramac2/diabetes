## Thoughts

If we compare the score of simple vs multiple linear regression. I think simple regression has a narrowed set of factors. If we compare the R2 and RMSE scores:
- Simple
    - R2: 0.23, RMSE: 63.7
- Multiple
    - R² = 0.45, RMSE = 53.9
This shows that the disease progression is not just based on a single factor it based on multiple factors. THis makes multiple regression more appropriate for this dataset. 

In polynomial Regression, when provided with a degreee of 2 and 3 it was way overfitting resulting in a R2 score of 1.0. It also performed much worset on the test set which had a negative R2 and more than 370 RMSE

Comparing the Ridge and Lasso with Multiple Regression, Ridge and Lasso perfomed better when provided with an alpha value of 0.001. 
- Ridge: R2 = 0.5108, RMSE = 50.91
- Lasso: R2 = 0.5013, RMSE = 51.40
On the other hand, when the alpha is 10, the lasso model fails drastically. We can see that in the R2 score < 0.
Regularization helps prevent overfitting and improves generalization. 

Finally I would say the best performing model would be the ridge regression with a alpha of 0.001. It provided good R2 score and lowest RMSE on test set. 


