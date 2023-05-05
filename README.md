# In-Vehicle-Coupon-Recommender
## Dataset
This data was collected via a survey on Amazon Mechanical Turk. The survey describes different driving scenarios including the destination, current time, weather, passenger, etc., and then ask the person whether he will accept the coupon if he is the driver. For more information about the dataset, please refer to the paper:
Wang, Tong, Cynthia Rudin, Finale Doshi-Velez, Yimin Liu, Erica Klampfl, and Perry MacNeille. 'A bayesian framework for learning rule sets for interpretable classification.' The Journal of Machine Learning Research 18, no. 1 (2017): 2357-2393

##Summary 
This project involved Data Cleaning and Data Visualization using Univariate and Bivariate Analysis. Through bivariate analysis, the Python libraries such as matplotlib and seaborn are implemented to create a 3x3 grid of subplots with the specified figsize. The subplots are flattened into a 1D array for convenience.
Then, a loop is executed where each subplot is assigned to a variable ax, and a categorical variable col is selected from the columns - 'destination', 'passenger', 'weather', 'time', 'coupon', 'expiration', 'gender', 'maritalStatus', 'education', for plotting.
In each iteration of the loop, the seaborn countplot() function is used to create a bar chart of the col variable, colored by the binary variable Y, and the resulting plot is displayed on the corresponding ax subplot.
Finally, plt.tight_layout() is called to improve the layout of the subplots, and plt.show() displays the complete figure.
Overall, the below code is creating a 3x3 grid of bar charts that visualize the distribution of the specified categorical variables in a DataFrame df, colored by the binary variable Y.
Further by plotting the ROC and AUC curves and calculating the AUC,it was evaluated how well the model is able to distinguish between positive and negative examples. The ROC curve provides a visual representation of the performance of the model at different thresholds, allowing us to select a threshold that balances the trade-off between TPR and FPR based on specific application. The AUC is a summary statistic that provides a single number that can be used to compare the performance of different models or to track the performance of a model over time.
