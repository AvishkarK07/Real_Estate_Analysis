# Real_Estate_Analysis

<img width="900" height="500" alt="Screenshot 2025-09-14 211235" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/dash.jpg" />

<H1>Tool Used :</H1>
<img width="315" height="250" alt="Screenshot 2025-09-14 211235" src="https://github.com/AvishkarK07/Power-Bi-Phone_Pay/blob/main/images/power%20bi.jpeg" />


<h1>📌 Project Overview</h1>

This dataset contains detailed information about real estate properties, including their physical characteristics, pricing, location, ownership, and listing details. It is suitable for building dashboards, running exploratory data analysis, predictive modeling, and real estate market insights.


## 🏠 **1. Property Information**

- **PropertyID** – Unique identifier for each property  
- **PropertyName** – Name or label of the property  
- **PropertyType** – Condo, villa, house, apartment, duplex, etc.  
- **ListingType** – Sale / Rent / Lease  

## 📍 **2. Location Details**

- **Address**
- **City**
- **State**
- **Country**
- **ZipCode**
- **Latitude**
- **Longitude**

  ## 🧱 **3. Property Features**

- **Bedrooms**
- **Bathrooms**
- **SquareFeet** – Built-up area  
- **LotSize** – Total land area  
- **YearBuilt**
- **ConditionStatus**
- **FurnishingStatus** – Furnished / Semi-furnished / Unfurnished  
- **ParkingSpaces**
- **HeatingType**
- **CoolingType**
- **PropertyDescription**

  ## 💰 **4. Market & Pricing Data**

- **MarketValue** – Estimated value  
- **ListedPrice** – Price at listing  
- **ListingDate**  
- **SoldDate**
- Great for time-series and price prediction models.

  ## 🧑‍💼 **5. Administrative Identifiers**

- **AgentID**
- **OwnerID**
- **NeighborhoodID**

Useful for agent performance, ownership analysis, and neighborhood segmentation.

## 🎯 **Use Cases**

This dataset is ideal for:

- **Real estate price trend analysis**
- **Predictive models** (price prediction, property classification)
- **Building dashboards** in Power BI / Tableau
- **Market segmentation** by city, type, or neighborhood
- **Agent and owner analytics**
- **Geospatial visualizations** using latitude & longitude

## 🧹 **Data Quality Notes**

- Some fields have inconsistent capitalization (e.g., “TX”, “tx”, “Tx”).  
- Some **PropertyName** values are missing.  
- Dates may require formatting for time-series processing.  
- Category fields should be normalized for modeling.

  


## 📊 **Recommended Dashboard Visuals**

- **Bar Chart:** Properties by city  
- **Pie Chart:** Distribution of property types  
- **Line Chart:** Listing trend by date  
- **KPI Cards:** Average price, total listings, average square feet  
- **Map Visual:** Property locations  
- **Donut Chart:** Furnishing status breakdown




# 🏡 **Property Performance Overview – Dashboard Explanation**

This dashboard provides a complete analysis of property performance across price, market value, listing type, and city. Below is a section-wise explanation of each component.

<img width="900" height="500" alt="item type" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/property1.png" />



---

## 📌 **1. KPI Summary Cards**

### **Average of MarketValue – 492.83K**
Shows the average market value of all listed properties.

### **Sum of ListedPrice – 5bn**
Total combined listed price of all properties.

### **Sum of LotSize – 50M**
Total land area (lot size) covered by all properties.

### **Sum of SquareFeet by LotSize – 3872**
Total indoor area aggregated based on LotSize.

These KPIs give a quick financial and physical overview of the property market.

---

## 🎛 **2. Filters (Slicers)**

### **City Filter**
- Austin  
- Dallas  
- Houston  

Filters all visuals based on selected city.

### **Condition Status Filter**
- Average  
- Excellent  
- Good  
- Poor  

Allows performance comparison based on property condition.

---

## 📊 **3. Donut Chart: Sum of ListedPrice by PropertyType**

