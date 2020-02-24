#### Inverview study guide

- If you wanted to predict customer churn what subset of ML would you use?
    - Classification

- What is feature engineering?
    - Feature engineering is creating new features derived from already existed data points.

- What is the difference between a regression and classification problem?
    - Regression predicts a continuous target, classification predicts a distrete target.

- How would you measure the effectiveness of a model?
    - Run model against test and train datasets
    - Cross validation
    - Use F1, precision, or accuracy scores to determine which best fits your desired results.

- How is KNN different from k-means clustering?
    - KNN is supervised and requires labeled data to classify
    - K Means is unsupervised and used for clustering

- How do you handle missing or corrupted data?
    - you can drop data if the dataset is sufficiently large
    - replace data with another logical value (mean, prior day value, median, etc)

- How is a decision tree pruned?
    - Reduced error pruning is the simplest method: replace each node. If it doesn't decrease accuracy, keep it pruned.

- A model performs at 99% accuracy. Under what conditions could this metric be misleading?
    - Detecting fraud is one real world example. Any model where one outcome is heavily skewed would need additional analysis of the quality of the model.

- What is the F1 score and how would you use it?
    - The weighted average of precision and recall. Used when true negatives are not overly important.

- How would you handle an imbalanced dataset?
    - Collect more data to balance
    - Resample and stratify the data
    - Use a random subset of the over represented data.

- Explain A/B testing use cases, goals, method
    - Used to test two different choices against each other.
    - Goal is to identify which choice is more likely used
    - Method: Depends on the use case. Used in web page design optimization, in this instance it could be the click through rate of an ad depending on where it is placed on the page.

- Explain what overfitting is. How would you control for it?
    - Overfitting is when you find results that are too closely fit to your train dataset and cannot be reproduced with the test or future datasets.
    - Reduce numer of features, use cross validation, and regularization techniques like LASSO to penalize overfitting parameters.
    - Examples: Regression model that hits each sample data point, a decision tree that is set too deep and finds the sample observation.

- What is spurious correlation?
    - Spurious correlation is when two variables appear to be correlated but it is coincidence or related to an unseen third (or more factors)

- What are the most important Python libraries for data science?
    - Pandas, Numpy, sklearn, matplotlib

- What is the difference between long and wide formatted data?
    - Long data is presented vertically in a table, wide is presented horizontally

- How would you know if you have normal distribution?
    - Unimodal
    - symetrical left and right halfs
    - bell shaped
    - mean, median, and mode are all located near center

- What can you infer about probabilities know you have normal distribution
    - ability to measure what % of the population is included based on distance from the mean.
    - 

- Which data scientist do you admire most? Which startups?
    - Steven Levitt, not technically a data scientist, but he was the first person I came across who was using data in creative and unique ways to uncover answers that others were missing.
    - Nate Silver is a more traditional data scientist that I admire. He wrote the book Signal and the Noise and is the creator of the FiveThirtyEight website. He was a very early adopter in the world of data science and predictive modeling.
    - I appreciate what companies like Quickpath are doing. They are helping companies see the value and business application of data science when they don't even know they need it.

- What is your favorite ML algorithm? Why? 
    - I like logistic regression for classification. Useful for understanding several independent variables. Easy to explain results over more black box type algorithms.

- What is the difference between a Type I and Type II error?
    - A Type I error is a false positive, a Type II is a false negative. Type I erros means claiming something happened that hasn't, while Type II error means claim nothing when something happened.
    - A clever way to think about this is to think of Type I error as telling a man he is pregnant, while Type II error means you tell a pregnant woman she isn’t carrying a baby.

- What is the difference between supervised and unsupervised machine learning?
    - supervised uses labeled data, unsupervised uses unlabled data

- If you could spend the next week doing a data science project what would you do?
    - I would like to work on a project for my wife's non profit predicting likely donors based on their demographics and interests.

- How do you rest your brain from looking at a computer screen?
    - I like to step outside and take a walk when I need a break from the computer.

- How do you start a project?
    - I like to start a project by really understanding what question(s) I am trying to answer. Thinking about what kind of data I might need to answer such a question and the feasibility of acquiring that data. I try to take a very unstructured look at my problem that isn't constrained by preconceived ideas or expectations.

- What is Bayes' Theorem?
    - It is the true positive rate of a condition sample divided by the sum of the false positive rate.
    - If you h

- Why is "Naive" Bayes naive?
    - it implies absolute independence of features, very unlikely in real life scenarios.

##### Confusion matrix
            predicted: NO   predicted: YES    Total
actual: NO      TN = 50         FP =  10       60
actual: YES     FN =  5         TP = 100      105
                     55              110

    - accuracy: what % of predictions were correct
    - precision: what % of the positive predictions did you catch
    - recall: what percent of the positive cases 

- What could be happening if a model appeared to perform well when training/test but when deployed the results were drastically different?
    - This could be caused by not having a representative dataset. ie used only data from Texas to predict love of breakfast tacos nationwide.

- What is bootstrapping?
    - Bootstrapping is a resampling technique
    - also known as bagging

- What is boosting?
    - boosting is algorithm that seeks to improve prediction by training a sequence of weak models that compensate the weakness of prior models

- What are ensemble models?
    - ensemble models are models that use multiple models to attempt to better make a prediction.

- What is machine learning?
    - Machine learning is a method of data analysis that automates analytical model building. It is a branch of artificial intelligence based on the idea that systems can learn from data, identify patterns and make decisions with minimal human intervention

- What are common classificastion algorithms?
    - Logistic regression, KNN, Decision Tree

- What are common Regression algorithms?
    - Linear Regression, LASSO Regression (Least Absolute Selection Shrinkage Operator)

- How can you identify outliers?
    - IQR, Box Plot, Z-score

- Describe Data Science Pipeline
    - Plan, Acquire, Prep, Explore/Analze, Model, Deploy

- What are some data products or deliverables you might develop as a data scientist?
     - predicting seasonal sales, customer churn, voter turnout, etc

- How would you determine optimal k for your k means?
    - elbow method

- What are important Python specific skills to have for data analysis?
    - list, dictionary, tuple, set manipulation
    - Pandas Dataframes
    - Scikit-learn familiarity
    - Small, clean functions

- What is one hot enocoder?
    - converting categorical variables into a form more easily handled by ML algorithms

- What is a dummy variable?
    - A value of 0 or 1 to indicate the absense or presence of a categorical variable

- What are some resampling methods?
    - Cross validation, bootstrap

- What is logistic regression? When might you use it? Explain the difference between logistic and linear Regression
    - Logistic regression is used to predict binary outcomes from a linear combination of predictor features. 
    - Linear is used to predict the value of a discrete target.

- What is p value?
    - p value is the probability of obtaining the observed result and wasn't just random chance.

- How do you deal with seasonality in Time Series Analysis?
    - Differencing: if there is weekly seasonality, you can subtract the prior week's value from the current week's to account for the weekly swing.
    - Looking at different types of moving averages

