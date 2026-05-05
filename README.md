# Superstore Data Analysis Project

## Project Overview
This project performs comprehensive data analysis on Superstore sales data using Python and Jupyter Notebook. The analysis includes data cleaning, exploratory data analysis (EDA), statistical correlation analysis, customer segmentation, and time series trend analysis.

## Objective
To analyze Superstore sales data and derive meaningful business insights including:
- Category-wise sales and profit distribution
- Monthly and yearly sales trends
- Impact of discounts on profitability
- Customer segment analysis and performance
- Time series trends to identify growth patterns

## Dataset Information
**File:** `Superstore.csv`

### Columns:
- **Row ID:** Unique row identifier
- **Order ID:** Unique order identifier
- **Order Date:** Date when order was placed
- **Ship Date:** Date when order was shipped
- **Ship Mode:** Shipping method (e.g., Second Class, Standard Class)
- **Customer ID:** Unique customer identifier
- **Customer Name:** Name of the customer
- **Segment:** Customer segment (Consumer, Corporate, Home Office)
- **Country/City/State/Postal Code/Region:** Customer location
- **Product ID:** Unique product identifier
- **Category:** Product category (Furniture, Office Supplies, Technology)
- **Sub-Category:** Specific product subcategory
- **Product Name:** Name of the product
- **Sales:** Revenue generated from the order
- **Quantity:** Number of units ordered
- **Discount:** Discount percentage applied
- **Profit:** Profit from the order

## Dependencies
The project requires the following Python libraries:

```
pandas
numpy
matplotlib
seaborn
plotly
```

## Installation

### Install Required Libraries:
```bash
pip install pandas numpy matplotlib seaborn plotly
```

## Project Structure

### Step 1: Import Library and Dataset
- Imports all necessary libraries (pandas, numpy, matplotlib, seaborn, plotly)
- Loads the Superstore CSV data with encoding handling (latin1/cp1252)
- Displays first 5 rows for initial data exploration

### Step 2: Data Cleaning & Processing
- Checks for missing values in the dataset
- Converts 'Order Date' and 'Ship Date' columns to datetime format
- Creates new features through Feature Engineering:
  - **Order Year:** Extract year from Order Date
  - **Order Month:** Extract month name from Order Date
  - **Order Day:** Extract day name from Order Date
  - **Profit Margin:** Calculates profit margin percentage = (Profit / Sales) * 100

### Step 3: Exploratory Data Analysis (EDA)

#### A. Category-wise Sales and Profit Analysis
- Groups data by product category
- Calculates total sales and profit for each category
- Creates interactive bar chart using Plotly showing sales vs profit comparison
- Identifies which product category is most profitable

#### B. Monthly Sales Trend Analysis
- Aggregates sales by year and month
- Visualizes trends across different years using line plots with hue differentiation
- Helps identify seasonal patterns and business cycles

### Step 4: Statistical Correlation Analysis
- Computes correlation matrix for key metrics:
  - Sales
  - Quantity
  - Discount
  - Profit
- Creates a heatmap to visualize relationships between variables
- Key insight: Analyzes whether offering discounts negatively impacts profit

### Step 5: Customer Segmentation Analysis
- Groups customers by segment (Consumer, Corporate, Home Office)
- Aggregates total sales, profit, and order count for each segment
- Creates interactive pie chart showing profit distribution across segments
- Identifies which customer segment generates maximum profit

### Step 6: Time Series Analysis
- Converts Order Date to index for time series analysis
- Resamples data at monthly frequency to aggregate sales
- Creates line chart with markers to visualize sales trends over the full timeline
- Helps identify business growth patterns and anomalies

## Output Files
The project generates interactive visualizations stored in:
- **iframe_figures/figure_7.html:** Generated Plotly visualization
- **iframe_figures/figure_9.html:** Generated Plotly visualization

These HTML files can be opened in any web browser for interactive exploration.

## How to Run

1. **Open the Jupyter Notebook:**
   ```bash
   jupyter notebook superstore_data_analysis.ipynb
   ```

2. **Run All Cells:**
   - Use Jupyter menu: Cell → Run All
   - Or press Ctrl+A followed by Ctrl+Enter

3. **Execute Individual Sections:**
   - Run cells sequentially from top to bottom
   - Each section builds upon previous data cleaning steps

4. **View Interactive Visualizations:**
   - Plotly charts will display inline within the notebook
   - Download generated HTML files from iframe_figures folder

## Key Insights Expected

Based on the analysis, you can expect insights such as:

1. **Category Performance:** Which product category (Furniture, Office Supplies, Technology) drives revenue and profit

2. **Discount Impact:** Correlation between discount rate and profit margin—identifying if heavy discounting reduces profitability

3. **Segment Value:** Identification of the most valuable customer segment (Consumer, Corporate, or Home Office)

4. **Seasonal Trends:** Identification of peak sales months and seasonal patterns

5. **Growth Patterns:** Overall sales trend direction—whether business is growing or declining over time

## Technical Details

### Visualization Libraries Used:
- **Matplotlib:** For static visualizations (line plots)
- **Seaborn:** For statistical visualizations (heatmap, correlation plots)
- **Plotly:** For interactive visualizations (bar charts, pie charts, line charts)

### Data Processing:
- Uses pandas for data manipulation and aggregation
- NumPy for numerical computations
- DateTime parsing for time-based analysis

## Notes

- The notebook handles encoding issues automatically (tries latin1, falls back to cp1252)
- All dates are properly converted to datetime format for accurate time series analysis
- Interactive visualizations created with Plotly can be zoomed, panned, and explored interactively
- Missing values are identified but the dataset appears complete

## Author
Created as part of NavioTech Project 2

## Last Updated
May 2026

---

For questions or modifications, ensure you maintain the data processing logic and only update documentation as needed.
