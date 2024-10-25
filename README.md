# Brazilian E-commerce Data Analysis

This project analyzes e-commerce data from Brazil, exploring insights on customer orders, payments, products, and delivery patterns.

## Table of Contents
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Installation](#installation)
- [Data Loading and Exploration](#data-loading-and-exploration)
- [Analysis](#analysis)
  - [Basic Analysis](#basic-analysis)
  - [Time-Based Analysis](#time-based-analysis)
- [Future Work](#future-work)
- [Contributing](#contributing)

## Project Overview
This analysis is based on a dataset from Kaggle covering Brazilian e-commerce data. The main objectives are to understand order trends, customer behavior, and payment methods.

## Data Source
- Dataset: [Brazilian E-commerce on Kaggle](https://www.kaggle.com/datasets/olistbr/brazilian-ecommerce)

## Installation
To run this project in Google Colab, install Kaggle's API and upload your Kaggle credentials.



```python
# Install Kaggle API
!pip install -q kaggle

# Upload kaggle.json file
from google.colab import files
files.upload()  # Upload your kaggle.json

# Set up kaggle.json
!mkdir -p ~/.kaggle
!cp kaggle.json ~/.kaggle/
!chmod 600 ~/.kaggle/kaggle.json

# Download the dataset
!kaggle datasets download -d olistbr/brazilian-ecommerce
!unzip brazilian-ecommerce.zip
```
## Data Loading and Exploration
The project loads the following five datasets:

- `olist_orders_dataset.csv`
- `olist_customers_dataset.csv`
- `olist_order_items_dataset.csv`
- `olist_products_dataset.csv`
- `olist_order_payments_dataset.csv`

For each dataset, basic information is displayed, including shape, sample rows, and any missing values.

## Analysis

### Basic Analysis
- **Order Status Distribution**: Visualized as a bar chart.
- **Payment Types**: Frequency of each payment type is analyzed.
- **Average Order Value**: The mean order value is calculated.

### Time-Based Analysis
- **Monthly Orders**: Monthly trends in orders over time, visualized with a line chart.

## Future Work
Potential future analyses include:
- Customer segmentation
- Product category analysis
- Geographical analysis
- Delivery performance analysis

## Contributing
Contributions are welcome! Please feel free to open issues or submit pull requests.

