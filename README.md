TASK 3: Data Visualization

Objective

The objective of Task 3 is to transform raw data into meaningful visual representations using data visualization techniques. 
Visualizations help in understanding patterns, trends, and distributions in data,
making it easier to derive insights and support decision-making.

Tools & Technologies Used

Python

Pandas – Data handling and preprocessing

Matplotlib – Creating basic visualizations

Seaborn – Statistical data visualization

Jupyter Notebook 


Dataset Description

The dataset contains product-related information such as:

title – Product name

price – Product price

instock – Product availability status


The dataset used in this task was previously cleaned and explored during Task 2: Exploratory Data Analysis (EDA).


🔄 Steps Performed

1️⃣ Data Loading

The dataset was loaded using Pandas for visualization.

import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

df = pd.read_excel("Book_scrap.xlsx")


---

2️⃣ Price Distribution Visualization (Histogram)

A histogram was created to understand the distribution of product prices.

plt.figure()
plt.hist(df['Price'], bins=20)
plt.xlabel("Price")
plt.ylabel("Frequency")
plt.title("Distribution of Product Prices")
plt.show()

📊 Purpose:

To analyze how prices are distributed

To identify common price ranges

To detect any skewness or unusual patterns



3️⃣ Stock Availability Visualization (Count Plot)

A count plot was used to compare in-stock and out-of-stock products.

sns.countplot(x='instock', data=df)
plt.title("Product Availability Status")
plt.show()

📊 Purpose:

To understand inventory distribution

To compare product availability clearly



📈 Key Insights

Most products fall within a specific price range, indicating standard pricing behavior.

The histogram makes it easy to identify price concentration.

The count plot shows that a majority of products are available in stock.

Visualizations simplify complex data and improve clarity.
