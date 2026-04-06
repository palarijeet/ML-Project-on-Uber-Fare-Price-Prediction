🚕 Uber Fare Price Prediction (Machine
Learning Project)
📌 Overview
This project focuses on predicting Uber ride fares using Machine Learning. The main objective is to
analyze ride data, perform feature engineering, and build a regression model that can accurately
estimate fare based on trip characteristics.
🎯 Objective
To develop a predictive model that estimates Uber fare price using features such as distance, time,
and ride conditions.
📊 Dataset Description
The dataset contains information about Uber rides including pickup time, location coordinates, and
fare amount.
🔑 Key Features:
• distance in km – Distance between pickup and drop-off locations using Phaversine
formula
• pickup_datetime – Date and time of ride
• passenger_count – Number of passengers
🧠 Engineered Features:
• hour – Hour of the day
• day_of_week – Day index (0–6)
• is_weekend – Weekend indicator (0 or 1)
• part_of_day – Morning / Afternoon / Evening / Night
🧹 Data Preprocessing
• Removed invalid and zero-distance trips
• Filtered unrealistic fare values and extreme outliers
• Converted datetime into useful time-based features
• Applied one-hot encoding for categorical variables
• Ensured clean and structured dataset for modeling
📈 Exploratory Data Analysis (EDA)
• Visualized fare vs distance using scatter plots
• Identified strong positive correlation between distance and fare
• Analyzed impact of time-based features on pricing
• Detected skewness and outliers in the dataset
🤖 Model Used
• Linear Regression (Scikit-learn)
📊 Model Performance
• R² Score: 0.73
• Mean Absolute Error (MAE): ~2.95
• Root Mean Squared Error (RMSE): ~4.85
👉 The model provides a good fit and produces realistic predictions.
🔮 Sample Predictions
Distance
(km) Conditions Predicted
Fare
6 km Evening ₹18.58
10 km Weekend
Evening ₹26.94
15 km Night ₹37.23
🧠 Key Insights
• Distance is the most important feature affecting fare
• Fare increases approximately linearly with distance
• Time-based features have moderate influence
• Passenger count and weekend have minimal impact
• Data cleaning significantly improves model accuracy
🚀 Future Improvements
• Implement advanced models (Random Forest, XGBoost)
• Include real-world factors like traffic and surge pricing
• Deploy the model using Streamlit or Flask
• Improve feature engineering for better accuracy
🛠 Tech Stack
• Python
• Pandas, NumPy
• Matplotlib, Seaborn
• Scikit-learn
📌 Conclusion
This project demonstrates a complete machine learning workflow, including data preprocessing,
feature engineering, visualization, model building, and evaluation. The Linear Regression model
achieved good performance and successfully predicts Uber fares based on input features.
📂 Project Structure
Uber-Fare-Prediction/
│ ├── Uber_Fare_Price_Prediction.ipynb
├── README.md
⭐ Author
Arijeet Pal
📎 Note
This project is built for learning and demonstration purposes as part of a Machine Learning journey.
