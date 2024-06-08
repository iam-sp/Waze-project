# Waze-project

**Project Overview**

Waze’s free navigation app makes it easier for drivers around the world to get to where they want to go. Waze’s community of map editors, beta testers, translators, partners, and users helps make each drive better and safer. Waze partners with cities, transportation authorities, broadcasters, businesses, and first responders to help as many people as possible travel more efficiently and safely.

Waze leadership has asked our data team to develop a machine learning model to predict user churn. Churn quantifies the number of users who have uninstalled the Waze app or stopped using the app. This project focuses on monthly user churn. An accurate model will help prevent churn, improve user retention, and grow Waze’s business.

**Business Understanding**

This project is part of a larger effort at Waze to increase growth. Developing a churn prediction model will help prevent churn, improve user retention, and grow Waze’s business. An accurate model can also help identify specific factors that contribute to churn.

If Waze can identify a segment of users who are at high risk of churning, Waze can proactively engage these users with special offers to try and retain them. Otherwise, Waze may simply lose these users without knowing why.

**Data Understanding**

This is a project from the Google Advanced Data Analytics course which has been developed in collaboration with Waze. The dataset was created for pedagogical purposes and does not represent Waze’s actual data.

**Modeling and Evaluation**

Logistic Regression was carried out initially but the result was not satisfactory. The team has subsequently decided to use another 2 models: Random Forest and XGBoost model.

Data was split into training, validation, and test sets. Splitting the data three ways means that there is less data available to train the model than splitting just two ways. Performing model selection on a separate validation set enables testing of the champion model by itself on the test set, which gives a better estimate of future performance than splitting the data two ways and selecting a champion model by performance on the test data.

**Conclusion**

Engineered features accounted for six of the top 10 features: km_per_hour, percent_sessions_in_last_month, total_sessions_per_day, percent_of_drives_to_favorite, km_per_drive, km_per_driving_day.

The XGBoost model fit the data better than the random forest model.

This modeling effort confirms that the current data is insufficient to consistently predict churn. It would be helpful to have drive-level information for each user (such as drive times, geographic locations, etc.). It would probably also be helpful to have more granular data to know how users interact with the app. For example, how often do they report or confirm road hazard alerts? Finally, it could be helpful to know the monthly count of unique starting and ending locations each driver inputs.
