# Hotel Booking Cancellation Prediction

## Project Overview

This project builds an end-to-end machine learning workflow to predict whether a hotel reservation will be cancelled.

The goal is to use booking related features to classify each booking as either cancelled or not cancelled. This type of model could help hotels identify bookings with a higher cancellation risk and make better decisions around staffing, room availability, overbooking, and customer follow-up.

This project was completed as my final project for the Codecademy Machine Learning course.

---

## Dataset

The dataset is the Hotel Booking Cancellation Prediction dataset from Kaggle (found at https://www.kaggle.com/datasets/youssefaboelwafa/hotel-booking-cancellation-prediction?resource=download).
The dataset contains hotel reservation records with numerical and categorical features:

- Number of adults and children
- Number of weekend and week nights
- Meal plan
- Room type
- Lead time
- Market segment
- Previous cancellations
- Average price
- Special requests
- Booking status

The target variable is booking_status.

## Installation and setup 

First, clone the repository:
```bash
 git clone https://github.com/LiamOB96/hotel-booking-cancellation-prediction.git
 cd hotel-booking-cancellation-prediction
 ```

Next, the simplest method is to use Anaconda Navigator. Open Anaconda Navigator and launch Jupyter Notebook. Open final_project.ipynb. Run the notebook cells from top to bottom.

## Project Summary

The project follows an end-to-end machine learning workflow:

- Exploratory data analysis
- Data cleaning and feature engineering
- Train-validation-test split
- Preprocessing 
- Model comparison
- Hyperparameter tuning
- Final model evaluation

The models tested were:

- Logistic Regression
- Decision Tree
- Random Forest
- Gradient Boosting

The final selected model was a Random Forest classifier.

## Results

The final model achieved strong performance on the test set.

| Metric | Score |
|---|---:|
| Accuracy | 0.903 |
| Precision | 0.879 |
| Recall | 0.818 |
| F1-score | 0.848 |
| ROC-AUC | Add your ROC-AUC here |

The confusion matrix showed that the model correctly identified most cancelled and non-cancelled bookings, with a reasonable balance between false positives and false negatives.

## Key Takeaways

- Bookings with longer lead times were more likely to be cancelled.
- Bookings with more special requests were less likely to be cancelled.
- Market segment type appeared useful for predicting cancellation behaviour.
- Random Forest performed best overall.
- Hyperparameter tuning did not improve the model in this case.