### Project Title
Creation of Machine Learning models that can be used to predict weight loss using exercise and dietary information for use by stakeholders that want to understand the features that are key for weight loss.


**Author**
Ratan Yalamanchili
#### Executive summary
Machine learning (ML) is a branch of Artificial Intelligence (AI) that enables computers to “self-learn” from training data and improve over time, without being explicitly programmed. This can be used to predict weight loss, as people who lose weight tend to have certain patterns in their behavior. For example, they may eat less, exercise more, or change their diet. By analyzing data from people who have lost weight, machine learning algorithms can identify these patterns and use them to predict whether or not someone will be successful in their weight loss efforts.

This technology has the potential to revolutionize the way we think about weight loss. Instead of relying on traditional methods like dieting and exercise, we may be able to use machine learning to create personalized weight loss plans that are more likely to be successful.


#### Rationale
Weight loss is a difficult and often frustrating process, but it can be life-changing. Here are just a few reasons why anyone should care about weight loss:

Weight loss can improve your health, extra weight puts a strain on your heart, lungs, and joint and losing this weight can help to reduce your risk of developing health problems like heart disease, stroke, and type 2 diabetes
Weight loss can improve your self-esteem, the extra weight can make people feel self-conscious and uncomfortable in your own skin. Losing weight can help you to feel more confident and comfortable in your own body
Weight loss can improve your life expectancy. Carrying around extra weight can shorten your lifespan. Losing weight can help you to live a longer, healthier life


#### Research Question
There are many different research questions that could be asked about weight loss. Some examples include:

What are the exercises that has the most impact on weight loss
Does diet have a positive impact on weight loss
With the dataset available, does Age, weight and gender have an impact on weight loss

#### Data Sources
The following datasets will be used for this project:

Fitbit weight data loss dataset from https://www.kaggle.com/datasets/arashnic/fitbit
#### Methodology
The following Machine Learning models will be used:

Linear regression is a statistical method that can be used to understand the relationship between variables that contribute to weight loss, the variables would be exercise and weight loss.


#### Results
Results
Data Visualization
As mentioned above, in exploring the dataset, a number of visualization was created to understand the distribution of weight loss information in the dataset. An example is the chart below that shows the number of steps taken by a Fitbit user during the period of 4/12/2016 to 5/12/2016.

Fitbit User Total Steps taken Over a Month's Period!

The average number of steps for this user is approximately 12,000 and supports the average Calories recorded below.

With the average number of steps above, how does this translates to average number of calories. The chart below shows the number of calories lost by this user over the same period of 4/12/2016 to 5/12/2016.

Fitbit User Calories Lost Over a Month's Period!

This User is a fairly active users over the number of days in the dataset with average of 1816 calories over the number of days above

Finally, a visualization of the final data used to create the ML applications looking at the count of the Calories lost by all 33 Fitbit users.

Count of Calories lost by 33 Fitbit Users in Final Dataset!

The chart shows that largest amount of Calories lost recorded by users at 2,000, a fair distribution of calories lost data from 1,400 to 4,000 which means the ML Application would probably make better predictions for users that have recorded their number of steps and other variables in the data against these calories.



AI Application 1 - ML Regressors
Regressors are a type of ML algorithms that can be used to predict a continuos value. The do this by learning from data (i.e., number of steps taken, total distance etc.) and then using that data to create a model that can make predictions about new data (i.e., number of calories lost)

The application uses variables like Total Distance and No of Steps taken to predict number of calories that a user could lose.

Algorithm: GradientBoostingRegressor

Training Score	85%
Test Score	61%
This algorithm can predict calories loss with an accuracy of over 60%+


#### Next steps
What suggestions do you have for next steps?

#### Outline of project

- https://github.com/Ratanyk/capstone-predicting-weightloss/blob/main/notebooks/predicting-weight-loss-notebook1-linear-regression.ipynb
- https://github.com/Ratanyk/capstone-predicting-weightloss/blob/main/notebooks/predicting-weight-loss-notebook2-decision-tree.ipynb
- https://github.com/Ratanyk/capstone-predicting-weightloss/blob/main/notebooks/predicting-weight-loss-notebook3-comparing-classifiers.ipynb


Recommendations : 

Recommended Model: GradientBoostingRegressor
    - Training accuracy: 86% | Testing accuracy: 61%
    - Strong candidate for predicting calories burned and weight loss potential
    - Performance can be further improved with more diverse and high-activity data (e.g., users with >30k steps/day and >5 miles distance)


Data Collection for Model Enhancement:
    - Lifestyle Metrics: Daily water intake, sleep patterns, and calorie intake (Protein, Carbs, Fats)
    - User Demographics: Age, Gender, Weight, Height, BMI
    - Activity Metrics: Heart rate, active minutes, and step intensity
    - Including these features will help the model capture personalized patterns, improving prediction accuracy


##### Contact and Further Information
Author - Ratan Yalamanchili

Email - myselfratan@gmail.com