Shows the percentage share of total listed price contributed by each property type:

- Apartment  
- Villa  
- Duplex  
- House  
- Condo  

Helps identify which property categories dominate market value.

---

## 📈 **4. Bar Chart: Average of MarketValue by City**

Compares average market value of properties across cities:

- Houston  
- Austin  
- Dallas  

Useful for understanding city-wise real estate pricing trends.

---

## 📉 **5. Bar Chart: Sum of ListedPrice by ListingType**

Shows total listed price distribution across listing types:

- Sale  
- Lease  
- Rent  

Helps understand whether most market value comes from sales, rentals, or leases.

---

## 📝 **Overall Insights**

- Provides a full financial and performance summary of real estate data.  
- Shows which city has higher property value.  
- Compares property types and their market share.  
- Highlights how listing type affects pricing.  
- Includes size metrics (LotSize & SquareFeet) for deeper analysis.

---

# 🏡 **Dashboard Explanation**

This dashboard provides insights into property size, bedroom distribution, property types, and parking space trends. Below is a clear breakdown of each section.
---
<img width="900" height="500" alt="weekly pattern" src="https://github.com/AvishkarK07/Power-Bi-Phone_Pay/blob/main/images/insurance.png" />

## 📌 **1. KPI Summary Cards**

### **Min of SquareFeet – 600**
The smallest property in the dataset has 600 sq. ft.

### **Max of SquareFeet – 5000**
The largest property measures 5000 sq. ft.

### **Min of Bedrooms – 1**
Shows the smallest bedroom count in the dataset.

### **Max of Bedrooms – 6**
Shows the maximum number of bedrooms available across properties.

These KPIs help understand the overall range of property sizes and bedroom capacities.

---

## 📊 **2. Count of Properties by Bedrooms (Bar Chart)**

This chart displays how many properties exist for each bedroom category:

- **1 Bedroom → 1722 properties**
- **2 Bedrooms → 1642 properties**
- **3 Bedrooms → 1606 properties**
- **4 Bedrooms → 1692 properties**
- **5 Bedrooms → 1639 properties**
- **6 Bedrooms → 1699 properties**

This visual shows which bedroom count is most common in the market.

---

## 🎛 **3. Filters (Slicers)**

### **PropertyType Filter**
Select property categories such as:
- Apartment  
- Condo  
- Duplex  
- House  
- Villa  

This allows users to analyze specific property segments.

### **ListingDate Range Filter**
A slider that filters properties based on selected listing dates.

---

## 📈 **4. Average of SquareFeet by PropertyType and ParkingSpaces**

This clustered bar chart compares:

- Different **property types** (Condo, House, Duplex, Apartment, Villa)
- Different **parking spaces** (0, 1, 2, 3, 4)
- Their corresponding **average SquareFeet**

## Key Insights:
- Properties with **more parking spaces generally have larger square footage**.
- Houses, Duplexes, and Villas tend to be **larger** than Apartments and Condos.
- Parking availability significantly influences property size.

---

## 📝 **Overall Insights**

- Provides a detailed view of property size distribution.
- Shows bedroom count popularity across the dataset.
- Highlights size variation across property types and parking capacities.
- Allows filtering by property type and listing date for deeper analysis.



---


<H1>💰 Loan</H1>
<img width="900" height="500" alt="OUTLET" src="https://github.com/AvishkarK07/Power-Bi-Phone_Pay/blob/main/images/loan.png" />

<H1>💸 Money Transfer</H1>
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Power-Bi-Phone_Pay/blob/main/images/Money%20Transfer.png" />

<H1>📱 Recharge_Bills</H1>
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Power-Bi-Phone_Pay/blob/main/images/Recharge_bill.png" />



<h1>📌 Conclusion</h1>

This analysis highlights the rapid adoption of digital payments in India, with strong growth across states, particularly urban regions. Insights support better product strategies and targeted financial services.
