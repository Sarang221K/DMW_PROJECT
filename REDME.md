
# Zomato Restaurant Rating Prediction

## **Objective**
The objective of this project is to predict restaurant ratings based on features such as location, cost, online order availability, booking options, and type. This prediction model can be valuable for both customers who want to explore restaurants with high ratings and for restaurant managers aiming to improve their services.

## **Overview**
The dataset used in this project contains various attributes related to restaurants, including their location, average cost, online order availability, restaurant type, cuisines offered, and more. By using machine learning techniques, we aim to develop a model that predicts restaurant ratings.

## **Key Features**
- **Location**: The city or area where the restaurant is located.
- **Average Cost**: The estimated cost for two people to dine.
- **Online Order Availability**: Whether the restaurant provides an option to order food online.
- **Restaurant Type**: Type of restaurant (e.g., Pub, Dine-out, Buffet, etc.).
- **Cuisines**: The types of food served by the restaurant.

## **Approach**
1. **Data Preprocessing**:
   - Handle missing data.
   - Encode categorical variables using label encoding.
   - Remove duplicate entries.
   - Clean the data (e.g., remove commas in the 'average cost' column).
   
2. **Exploratory Data Analysis (EDA)**:
   - Visualize distribution of various features.
   - Examine correlations between features.
   - Perform feature importance analysis.

3. **Modeling**:
   - **Linear Regression**: To get a baseline performance.
   - **Decision Tree Regression**: To capture non-linear relationships.
   - **Random Forest Regression**: To improve accuracy and reduce overfitting.
   - **Extra Trees Regressor**: For faster training and better performance.

4. **Evaluation**:
   - Evaluate models based on the R-squared value to assess how well the model predicts restaurant ratings.

## **Installation Instructions**

To run this project, follow these steps:

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/zomato-rating-prediction.git
cd zomato-rating-prediction
```

### 2. Install Required Libraries
Create a virtual environment and install dependencies:

```bash
pip install -r requirements.txt
```

If you don't have `requirements.txt` yet, here's a sample list of packages to include:
```txt
pandas
numpy
matplotlib
seaborn
scikit-learn
```

### 3. Run the Jupyter Notebook
Open and run the Jupyter notebook in your preferred environment:

```bash
jupyter notebook
```

Navigate to the notebook file `Zomato_Rating_Prediction.ipynb` to execute the project step by step.

## **Project Structure**

```
zomato-rating-prediction/
├── Zomato_Rating_Prediction.ipynb  # Jupyter notebook with the implementation
├── data/                           # Folder containing the Zomato dataset (zomato.csv)
├── requirements.txt                # List of required Python packages
├── README.md                       # Project documentation
└── images/                         # Folder with any visualizations or charts
```

## **Results**
- The final model provides predictions of restaurant ratings based on various features.
- The **Decision Tree Regression** model performed the best with an **R-squared value of 0.85**, indicating that it explains 85% of the variance in the restaurant ratings.

## **Conclusion**
The model demonstrates that **restaurant features** like **location**, **cost**, **restaurant type**, and **online ordering availability** are important factors in predicting restaurant ratings. The model can be used by customers to choose restaurants based on predicted ratings and can help restaurant managers identify areas of improvement.

## **Future Work**
- Experiment with more advanced models like **Gradient Boosting** or **XGBoost** for potentially better results.
- Incorporate additional features like customer reviews, operating hours, or seasonal changes.
- Deploy the model as a web application to provide real-time predictions for users.

## **Acknowledgments**
- The dataset is sourced from Zomato (available on Kaggle).
- Special thanks to the community for their contributions to open-source libraries like Scikit-learn, Pandas, and Seaborn.

---