# Bank-Customer-Churn-Model-Final-Project-YBI-Foundation
### Using a .ipynb File in Google Colab or Jupyter Notebook:

1. **Upload the `.ipynb` File:**
   - Upload the `.ipynb` file with your notebook code to your Google Drive.

2. **Access the File in Google Colab:**
   - In Google Colab, mount your Google Drive to access the uploaded file using the following code:

   ```python
   from google.colab import drive
   drive.mount('/content/drive')

### Models Trained on Raw Data:

1. **Before Hyperparameter Tuning:**
   - **Model 1:**
     - Precision: 0.84 (class 0), 0.84 (class 1)
     - Recall: 0.99 (class 0), 0.22 (class 1)
     - F1-score: 0.91 (class 0), 0.34 (class 1)

2. **After Hyperparameter Tuning:**
   - **Model 2:**
     - Precision: 0.89 (class 0), 0.45 (class 1)
     - Recall: 0.84 (class 0), 0.56 (class 1)
     - F1-score: 0.86 (class 0), 0.50 (class 1)

### Models with Sampling Techniques:

1. **Random Under Sampling:**
   - **Before Hyperparameter Tuning:**
     - Precision: 0.69 (class 0), 0.70 (class 1)
     - Recall: 0.73 (class 0), 0.66 (class 1)
     - F1-score: 0.71 (class 0), 0.68 (class 1)
   - **After Hyperparameter Tuning:**
     - Precision: 0.69 (class 0), 0.70 (class 1)
     - Recall: 0.74 (class 0), 0.65 (class 1)
     - F1-score: 0.71 (class 0), 0.68 (class 1)

2. **Random Over Sampling:**
   - **Before Hyperparameter Tuning:**
     - Precision: 0.71 (class 0), 0.74 (class 1)
     - Recall: 0.76 (class 0), 0.69 (class 1)
     - F1-score: 0.73 (class 0), 0.72 (class 1)
   - **After Hyperparameter Tuning:**
     - Precision: 0.96 (class 0), 0.86 (class 1)
     - Recall: 0.84 (class 0), 0.96 (class 1)
     - F1-score: 0.89 (class 0), 0.91 (class 1)

### Observations and Conclusion:

- **Raw Data Models:** Hyperparameter tuning might not always lead to improved performance, as seen in Model 2.
  
- **Sampling Techniques:** Both random under sampling and over sampling, coupled with hyperparameter tuning, didn't notably alter the models' performance in this scenario.

- **Best Performing Model:** The model using random over sampling after hyperparameter tuning seems to perform the best, displaying substantially improved metrics for both classes with notably high precision, recall, and F1-scores, resulting in a higher overall accuracy of 90%.
