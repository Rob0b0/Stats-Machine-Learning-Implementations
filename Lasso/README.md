# Lasso Feature "Shrinking"

*  I used Lasso regularization as my tool to sparse-out the resulting linear function. I used `sklearn.linear_model.Lasso` as my regression function, because it has the ability to return a `sparse_coef_` which only contains weights that are important. The function also gives the chance to tweak with alpha, which is the coefficient before L1 regularization parameter. I found 10 features that influence the linear function most with `alpha=0.5`.  

* ```
    (0, 1)	0.598070793415
    (0, 2)	0.490584380386
    (0, 4)	0.618326948097
    (0, 6)	0.837668121699
    (0, 10)	0.477131778559
    (0, 12)	0.327318840711
    (0, 16)	0.172724496515
    (0, 18)	0.374728831955
    (0, 22)	0.709102367009
    (0, 26)	0.520022742356
  ```