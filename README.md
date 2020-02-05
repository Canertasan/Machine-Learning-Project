First, we tried to select the features from the list that could actually increase the reliability of the results of our project. 
We searched for the parameters that could affect someone's loan status. In the beginning, we selected a few of the given features;
as we added new ones, we saw that our accuracy increased more and more. But, as we saw in the lectures, after some point, adding 
several features could harm your system’s performance. Therefore, we tried to avoid the features that actually end up in the similar
meaning; for instance, employment length and employment title. One needs to know whether the applicant for the loan is working or 
not; and it can be understand from the job title and from employment length too. What we mean by that is if the job title is empty,
then the applicant is unemployed which is actually same as an empty job length. Therefore, we just used one of them with the other 
features such as grade, home ownership, annual income, dti, public record and so on. In order to work in an efficient way with our
data, we replaced the chosen features with related integers. Moreover, we split our data into training and validation data with 20% ratio. 
And, we saw 0.803 accuracy in our validation data. However, after testing our system with the test data, we got 0.78 accuracy.
Therefore, we tried to find other ways to increase our accuracy. We found out that making changes on hyper parameters of random forest 
which was the model we were using, could affect our accuracy. After doing some research, we found out with trial and error that
doing changes on hyper parameters such as random state, n_estimators, max_depth, min_samples_split and min_samples_leaf increased 
our accuracy to 0.801.
