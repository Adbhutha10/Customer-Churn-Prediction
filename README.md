# Customer Churn Prediction Application 🚀

An end-to-end Machine Learning platform designed to predict e-commerce customer churn. Featuring a robust Flask backend and an interactive web UI, the system analyzes behavioral metrics like tenure, satisfaction, and order history to generate real-time risk probabilities, empowering businesses to drive proactive and data-driven retention strategies.

---

## 📌 Table of Contents
- [Overview](#overview)
- [Key Features](#key-features)
- [Technology Stack](#technology-stack)
- [Dataset Information](#dataset-information)
- [Project Structure](#project-structure)
- [Installation & Setup](#installation--setup)
- [Application Interfaces](#application-interfaces)

---

## 🌐 Overview
Creating accurate churn prediction models involves using historical customer interaction data to forecast the likelihood of a customer leaving a service or platform. This application focuses on an e-commerce case study where predicting customer churn allows the business to launch highly targeted marketing campaigns and optimize resource allocation.

---

## ✨ Key Features
- **Real-Time Inference Engine**: Instantly calculates churn probabilities via a pre-trained Scikit-learn model.
- **Dynamic Web Interface**: Clean, responsive, Bootstrap-powered HTML forms for easy metric input.
- **One-Hot Metadata Mapping**: Automatically processes and maps categorical inputs into model-ready numerical formats via a robust `.json` schema.
- **Server API**: Server-side processing utilizing Python and Flask to validate incoming POST requests and execute algorithmic predictions.

---

## 🛠️ Technology Stack
- **Backend**: Python 3.13, Flask, Werkzeug
- **Machine Learning**: Scikit-learn, Pandas, NumPy
- **Frontend**: HTML5, CSS3, Bootstrap 4
- **Serialization**: Pickle (`.pkl` Model Weights), JSON (`.json` Feature Schema)

---

## 📊 Dataset Information
[**Original Dataset Source Explorer**](https://www.kaggle.com/datasets/ankitverma2010/ecommerce-customer-churn-analysis-and-prediction/data)

The predictive model was trained on historical e-commerce interactions containing the following features:

| Feature Name               | Description                                                                        |
|----------------------------|------------------------------------------------------------------------------------|
| CustomerID                 | Unique customer ID                                                                 |
| Churn                      | Flag indicating whether the customer churned (1) or not (0)                        |
| Tenure                     | Tenure of the customer in the organization                                          |
| PreferredLoginDevice       | The preferred device used by the customer to log in (e.g., mobile, web)            |
| CityTier                   | City tier classification (e.g., Tier 1, Tier 2, Tier 3)                            |
| WarehouseToHome            | Distance between the warehouse and the customer’s home                             |
| PreferredPaymentMode       | Preferred payment method used by the customer (e.g., credit card, debit card, cash on delivery) |
| Gender                     | The gender of the customer                                                         |
| HourSpendOnApp             | Number of hours spent on the mobile application or website                         |
| NumberOfDeviceRegistered   | Total number of devices registered to the customer’s account                       |
| PreferedOrderCat           | Preferred order category of the customer in the last month                         |
| SatisfactionScore          | Customer’s satisfaction score with the service                                     |
| MaritalStatus              | Marital status of the customer                                                     |
| NumberOfAddress            | Total number of addresses added to the customer’s account                          |
| OrderAmountHikeFromlastYear| Percentage increase in order value compared to last year                           |
| CouponUsed                 | Total number of coupons used by the customer in the last month                     |
| OrderCount                 | Total number of orders placed by the customer in the last month                    |
| DaySinceLastOrder          | Number of days since the customer’s last order                                     |
| CashbackAmount             | Average cashback received by the customer in the last month                        |

---

## 📂 Project Structure

```text
customer-churn-prediction-application/
│
├── end_to_end_deployment/
│   ├── app.py                     # Main Flask Application controller
│   ├── requirements.txt           # Python environment dependencies
│   ├── models/
│   │   ├── churn_prediction_model.pkl # Serialized Machine Learning Model
│   │   └── columns.json           # Data schema for one-hot mapping
│   ├── static/
│   │   └── img/                   # Static assets and icons
│   └── templates/                 # HTML5 UI components
│       ├── index.html             # Client-side data input form
│       └── result.html            # Server-rendered prediction dashboard
├── README.md                      # Detailed project documentation
└── requirements.txt               # Updated python 3.13 dependencies
```

---

## 🚀 Installation & Setup

Follow these steps to run the application securely on your local development server:

1. **Navigate to the Directory**:
   Open your terminal/command prompt and ensure you are in the project root:
   ```bash
   cd customer-churn-prediction-application
   ```

2. **Create a Virtual Environment**:
   It is highly recommended to use a virtual environment to manage dependencies:
   ```bash
   python -m venv .venv
   # Windows:
   .venv\Scripts\activate
   # Mac/Linux:
   source .venv/bin/activate
   ```

3. **Install Dependencies**:
   Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

4. **Launch the Flask Server**:
   Start the application:
   ```bash
   python end_to_end_deployment/app.py
   ```

5. **Interact via Web Browser**:
   Open a browser (Chrome, Firefox, etc.) and navigate to the local development server: `http://127.0.0.1:5000`

---


