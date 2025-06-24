# Smart Lender - Applicant Credibility Prediction for Loan Approval

Smart Lender is an Machine Learning based web application that predicts whether a loan application is likely to be approved or rejected based on user-inputted financial and demographic details. It combines machine learning with a sleek user interface to provide real-time, reliable insights for applicants and lenders alike.

## 🔗 Website Link

**[Click here!]()**

## 🔍 Features

- Machine Learning prediction using Random Forest
- Clean, responsive HTML/CSS frontend with JS validation
- Flask-based backend integration
- Dynamic result display for approved or rejected applications
- Consistent and user-friendly interface

## 🧠 Model Information

The application uses a **Random Forest Classifier**, chosen for its:

- Strong performance in both accuracy and F1 score
- Robustness to overfitting
- Ability to handle both categorical and numerical features
- High interpretability for business decision making

> Final Model Stats:  
> - F1 Score: **0.8221**  
> - Accuracy: **0.8125**  
> - Cross-validation Accuracy: **0.8107**  

## 🛠️ Tech Stack

- **Frontend**: HTML, CSS (modern minimal design), JavaScript
- **Backend**: Python Flask
- **ML Libraries**: Scikit-learn, NumPy, Pandas
- **Model**: RandomForestClassifier with Hyperparameter Tuning
- **Deployment**: Runs locally via Flask, hosted using like Render

## 📁 Project Structure

```
5. Project Executable Files/
│
├── app/
│   ├── app.py                # Flask backend
│   ├── templates/
│   │   ├── index.html        # Homepage
│   │   ├── form.html         # User form
│   │   └── submit.html       # Prediction result page
│   ├── static/
│   │   ├── styles.css        # Global styling
│   │   └── assets/           # Images (logo, icons, etc.)
│
├── model/
│   ├── random_forest_model.pkl   # Saved model
│   └── scaler.pkl                # Saved scaler
│
├── src/
│   └── train_model.py        # Model training and tuning
│
|
|__ notebooks/
|     └── eda.ipynb        # Data visualization and analysis
|
|
|___ requirements.txt         # Liraries required before execution
|
|
└── README.md
```

## 🚀 How to Run Locally

1. **Clone the repository**:
   ```bash
   git clone <your-repo-url>
   cd Project/app
   ```

2. **Create virtual environment**:
   ```bash
   python -m venv venv
   venv\Scripts\activate  # On Windows
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the app**:
   ```bash
   python app/app.py
   ```

5. Open `http://127.0.0.1:5000/` in your browser.

## ✅ Inputs Used for Prediction

- Gender
- Marital Status
- Dependents
- Education
- Self Employment
- Applicant Income
- Co-applicant Income
- Loan Amount & Term
- Credit History
- Property Area

## 📌 Notes

- The ML model uses one-hot encoding and scaling for preprocessing.
- Make sure model files (`.pkl`) are in the correct path (`../model/` relative to app.py).
- Static assets and CSS are shared across all pages.

## 📄 License

This project is for educational purposes only. All rights reserved.

## 🙌 Credits

Developed by [Yash Chugani](https://github.com/YashChugani), [Yash Dharad](), and [Aashish Kumar Mandhyani]().
Machine Learning logic, design, and full-stack integration by the developer  
