# Megaline_Machine_Learning_Project
Develop a model that picks the correct plan for Megaline's legacy customers.

# Introduction
In this project, we will work with a dataset from a mobile network company named Megaline Mobile. Their main concern is about the number of customers still using their old plan. They are aiming to create a model that can analyze customer behavior and recommend to them either Smart or Ultra packages.

The dataset provided to use contains data on customer behavior, specifically the ones who have already made the switch to new packages from a previous statistical data analysis project. We will develop a model that can accurately choose the appropriate package for each customer. Our primary goal is to achieve a high accuracy level with the minimum set at 75%.

# Data Description

- `сalls` — number of calls,
- `minutes` — total call duration in minutes,
- `messages` — number of text messages,
- `mb_used` — Internet traffic used in MB,
- `is_ultra` — plan for the current month (Ultra - 1, Smart - 0).

# Conclusion
The model performs well for the Smart (0) class with high precision (83%) and recall (94%). This means it's good at identifying Smart users and has a low false negative rate for this class.

For the Ultra (1) class, the model has lower recall (56%) compared to precision (82%). This indicates that while the model is relatively good at identifying Ultra users when it makes a prediction, it misses a significant portion of them.

The model achieves an overall accuracy of 83%, which is good. However, the lower recall for Ultra (1) suggests that the model might not be performing as well in identifying all instances of the Ultra class.

The best model is the RandomForrestClassifier with an accuracy of 83%.
Best Param {'n_estimators': 100, 'max_depth': 10, 'min_samples_split': 5}
