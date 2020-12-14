# Model Sharing Games

This is supporting code for https://arxiv.org/abs/2010.00753 (AAAI 2021). Note that all of the results in this paper are theoretical and so none of them strictly depend on the results in these notebooks. However, we did end up writing a fair bit of code during the process of this paper, mainly to check conjectures and verifying that theorems matched our intuition. Hopefully, these notebooks will be useful for readers who wish to experiment with our area of study themselves. If you have any questions or find any errors, please email <kdonahue@cs.cornell.edu>. 

## Overview of notebooks

`01_mean_simulation` calculates exact MSE for the mean estimation case and performs simulations for the same case, to verify that they are the same, up to noise. 

`02_regression_simulation` does the same analysis for the linear regression case. In the limit where n>>D (there are many more data points than the dimension of the linear regression problem), linear regression has the same error as mean estimation, so future cases simply use the mean estimation errors. 

`03_calculate_stability` uses the results of `01_mean_simulation` to build tools for determining which arrangements of a given set of players are stable. It also reproduces tables and error values used in the Motivating Example section and the core stability exploration in the end of Appendix D. 

