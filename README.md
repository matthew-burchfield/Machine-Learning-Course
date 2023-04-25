# Machine-Learning-Course
Labs from a PhD level machine learning course I took at Northeastern University in 2020.

Lab 1 is simple exploratory data analysis and visualization.

Lab 2 explores regression methods for housing data and MRI slices.

Lab 3 explores much of the topics in Lab 1 and Lab 2. Part 1 of the lab begins with a database of voice samples consisting of 20 numeric feature variables (such as mean frequency and spectral entropy) and one target variable, namely gender of the speaker. 
We're tasked with determining which features are most predictive of gender. I answer the question qualitatively (by inspecting violin plots and box plots) as well as quantitatively (by performing regressions of the target variable against individual features). 
Part 2 of the lab is comparitively simpler. I return to the MRI data set explored in Lab 2, and once again perform regressions against the target (degree of dementia). In this case, however, I treat the target as a categorical rather than as a numeric and achieve noticeable improvements in the accuracy of the regression, thus suggesting that dementia should not be treated as a numeric but rather as a categorical.
Thus, Lab 3 is the first interesting lab of the course in the sense that it's the first time I used statistical methods in data science to uncover empirically meaningful information. 
