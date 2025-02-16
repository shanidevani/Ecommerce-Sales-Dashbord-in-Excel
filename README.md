# **Ecommerce Sales Dashboard - Excel Report**
## **Overview**
This **Ecommerce Sales Dashboard** is designed to analyze key business metrics such as **total sales, quantity sold, profit, and customer behavior**. Built using **Microsoft Excel**, the dashboard visualizes essential insights through interactive charts, helping businesses track performance trends and make data-driven decisions.

# **Key Performance Indicators (KPIs)**
At the top of the dashboard, four major KPIs summarize overall sales performance:
  - **Total Sales Amount (₹437,771)**: The total revenue generated.
  - **Total Quantity Sold (5615)**: The number of units sold across all categories.
  - **Total Profit (₹36,963)**: The net profit earned after deductions.
  - **Average Price (₹77.96)**: The average selling price per unit.
These KPIs provide a **quick performance summary** to assess revenue growth, profitability, and sales volume.

# **Detailed Breakdown of Charts**
## **1. Profit by Payment Mode (Bar Chart)**
This chart displays profit distribution across different payment methods:
  - **Credit Card & COD (Cash on Delivery)** generate the highest profit.
  - **EMI, Debit Card, and UPI** contribute smaller profit margins.
> [!IMPORTANT]
>**Insight**: Encouraging digital payments and providing discounts on high-profit payment methods can enhance revenue.

## **2. Top 5 States by Sold Quantity (Donut Chart)**
This visualization shows the top-performing states based on sales volume:
  - **Madhya Pradesh (37%)** leads in sales quantity.
  - **Maharashtra (33%)** follows closely.
  - Other high-performing states include D**elhi (9%), Gujarat (10%), and Uttar Pradesh (11%)**.
> [!IMPORTANT]
> **Insight**: Expanding product distribution in these states can further drive sales.

## **3. Top 6 Customers by Amount (Bar Chart)**
This chart identifies the highest-paying customers:
  - **Harjyash, Madhav, and Madan Mohan** are the top spenders.
  - **Shiva, Vishaka, and Vimala** also contribute significantly to revenue.
> [!IMPORTANT]
> **Insight**: Offering personalized deals or loyalty programs to high-spending customers can boost retention and sales.

## **4. Monthly Profit (Bar Chart)**
This graph illustrates monthly profit trends:
  - Profits fluctuate across different months.
  - Some months show **negative profits**, indicating higher costs or lower sales.
  - The highest profit spike is seen in **December**, suggesting a strong year-end sales period.
> [!IMPORTANT]
> **Insight**: Seasonal promotions and better cost management strategies can optimize profits.

## **5. Top 5 Cities by Amount (Bar Chart)**
This chart ranks cities based on total sales revenue:
  - **Indore (₹63,680)** and **Mumbai (₹58,886)** generate the highest sales.
  - Other top-performing cities include **Pune, Mathura, and Bhopal**.
> [!IMPORTANT]
> **Insight**: Strengthening marketing and logistics in these cities can enhance business growth.

## **6. Top 5 Sub-Categories by Quantity (Bar Chart)**
This visualization highlights the most sold product categories:
  - **Sarees (795 units)** and **Handkerchiefs (741 units)** have the highest sales.
  - **Stoles, Furnishings, and T-shirts** also contribute significantly to sales volume.
> [!IMPORTANT]
> **Insight**: Stocking up on high-demand products and optimizing inventory can improve revenue and reduce stockouts.

# **Financial Year Calculation (Custom Excel VBA Function)**
To analyze data based on the **financial year (April to March)**, a **custom VBA function** has been created. This function calculates the **financial year** for any given date.

## **VBA Code for Financial Year Calculation**
```Excel
   Function FY(dateValue As Date) As String
      Dim yearr As Integer
      Dim monthh As Integer
  
      yearr = Year(dateValue)
      monthh = Month(dateValue)
  
      If monthh < 4 Then
          FY = (yearr - 1) & "-" & yearr
      Else
          FY = yearr & "-" & (yearr + 1)
      End If
   End Function
```
## **How It Works:**
  - This function **takes a date as input** and returns the **financial year** in the format **YYYY-YYYY**.
  - If the month is **January, February, or March**, it assigns the previous year as the start of the financial year.
  - If the month is **April or later**, it assigns the current year as the start of the financial year.

## **Example Usage in Excel VBA:**
```=FY(Date) ' If today is 16-Feb-2025, it returns "2024-2025"```

## **Practical Use Cases:**
  - Categorizing sales and profits based on financial years.
  - Financial reporting for tax and accounting purposes.
  - Trend analysis based on fiscal years instead of calendar years.

# **Conclusion**
This **Ecommerce Sales Dashboard (Excel Report)** provides **valuable insights** into customer behavior, regional sales trends, and profitability. The analysis enables businesses to make informed decisions on pricing, marketing, and inventory management.

The addition of the **Financial Year VBA function** enhances financial reporting and helps businesses align data with fiscal periods
