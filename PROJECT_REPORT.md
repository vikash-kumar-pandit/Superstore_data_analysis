# SUPERSTORE DATA ANALYSIS - PROJECT REPORT

---

## QUICK SUMMARY

This project looks at sales data from a superstore. It helps us understand which products sell well, how discounts affect profit, and which customers are most important. We use Python and Jupyter to analyze the data and show results in easy-to-read charts.

---

## PROJECT OVERVIEW

### Project Name
**Superstore Sales Data Analysis**

### Project Type
Data Analysis (Learning how to use data)

### What Does It Do?
We look at superstore sales data and find important patterns and trends.

### What Questions Does It Answer?
- Which products make the most money?
- Does giving discount reduce profit?
- Which type of customers buy most?
- When do sales go up and down?
- Is the business growing or getting smaller?

---

## WHAT IS THIS PROJECT?

This is a **data analysis project**. 

Think of it like this:
- We have a big CSV file with sales information
- We clean the data
- We ask questions about the data
- We create charts to show answers
- We help make better business decisions

We use simple tools:
- **Python:** A computer language to work with data
- **Jupyter Notebook:** A tool to write and run Python code
- **Charts:** Pictures that show data

---

## HOW DOES IT WORK?

### Simple Steps

```
Step 1: Load the data from CSV file
        ↓
Step 2: Clean the data (remove bad parts)
        ↓
Step 3: Create new information from data
        ↓
Step 4: Ask questions about data
        ↓
Step 5: Show answers with charts
```

### What Happens At Each Step

#### **STEP 1: LOAD THE DATA**

We bring in the CSV file into Python. The file has 9,994 rows. Each row is one sale.

We use these tools:
- **Pandas:** Read the CSV file
- **NumPy:** Do math
- **Plotly:** Make interactive charts
- **Matplotlib:** Make simple charts

**Input:** CSV file
**Output:** Data ready to use

---

#### **STEP 2: CLEAN AND FIX THE DATA**

We check the data for problems.

What we do:
- Look for empty cells or wrong data
- Change dates from text to date format
- Create new columns with useful info

**New columns we create:**

| Column Name | What It Is | Why We Need It |
|-------------|-----------|---|
| Order Year | Year of the order | Compare different years |
| Order Month | Month of the order | See monthly trends |
| Order Day | Day of the week | See which days are busy |
| Profit Margin | How much profit we make | See which sales are good |

**Input:** Raw data with problems
**Output:** Clean data ready to analyze

---

#### **STEP 3: LOOK AT THE DATA (EXPLORATORY ANALYSIS)**

We ask simple questions about the data.

**Question A: Which category sells best?**
- Group sales by category (Furniture, Office, Technology)
- Add up total money and profit for each
- Show results in a bar chart
- Find which one makes most money

**Question B: What are the trends each month?**
- Look at sales for each month
- Compare different years
- Show in a line chart
- See if there are busy months

---

#### **STEP 4: CHECK RELATIONSHIPS BETWEEN DATA**

We ask: Do different things affect each other?

**We check these relationships:**
1. Sales and Quantity - More units sold = more money?
2. Discount and Profit - Less price = less profit?
3. Quantity and Profit - More items = more profit?

We use a special math called Pearson correlation.

**What we show:** A heatmap (a chart with colors showing relationships)

**Important finding:** If we give too much discount, profit goes down!

---

#### **STEP 5: LOOK AT DIFFERENT CUSTOMER TYPES**

We separate customers into 3 groups:

1. **Consumer:** Regular people buying for home
2. **Corporate:** Companies buying for office
3. **Home Office:** People working from home

For each group we check:
- How much money they spend
- How much profit they bring
- How many times they buy

We show this in a pie chart.

---

#### **STEP 6: LOOK AT SALES OVER TIME**

We look at what happened month by month over the whole time period.

**We do this:**
1. Sort data by date
2. Add up sales for each month
3. Show in a line chart with dots
4. See if sales go up or down

**What we learn:**
- Is business getting better?
- When do we sell most?
- Are there any sudden changes?

---

## THE DATA

### File Details
- **File Name:** Superstore.csv
- **Type:** Text file with data separated by commas
- **Number of Rows:** 9,994 (9,994 sales)
- **Number of Columns:** 21 (21 pieces of information)

### All the Information We Have

