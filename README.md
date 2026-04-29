✴︎ Customer Satisfaction Prediction (ML Project)

Customer satisfaction plays a huge role in the success of any business. In this project, I tried to understand what actually makes customers happy by using machine learning on real-world e-commerce data.

---

✴︎ What this project is about

The goal of this project is simple — predict how satisfied a customer is (review score) based on factors like delivery time and product price.

At the same time, I also wanted to figure out which factors influence customer satisfaction the most.

---

✴︎ Dataset

For this project, I used the **Olist Brazilian E-commerce dataset** from Kaggle.

🔗 https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce
Files used:
- olist_customers_dataset.csv
- olist_orders_dataset.csv
- olist_order_reviews_dataset.csv
- olist_order_items_dataset.csv
- olist_products_dataset.csv

Instead of relying on a single dataset, I combined multiple datasets to get a better understanding:

* Customers → basic customer details
* Orders → order information
* Reviews → customer ratings
* Order Items → pricing details

Merging these datasets helped create a more complete picture for analysis.

---

✴︎ Approach

I followed a step-by-step machine learning workflow:

* Cleaned the data and handled missing values
* Converted date columns into proper format
* Created a new feature called **delivery time** (this turned out to be very important)
* Selected relevant features like delivery time and price
* Trained multiple models and compared their performance

---

✴︎ Models Used

I experimented with a few regression models:

* Linear Regression
* Decision Tree Regressor
* Random Forest Regressor

Among these, **Random Forest gave the best results**.

---

✴︎ Results (RMSE)

| Model             | RMSE       |
| ----------------- | ---------- |
| Linear Regression | 1.5190496535856457 |
| Decision Tree     | 1.817060573382404 |
| Random Forest     | 1.5878003600720056 |

Linear Regression performed best with the lowest RMSE, indicating that the relationship between features and customer satisfaction is relatively linear.
This suggests that simpler models can sometimes outperform complex models when the data has a linear pattern and limited features.

---

✴︎ Key Insights

Here’s what I found from the analysis:

* Delivery time has a major impact on customer satisfaction
* Faster delivery generally leads to better ratings
* Price does have an effect, but not as much as delivery speed
* Delayed orders are one of the main reasons for low ratings

---

✴︎ Business Takeaways

Based on these results, businesses should:

* Focus on reducing delivery delays
* Improve logistics and order tracking
* Pay special attention to customers facing late deliveries

---

✴︎ Limitations

This project uses only a limited number of features.
It doesn’t consider factors like weather conditions, traffic, or customer behavior patterns.

---

✴︎ Future Improvements

This project can be improved further by:

* Adding more datasets like seller and payment data
* Trying advanced models like XGBoost or Neural Networks
* Deploying it as a real-time prediction system

---

✴︎ Tech Stack

* Python
* Pandas, NumPy
* Scikit-learn
* Matplotlib, Seaborn
* Jupyter Notebook
* 
---

✴︎ Final Note

This project helped me understand how data can be used to solve real business problems.
Even simple features like delivery time can provide powerful insights when analyzed properly.
