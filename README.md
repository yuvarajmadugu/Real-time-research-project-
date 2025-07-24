🌾 Real-Time Predictive Crop Yield Estimation
Predicetive Crop Yeild Estimation: Machine Learning Classifier Comparision

📌 Project Overview
The Predictive Crop Yield Estimation project is a real-time machine learning-based system developed as a research initiative to forecast agricultural crop yields. It classifies yield into low, average, and high categories using historical, environmental, and soil-related features. This project integrates two machine learning models—Orthogonal Matching Pursuit and Calibrated Logistic Regression—to explore the balance between interpretability and predictive performance.

- 🎯 Objectives
- 📊 Predict crop yield class (low, average, high) in real-time
- 🤖 Train and evaluate two classifiers:
-     Orthogonal Matching Pursuit (OMP)
-     Calibrated Logistic Regression
- 📈 Evaluate models using accuracy, precision, recall, and F1-score
- 📦 Save and reuse trained models to avoid retraining every time
- 🧪 Display predictions and insights for unseen test data

🧪 Dataset
- The dataset includes:
    Soil properties
    Rainfall
    Temperature
    Humidity
    Region-specific features
- Target variable: yield_class (Categorical: low, average, high)

📊 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix
- Classification Report
Example evaluation of CalibratedClassifier:
Accuracy    : 97.98%
Precision   : 98.05%
Recall      : 97.99%
F1-Score    : 97.97%
📌 Note: These metrics are visualized using Seaborn and Matplotlib.

📈 Visualization
- Count plot of yield classes
- Confusion matrix heatmap
- Class-wise precision, recall, F1
    sns.countplot(x=df['yield_class'], palette="Set3")
    sns.heatmap(conf_matrix, annot=True, cmap="Blues")
  
🛠️ How to Run
1. Install dependencies
    pip install -r requirements.txt
2. Train the models
    python src/train_models.py
3. Run evaluation and visualization
    python src/evaluate.py
4. Predict on new test data
    python src/predict.py
   
🔮 Sample Output (Prediction)
  Model Predicted of Row 0 Test Data is ---> average yield
  Model Predicted of Row 1 Test Data is ---> low yield
  Model Predicted of Row 2 Test Data is ---> high yield
  
✅ Dependencies
  numpy
  pandas
  scikit-learn
  matplotlib
  seaborn
Add them to requirements.txt as needed.

🤝 Contributions
- This project is open for improvements and contributions:
- Improve model accuracy with more features
- Add ensemble models or deep learning
- Integrate real-time sensor/IoT data

📬 Contact
- Author: Yuvaraj Madugu
- Email: 22ra1a6697@kpritech.ac.in
- LinkedIn: linkedin.com/in/yuvarajmadugu
- GitHub: github.com/yuvarajmadugu

📜 License
- This project is licensed under the SAK Informatics.