| Column | Type | What It Means | Example |
|--------|------|---|---|
| Row ID | Number | Line number | 1 |
| Order ID | Text | Order code | CA-2016-152156 |
| Order Date | Date | When order was made | 11/8/2016 |
| Ship Date | Date | When order was sent | 11/11/2016 |
| Ship Mode | Text | How it was sent | Second Class |
| Customer ID | Text | Customer code | CG-12520 |
| Customer Name | Text | Customer name | Claire Gute |
| Segment | Text | Type of customer | Consumer |
| Country | Text | Country | United States |
| City | Text | City name | Henderson |
| State | Text | State name | Kentucky |
| Postal Code | Number | Zip code | 42420 |
| Region | Text | Region | South |
| Product ID | Text | Product code | FUR-BO-10001798 |
| Category | Text | Product group | Furniture |
| Sub-Category | Text | Product type | Bookcases |
| Product Name | Text | Product name | Bush Somerset Collection Bookcase |
| Sales | Money | Money received | 261.96 |
| Quantity | Number | Items sold | 2 |
| Discount | Percentage | Price cut given | 0.00 (no cut) |
| Profit | Money | Money earned | 41.9136 |

---

## RESULTS WE GET

### Charts We Make

1. **Category Chart** - Shows money by type (Furniture, Office, Tech)
   - File: figure_7.html
   - Type: Interactive chart
   - Can click and explore

2. **Monthly Chart** - Shows sales each month for many years
   - Type: Line chart
   - Shows patterns

3. **Discount Impact** - Shows if discount hurts profit
   - Type: Heat map (color chart)
   - Shows connections between data

4. **Customer Type Chart** - Shows which customer type makes most profit
   - File: figure_9.html
   - Type: Pie chart (looks like a pizza)
   - Interactive

5. **Time Chart** - Shows total sales over all time periods
   - Type: Line chart with dots
   - Can zoom in and out

---

## WHAT WE LEARN

### Important Findings

**1. Best Product Categories**
- Which type of product makes most money
- Which type makes most profit
- Which products to focus on

**2. About Discounts**
- Do discounts help or hurt profit?
- Should we give less discount?
- How much discount is good?

**3. Best Customer Type**
- Which type of customer is most important
- Who spends the most money
- Who is most profitable

**4. Busy Seasons**
- When do people buy most?
- When do we make most profit?
- When is business slow?

**5. Business Growth**
- Is business getting bigger or smaller?
- What are the trends?
- What can we expect in future?

---

## TECHNOLOGY WE USE

### Main Tools
- **Python:** Programming language
- **Jupyter:** Tool to write and run Python
- **Windows:** Computer system

### Libraries (Extra Tools for Python)
```
pandas    - Read and organize data
numpy     - Do math with data
matplotlib - Make charts
seaborn   - Make nice charts
plotly    - Make interactive charts
```

### Steps We Follow
1. Open CSV file
2. Load data into memory
3. Clean the data
4. Fix data types
5. Add new columns
6. Group data
7. Do math
8. Make charts
9. Show results

---

## HOW TO USE THIS

### What You Need
- Python 3.7 or newer
- Jupyter Notebook
- Internet (for some charts)

### How to Start

**Step 1: Install tools**
```
pip install pandas numpy matplotlib seaborn plotly
```

**Step 2: Go to the folder**
```
cd "2nd project naviotech"
```

**Step 3: Start Jupyter**
```
jupyter notebook
```

**Step 4: Open notebook file**
- Click on superstore_data_analysis.ipynb

**Step 5: Run the code**
- Click Run All button
- Or run each cell one by one

**Step 6: See results**
- Charts show in notebook
- HTML files go to iframe_figures folder

### How Long Does It Take
- First time: 2-5 minutes
- Next times: 1-2 minutes

---

## WHAT WE CREATE

### Files We Get

1. ✅ Clean data (in computer memory)
2. ✅ Category analysis chart
3. ✅ Monthly sales trend chart
4. ✅ Discount impact chart
5. ✅ Customer type chart
6. ✅ Time series chart

### Chart Files
- figure_7.html - Category chart (interactive)
- figure_9.html - Customer type chart (interactive)
- Other charts show in notebook

---

## SUMMARY

### Why This Project Is Good

- Uses real data
- Easy to understand
- Shows clear answers
- Helps make decisions
- All charts are interactive
- Can run it yourself

### What This Helps With

1. **Making Plans:** Which products to focus on
2. **Sales Teams:** Set targets and goals
3. **Marketing:** Target right customer types
4. **Money:** Understand profit and loss
5. **Planning:** Plan for busy and slow seasons

---

## QUICK FACTS

### Most Important Numbers
- **Total Sales:** All money from all sales
- **Total Profit:** All money left after costs
- **Profit Margin:** How much profit per sale
- **Discount Effect:** Does discount hurt profit?
- **Sales by Category:** Which type sells most
- **Best Customer Type:** Which makes most profit

### Big Questions We Answer
1. Which products to promote?
2. Should we give discounts?
3. Which customers to target?
4. Is business growing?
5. When are busy seasons?

---

## PROJECT STATUS

✅ **Complete and Ready to Use**

**Last Updated:** May 5, 2026

---

**End of Report**
