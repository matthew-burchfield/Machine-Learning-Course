# Machine-Learning-Course
Labs from a PhD level machine learning course I took at Northeastern University in 2020.

Lab 1 is simple exploratory data analysis and visualization.

Lab 2 explores regression methods for housing data and MRI slices.

Lab 3 explores much of the topics in Lab 1 and Lab 2. Part 1 of the lab begins with a database of voice samples consisting of 20 numeric feature variables (such as mean frequency and spectral entropy) and one target variable, namely gender of the speaker. 
We're tasked with determining which features are most predictive of gender. I answer the question qualitatively (by inspecting violin plots and box plots) as well as quantitatively (by performing regressions of the target variable against individual features). 
Part 2 of the lab is comparitively simpler. I return to the MRI data set explored in Lab 2, and once again perform regressions against the target (degree of dementia). In this case, however, I treat the target as a categorical rather than as a numeric and achieve noticeable improvements in the accuracy of the regression, thus suggesting that dementia should not be treated as a numeric but rather as a categorical.
Thus, Lab 3 is the first interesting lab of the course in the sense that it's the first time I used statistical methods in data science to uncover empirically meaningful information. 

In Lab 4 I construct two artificial neural networks using tensorflow. One classifies the MNIST dataset, and the other classifies MRI slices with the target variable being degree of dementia (note that this is the same dataset as in Lab 3). I achieve 98% accuracy on the validation data for the MNIST dataset. In this lab the model is built iteratively, beginning with a simple ANN with one hidden layer which is gradually made more complex by adding more layers, dropouts, callbacks etc, gradually improving accuracy in each step. Dropouts are used to inoculate against overfitting. Batch normalization address the problem of vanishing gradients, which I discovered after directly inspecting the gradients at each layer. I also explore different activation functions and loss functions until I arrive at the optimal choices.

Problem 2 was far more elusive. I was unable to achieve accuracy on the validation data that was much better than the regression methods explored in Lab 3. Any attempts made at improving training accuracy essentially amount to overfitting, resulting in training accuracy that diverges from validation accuracy. I did, however, find further evidence to advance the conclusion that state of dementia should be treated as a categorical when, at the end of the lab, I changed the output activation function to ReLU only to achieve disastrous results in accuracy.
. 
