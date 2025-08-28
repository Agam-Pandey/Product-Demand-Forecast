### 📝 Project Overview

This repository contains a Jupyter notebook that demonstrates a product demand forecasting project using an LSTM model. The notebook includes a complete workflow from data loading and cleaning to exploratory data analysis (EDA), visualization, and model building. The primary objective is to predict future product demand based on historical order data.

### 📊 Exploratory Data Analysis (EDA)

The notebook begins with an in-depth analysis of the dataset, which includes information on `ProductCode`, `Warehouse`, `ProductCategory`, `Date`, and `OrderDemand`. Key insights from the EDA are:

  * **Data Cleaning**: Missing values in the `Date` column were dropped, and parentheses were removed from the `OrderDemand` column, which was then converted to an integer data type.
  * **Time Series Analysis**: The project analyzes the trends in order demand over time. A time-series plot shows the total order demand from 2012 to 2016. Monthly and yearly patterns are also visualized, revealing potential seasonality or growth trends.
  * **Categorical Variables**: The notebook explores the distribution of products across different warehouses and product categories. The `Whse_J` warehouse is shown to have the highest number of samples, while `Category_019` is the most frequent product category.

### 🧠 Methodology

The project uses a **Long Short-Term Memory (LSTM)** network, a type of recurrent neural network (RNN) well-suited for time-series forecasting. The model is built using the Keras library, and the data is preprocessed using `MinMaxScaler` from scikit-learn for optimal model performance. The model architecture consists of LSTM and Dense layers with Dropout for regularization.

### 💻 Installation

To run this project, you will need to install the following Python libraries:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn keras tensorflow
```

### 🚀 Usage

1.  Clone this repository:
    ```bash
    git clone https://github.com/Agam-Pandey/Product-Demand-Forecast
    ```
2.  Open the `forecast-product-demand-with-lstm.ipynb` notebook in a Jupyter environment.
3.  Execute the cells sequentially to reproduce the data analysis and run the LSTM forecasting model.

-----
