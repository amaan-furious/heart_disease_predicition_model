# ❤️ Heart Disease Prediction using Machine Learning (Logistic Regression)

This project uses **Logistic Regression** to predict whether a person has heart disease based on medical attributes.
It is a simple end-to-end Machine Learning pipeline built using **NumPy, Pandas, and Scikit-Learn**.

---

## 🚀 Project Workflow

### **1️⃣ Importing Dependencies**

The project uses:

* NumPy
* Pandas
* Train-Test Split
* Logistic Regression
* Accuracy Score

---

### **2️⃣ Loading the Dataset**

The dataset is loaded from:

```
/content/data.csv
```

Then the code:

* Shows first & last 5 rows
* Displays dataset shape
* Prints dataset info
* Checks for missing values
* Shows statistical summary
* Checks distribution of the target variable

---

## **3️⃣ Data Preparation**

Features (**X**) and target (**Y**) are separated:

* `X` → all columns except *target*
* `Y` → the *target* column

Then the data is split using:

```
test_size = 0.2  
stratify = Y  
random_state = 2  
```

---

## **4️⃣ Model Training: Logistic Regression**

A Logistic Regression model is trained using:

```python
model = LogisticRegression()
model.fit(X_train, Y_train)
```

---

## **5️⃣ Model Evaluation**

Evaluation includes:

* ✔️ Training Accuracy
* ✔️ Test Accuracy

Using:

```python
accuracy_score(Y_true, Y_pred)
```

---

## **6️⃣ Predicting Heart Disease for New Inputs**

A sample input such as:

```
(62,0,0,140,268,0,0,160,0,3.6,0,2,2)
```

is converted into a numpy array and reshaped before prediction.

Output meanings:

* **0 → No Heart Disease**
* **1 → Heart Disease Present**

---

## 📊 Model Performance

Typical Logistic Regression accuracy:

* **Training Accuracy:** ~84%
* **Test Accuracy:** ~82%

(May vary slightly based on dataset split.)

---

## 🧠 Technologies Used

| Library      | Purpose                      |
| ------------ | ---------------------------- |
| NumPy        | Numerical operations         |
| Pandas       | Data loading & preprocessing |
| Scikit-Learn | ML model, evaluation metrics |

---

## 📁 Project Structure

```
📂 Heart Disease Prediction
│
├── data.csv                # Dataset
├── heart_disease.ipynb     # Notebook (if used)
├── model.py                # Python script (optional)
├── README.md               # Documentation
```

---

## 📝 How to Run the Project

### **Install Dependencies**

```bash
pip install numpy pandas scikit-learn
```

### **Run the Script**

```bash
python model.py
```

Or use Jupyter Notebook / Google Colab.

---

## 💡 Future Improvements

* Add visualizations
* Use advanced ML models (Random Forest, XGBoost, SVM)
* Build a web app using Streamlit/Flask
* Save and load models with pickle

---

## 👨‍💻 Author

A Machine Learning beginner project demonstrating binary classification using Logistic Regression.
