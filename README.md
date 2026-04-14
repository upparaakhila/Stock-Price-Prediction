# 📈 Stock Price Prediction using Linear Regression

## 📌 Overview

This project demonstrates a simple machine learning approach to predict future stock prices using **Linear Regression**.
The model learns the relationship between the current stock price and the future stock price from a dataset.

---

## 🎯 Objective

* To understand basic machine learning concepts
* To implement **Linear Regression** for prediction
* To predict future stock prices based on current values

---

## 🧠 Machine Learning Concept

This project uses **Supervised Learning**, where:

* Input → Current Price
* Output → Future Price

The model learns a relationship:

```
Future Price = m × Current Price + c
```

---

## 🛠️ Technologies Used

* Python 🐍
* Pandas
* NumPy
* Scikit-learn
* Jupyter Notebook / PyCharm

---

## 📂 Dataset

The dataset is a simple CSV file with two columns:

| current_price | future_price |
| ------------- | ------------ |
| 100           | 130          |
| 105           | 135          |
| 110           | 140          |
| ...           | ...          |

---

## ⚙️ How It Works

1. Load dataset using pandas
2. Split data into input (X) and output (y)
3. Train model using Linear Regression
4. Predict future price for a new value
5. Display prediction result

---

## 💻 Code Example

```python
import pandas as pd
from sklearn.linear_model import LinearRegression

# Load dataset
df = pd.read_csv("stockss_predictions.csv")

X = df[["current_price"]]
y = df["future_price"]

model = LinearRegression()
model.fit(X, y)

# Predict
new_price = pd.DataFrame([[125]], columns=["current_price"])
prediction = model.predict(new_price)

print("Predicted Price:", prediction)
```

---

## 📊 Output

```
Predicted Price: [155.]
```

---

## 📈 Result

The model successfully predicts future prices.
It learned a linear relationship:

```
Future Price = Current Price + 30
```

---

## 🚀 Future Improvements

* Use real stock market datasets
* Apply advanced models (Random Forest, LSTM)
* Add visualization (graphs)
* Improve accuracy

---

## 📌 Conclusion

This project shows how machine learning can be used to predict stock prices using a simple linear model. It is a beginner-friendly implementation of regression.

---

## 👨‍💻 Author

**Ruthu Devaraj Poojary**

---

## ⭐ Note

This is a basic project for learning purposes and does not reflect real stock market predictions.
