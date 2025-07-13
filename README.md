# Prediction-of-Product-Sales

## Histograms to view the distributions of Item_Weight feature:
![Item_Weight](https://github.com/user-attachments/assets/017afd32-81fa-4cf3-bef8-5b31db4cc55b)
- we notice that the wigths of the product are distrebuted from 5 to 20 kg with the most common value at 7.5 kg

## Histograms to view the distributions of Item_Visibility feature:
![Item_Visibility](https://github.com/user-attachments/assets/df6bdfd4-732f-43c3-bb87-1236bf3f19e2)
- we notice that the Item_Visibility of the product are distrebuted from 0.0 to 0.328  with the most common value at 0.03 , the product count is the lowest at the highest Item_Visibility


## Boxplots to view statistical summaries of Item_Weight feature :
![Item_Weight_box](https://github.com/user-attachments/assets/e1eccb04-3ffb-416f-a34d-435fbee64792)
- we notice that the Item Wight has min at 5 and max at 25 with median at 13 with first quater at 9 and therd quater at 16 with iqr == 7 with good destripition of the value.

## Boxplots to view statistical summaries of Item_Visibility feature :
![Item_Visibility_box](https://github.com/user-attachments/assets/973d49ad-9370-4e33-ad6b-d7fbe70bf788)
- we notice that the Item_Visibility has min at 0 and max at 0.2 with median at 0.05 with first quater at 0.03 and therd quater at 0.01 with bad destripition of the value and many outliars .

## Countplots to view the frequency of each class of Item_Fat_Content feature in your dataset:
![Item_Fat_Content](https://github.com/user-attachments/assets/38f93b1c-01cf-4645-b08b-e3fb585835e6)
- we notice that the products with low fat has large count from the regural prouduct.

## Countplots to view the frequency of each class of Outlet_Type feature in your dataset:
![Outlet_Type](https://github.com/user-attachments/assets/4c49443e-c303-46aa-9b7f-23b37273fca0)
- we notice that the most common value is supermarket type1 with 6000 and the lost value is in  supermarket type2 .

## Heatmap to view the correlation between features:
![Heatmap](https://github.com/user-attachments/assets/adcf7d31-1871-4686-9f91-53637637b9ae)
- we notice that the correlation is intermediate positive correlation between item_outer_sale and item_mrp with 0.57 correlation and the rest of the feature dont have any relation betwwen them at all  .


# Predicting Retail Product Sales to Improve Stock Planning
## A machine learning solution for forecasting sales volume based on product and store attributes

**Author**: Feras Hani Alnahhal  
**Contact**: ferasnahhal2001@gmail.com

---

### 🧩 Business Problem:

Retailers need reliable sales forecasts to optimize inventory levels, minimize stockouts, and avoid overstock. This project aims to predict the **Item Outlet Sales** for different products across various store types using machine learning. The objective is to build a model that helps business stakeholders make data-driven decisions regarding stock planning and distribution.

---

### 📦 Data:

- **Source**: BigMart Sales Dataset  
- **Observations**: 8,523 rows  
- **Features**: 11 features related to items and outlet characteristics (e.g., Item_Type, Item_MRP, Outlet_Type, Item_Visibility, etc.)

The data includes product-level and store-level attributes and the sales target variable: `Item_Outlet_Sales`.

---

## 🔧 Methods

- **Data Cleaning**: Handled missing values in `Item_Weight` and `Outlet_Size` using imputation.
- **Feature Engineering**: Encoded categorical variables using OneHotEncoder.
- **Scaling**: Applied StandardScaler for numerical features where needed.
- **Modeling**: Trained and evaluated multiple regression models.
- **Validation**: Used R² Score, RMSE, and MAE as evaluation metrics.

---

## 📊 Results

### Insight 1: Item MRP Strongly Influences Sales
![MRP vs Sales](images/mrp_vs_sales.png)

> Higher-priced items tend to generate higher sales, suggesting price tier plays a crucial role in demand prediction.

---

### Insight 2: Store Type Impacts Performance
![Outlet Type Sales](images/outlet_type_sales.png)

> **Supermarket Type 3** consistently outperforms other outlet types in total sales, which may indicate better marketing, store size, or foot traffic.

---

## 🤖 Model

- **Best Model**: Random Forest Regressor
- **Evaluation Metrics**:
  - **R² Score**: 0.63
  - **RMSE**: 1104.78
  - **MAE**: 845.55

The model captures complex, non-linear patterns in the data, making it suitable for generalizing across different product categories and outlet types.

---

## ✅ Recommendations

- Focus inventory and marketing efforts on **high-MRP items** at **Supermarket Type 3** locations.
- Use the model to dynamically adjust stock levels based on sales predictions per product and outlet.
- Integrate this model into a real-time dashboard for store managers.

---

## ⚠️ Limitations & Next Steps

- Model performance can be further improved by including external factors such as **seasonality**, **promotions**, and **regional demand**.
- Future work should explore time-series modeling for better long-term forecasting.
- Deploy the model as a web app or dashboard for non-technical business stakeholders.

---

### 📫 For Further Information

If you have questions or want to explore the technical notebook:

- Check the notebook: [`sales_prediction.ipynb`](sales_prediction.ipynb)
- Contact the author: **ferasnahhal2001@gmail.com**



  

  

  
  





