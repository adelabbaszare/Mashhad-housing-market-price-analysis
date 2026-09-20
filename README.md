# 🏠 Mashhad Housing Market Price Analysis

![Mashhad Image](https://upload.wikimedia.org/wikipedia/commons/3/3f/Mashhad_City_in_the_morning.jpg)
![Top Language](https://img.shields.io/github/languages/top/adelabbaszare/Mashhad-Housing-Market-Price-Analysis)
![Languages Count](https://img.shields.io/github/languages/count/adelabbaszare/Mashhad-Housing-Market-Price-Analysis)
![Libraries](https://img.shields.io/badge/Pandas-Seaborn-green.svg)

[English](README.md) | [فارسی](README_fa.md)

## 📌 Project Overview

This project performs a comprehensive **Exploratory Data Analysis (EDA)** on apartment sale listings in **Mashhad, Iran**. The primary goal is to understand the key drivers of housing prices and visualize trends related to location, amenities, and property characteristics.

This analysis provides valuable insights for buyers, sellers, and real estate analysts looking to understand the current market dynamics in Mashhad.

## 📂 The Dataset

The analysis is based on the **Mashhad Apartment Sales Data** dataset, published on Kaggle:

**Dataset:** [Mashhad Apartment Sales Data](https://www.kaggle.com/datasets/adelzare/mashhad-apartment-sales-data/data)

The dataset is provided as `mashhad_apartment_sales_2025.csv` and contains **22,403** apartment sale listings with the following features:

| Feature | Description |
| :--- | :--- |
| **neighborhood** | The specific district/area within Mashhad. |
| **area** | Size of the apartment in square meters. |
| **construction_year** | The year the building was constructed (Shamsi calendar). |
| **rooms_count** | Number of bedrooms. |
| **floor** | The floor number of the unit. |
| **total_floors_count** | Total number of floors in the building. |
| **unit_per_floor** | Number of units per floor. |
| **has_elevator** | Boolean: Does the building have an elevator? |
| **has_parking** | Boolean: Does the unit have a parking spot? |
| **has_warehouse** | Boolean: Does the unit have storage/warehouse space? |
| **Price(Toman)** | Listing price in Toman. |
| **Price(USD)** | Listing price converted to USD. |
| **created_at_date** | Listing creation date (Gregorian). |
| **created_at_shamsi** | Listing creation date (Shamsi calendar). |

## 📊 Key Findings & Analysis

The notebook covers the following specific analyses:

### 1. Price Distribution
- **Observation:** The market is right-skewed. The majority of apartments fall within the **1 to 4 billion Toman** range, with very expensive luxury apartments being outliers.

### 2. Price vs. Area
- **Correlation:** There is a strong positive linear relationship between the area (m²) and price. As expected, larger apartments command higher prices.

### 3. Neighborhood Valuation
- **Top Areas:** Analysis was filtered for neighborhoods with significant listings (>50).
- **Most Expensive:** Neighborhoods such as **Sajjad**, **Hashemiyeh**, and **Koh Sangi** emerged as the most expensive areas by average price.

### 4. Impact of Rooms
- **Trend:** The median price increases significantly with the number of rooms. 2 and 3-bedroom apartments show a distinct price jump compared to 1-bedroom units.

### 5. Building Age
- **Density:** The highest volume of transactions occurs for buildings **0–10 years old**.
- **Value:** Newer properties generally hold higher value, with prices gradually depreciating as the building age increases.

### 6. Amenities Impact
- **Elevators:** Apartments with elevators are, on average, almost **twice as expensive** as those without.
- **Parking & Storage:** Both features add significant value to the property price.

## 🛠️ Technologies Used

- **Python 3.x**
- **Pandas & NumPy:** For data manipulation and cleaning.
- **Matplotlib & Seaborn:** For statistical data visualization.

## 🚀 How to Run This Project

1. **Clone the repository:**
   ```bash
   git clone https://github.com/adelabbaszare/Mashhad-Housing-Market-Price-Analysis.git
   cd Mashhad-Housing-Market-Price-Analysis
   ```

2. **Install dependencies:**
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. **Launch Jupyter Notebook:**
   ```bash
   jupyter notebook mashhad-housing-market-prices-analysis.ipynb
   ```

Alternatively, you can view and run the notebook directly on **Kaggle** by visiting the [dataset page](https://www.kaggle.com/code/adelzare/mashhad-housing-market-prices-analysis).

## 📈 Visualizations

*Note: This repository contains the source code to generate the following charts:*

1. **Price Distribution:** Histogram showing the distribution of apartment prices.
2. **Price vs. Area:** Regression plot confirming the strong relationship between area and price.
3. **Top Neighborhoods:** Bar chart of the 20 most expensive neighborhoods (filtered by listings >50).
4. **Price vs. Rooms:** Box plot illustrating how the number of bedrooms affects the median price.
5. **Building Age:** Hexbin plot showing the density of transactions and price trends by building age.
6. **Amenities Impact:** Comparative bar charts showing the added value of elevators, parking, and storage.

## 🤝 Contributing

Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/adelabbaszare/Mashhad-Housing-Market-Price-Analysis/issues).

## 📜 License

This project is open-source and available for use under the MIT License.

---

**Data Source:** [Kaggle - Mashhad Apartment Sales Data](https://www.kaggle.com/datasets/adelzare/mashhad-apartment-sales-data/data)  
**Last Updated:** September 2026
