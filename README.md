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

# 🏡 Dashboard Explanation 

This dashboard provides insights into property size, bedroom distribution, property types, and parking space trends. Below is a clear breakdown of each section.

<img width="900" height="500" alt="weekly pattern" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/property2.png" />

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

# 🏡 Dashboard Explanation

This dashboard provides a time-based analysis of MarketValue along with insights into Listing Dates, Property Types, Furnishing Status, and Listing Types. Below is a detailed breakdown of each visual.

---
<img width="900" height="500" alt="OUTLET" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/property3.png" />

## 📌 1. KPI Summary Cards

### **Min of MarketValue – 80K**
Represents the lowest recorded MarketValue in the dataset.

### **Max of MarketValue – 900K**
Represents the highest MarketValue among all properties.

These KPIs indicate the overall price range of the properties.

---

## 🎛 2. Listing Date Filter (Slicer)

A date range selector that filters all visuals by ListingDate  
*(e.g., from 01-01-2023 to 27-04-2023)*.

---

## 📈 3. Average of MarketValue by Year, Quarter, Month, and Day (Line Chart)

This time-series line chart shows:

- Daily/Monthly fluctuations in MarketValue  
- Overall price trends via the dotted trend line  
- Market behavior patterns over the selected time period  

It helps identify whether property values are rising, stable, or fluctuating.

---

## 📊 4. Count of ListingDate by PropertyType

A bar chart displaying the number of listings for each property type:

- Apartment – 2  
- Condo – 2  
- Duplex – 2  
- House – 2  
- Villa – 2  

All property types have equal listing counts within the selected date range.

---

## 📉 5. Average of MarketValue by FurnishingStatus

A horizontal bar chart comparing MarketValue across:

- Furnished  
- Unfurnished  
- Semi-Furnished  

This reveals whether furnishing level impacts property value.

---

## 🥧 6. Sum of ListedPrice by ListingType (Pie Chart)

Shows the percentage share of total listed price:

- **Sale – 50.44%**  
- **Rent – 24.79%**  
- **Lease – 24.77%**

Sale contributes the highest total value, while Rent and Lease contribute almost equally.

---

 ## 📝 Overall Insights

- Provides a complete view of MarketValue trends and property pricing.  
- Shows how furnishing status influences property value.  
- Highlights the distribution of listings across property types.  
- Displays how Sale, Rent, and Lease contribute to total listed price.  
- Time-based filtering allows detailed period analysis.


This dashboard is ideal for real estate analysts, investors, and decision-makers who want to understand market value behavior and listing patterns.

---

This dashboard is ideal for real estate analysts, investors, and decision-makers who want to understand market value behavior and listing patterns.


# 🏢 Commercial Office Market Insights – Dashboard Explanation

This dashboard provides a detailed overview of commercial office locations, their establishment trends, and city-wise distribution. It helps in understanding how many offices exist, where they are located, and when they were established.

---
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/office.png" />

## 📌 1. KPI Summary Cards

### **Count of OfficeID – 50**
Represents the total number of commercial offices in the dataset.

### **Count of EstablishedYear – 32**
Shows the number of unique establishment years across all offices.

These KPIs provide a quick snapshot of office volume and time span.

---

## 🎛 2. City Filter (Slicer)

Allows filtering data by:
- Austin  
- Dallas  
- Houston  

Selecting a city updates all visuals to show office data only for that specific location.

---

## 🎚 3. EstablishedYear Range Filter

A slider that filters offices based on their establishment year.  
Example: Viewing offices built between **1980 and 2020**.

All visuals adjust dynamically based on the selected range.

---

## 📊 4. Count of EstablishedYear by City (Bar Chart)

This chart displays the number of offices established in each city:

- **Dallas – 22 offices**  
- **Houston – 18 offices**  
- **Austin – 10 offices**

This highlights which cities have the highest development of commercial offices.

---

## 📋 5. Office Details Table

A detailed table showing:

- **OfficeID**  
- **OfficeName**  
- **ManagerName**  
- **City**  
- **Address**  
- **EstablishedYear**

### Insights from the table:
- Many offices are managed by **Bob Head**.
- Offices are spread across Austin, Dallas, and Houston.
- Establishment years range widely, from **1982 to 2020**.

This table is useful for looking up specific office information.

---

## 📝 Overall Insights

- Shows total office count and establishment year distribution.
- Highlights which cities have the most office developments.
- Provides full office details for deeper analysis.
- Helps analyze establishment trends across decades.
- Allows filtering by city and year for focused insights.

This dashboard is ideal for corporate planners, real estate analysts, and market researchers.

---


# 🏘️ Neighborhood Market Analysis – Dashboard Explanation

This dashboard provides insights into key neighborhood factors such as crime rate, school quality, income distribution, and walkability across three major cities: **Austin, Dallas, and Houston**. It helps compare neighborhood livability and market potential.

---
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/neighbor.png" />

## 📌 1. KPI Summary Cards

### **Average of CrimeRate – 4.55**
Represents the overall average crime rate across all neighborhoods.

### **Average of SchoolRating – 5.42**
Shows the average school quality rating among the cities.

### **Min of AverageIncome – 30K**
The lowest recorded household income in the dataset.

### **Count of WalkabilityScore – 86**
Indicates the total number of neighborhoods with available walkability data.

These KPIs offer a quick view of neighborhood safety, education, income, and accessibility.

---

## 🎛 2. City Filter

Allows users to analyze data specifically for:
- Austin  
- Dallas  
- Houston  

Selecting a city updates all visuals in the dashboard.

---

## 🥧 3. Average of CrimeRate by City (Pie Chart)

Displays the city-wise distribution of average crime rates:

- **Dallas – 37.16%**
- **Houston – 34.39%**
- **Austin – 28.45%**

### Insight:
Dallas has the **highest average crime rate**, while Austin has the **lowest**, indicating potentially safer neighborhoods.

---

## 📊 4. Average of SchoolRating by City (Bar Chart)

Shows the education quality across cities:

- **Dallas – highest**
- **Austin – moderate**
- **Houston – slightly lower**

### Insight:
Dallas neighborhoods rank best in school quality.

---

## 📉 5. Count of AverageIncome by City (Horizontal Bar Chart)

Number of neighborhoods with income data:

- **Austin – 75**
- **Houston – 72**
- **Dallas – 53**

### Insight:
Austin and Houston have more neighborhood entries than Dallas.

---

## 📝 Overall Insights

- Austin appears to be the **safest city**, with the lowest crime rate.  
- Dallas offers the **best school ratings** among the three.  
- Houston shows balanced mid-range performance across factors.  
- Income data is more extensive for Austin and Houston.  
- The dashboard helps compare livability factors across major cities effectively.

---


# 🧑‍💼 Agent Performance Overview – Dashboard Explanation

This dashboard provides a detailed analysis of real estate **agent performance**, focusing on experience levels, licensing trends, office distribution, and individual agent details. It helps management evaluate the strength and structure of the agent workforce.

---
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/agent.png" />

## 📌 1. KPI Summary Cards

### **Min Years of Experience – 1**
The least experienced agent has **1 year** of experience.

### **Count of Years of Experience – 20**
There are **20 unique levels of experience** across all agents (1–20 years).

### **Count of OfficeID – 50**
Represents the total number of office locations included in the dataset.

These KPIs give a high-level view of agent experience diversity and office coverage.

---

## 🎛 2. Region Filter

Allows filtering agent data by region:
- East  
- North  
- South  
- West  

Selecting a region updates the entire dashboard accordingly.

---

## 📋 3. Agent Details Table

This table displays detailed information for each agent:

- **OfficeID**  
- **AgentID**  
- **Full Name**  
- **Phone**  
- **Email**  
- **Years of Experience**  
- **License Number**

### Insight:
This acts as a complete **agent directory**, enabling quick reference and analysis of agent profiles, contact details, and experience.

---

## 📈 4. Count of LicenseNumber by Years of Experience (Line Chart)

This chart shows how many agents (based on license count) fall into each experience level.

### Key Insights:
- Some experience years have higher agent counts.  
- Experience distribution is mixed, indicating a workforce balanced between junior and senior agents.  
- Helps identify potential gaps in experience levels.

---
## 📝 Overall Insights

- Agent experience ranges from **1 to 20 years**, indicating a diverse team.  
- The company has **50 offices**, reflecting wide operational reach.  
- License distribution across experience levels helps track agent availability and qualification.  
- The detailed table enhances visibility into agent profiles and supports performance evaluation.  
- Region filters allow targeted analysis for localized decision-making.

---

<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/OWNER.png" />

# 🏠 Owner Profile Analysis – Dashboard Explanation

This dashboard presents a structured and searchable view of **property owner information**, allowing users to filter owners by **city** and review detailed contact and address data. It serves as a centralized directory for property ownership records.

---
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/OWNER.png" />

## 📌 1. Dashboard Purpose

The main objectives of this dashboard are:

- To display **complete owner profiles**  
- To enable **city-based filtering** for faster navigation  
- To provide quick access to owner **contact details and addresses**  
- To support **property management and verification processes**

---

## 🎛 2. City Filter Buttons

At the top right, the dashboard includes filters for selecting:

- **Austin**  
- **Dallas**  
- **Houston**

Selecting any city updates the table to show only the owners located in that specific city.

In the screenshot, **Austin is selected**, so only Austin-based owners are displayed.

---

## 📋 3. Owner Details Table

The main table shows detailed information for each owner, including:

### **OwnerID**  
A unique identifier for each property owner.

### **OwnerName**  
Name of the owner.  
*(In this dataset, all owners are named "Sarah", indicating sample or placeholder data.)*

### **ContactNumber**  
Owner’s phone number for communication.

### **Email**  
Email address of the property owner.

### **City**  
The city where the owner resides.  
Filtered dynamically based on selected city.

### **Address**  
Street address of the owner or their property.  
Some entries may show **N/A** if address data is missing.

---

## 📝 4. Dashboard Insights

- Displays **all owners from a selected city** in a clean and organized format.  
- Helps teams quickly **contact owners** using email or phone details.  
- Shows **complete property address information** for verification purposes.  
- Acts as a **central owner database**, useful for property management teams.  
- Ensures easy tracking and reference of owner details.

---

## 📌 Overall Summary

This dashboard functions as a **comprehensive Owner Profile Directory**, consolidating:

- Owner identity  
- Contact details  
- City and address information  

It makes owner management more efficient and supports both operational and analytical tasks.

---


# 🏘️ Market Insights: Agents and Properties – Dashboard Explanation

This dashboard provides a comprehensive overview of real estate **agents**, their **experience levels**, **geographic distribution**, and the **properties** they manage across key cities. It helps evaluate both workforce structure and market availability.

---
<img width="900" height="500" alt="Screenshot 2025-09-14 2136" src="https://github.com/AvishkarK07/Real_Estate_Analysis/blob/main/image/Agent-property.png" />

## 📌 1. KPI Summary Cards

### **Min of YR Of Exp – 1**
Indicates that the least experienced agent has **1 year** of experience.

### **Average of MarketValue – 492.83K**
Shows the average market value of properties handled by agents.

These metrics give a quick snapshot of agent experience and property value trends.

---

## 🎛 2. Filters (Slicers)

### **Region Filter**
Filter data by:
- East  
- North  
- South  
- West  

### **City Filter**
Filter data for:
- Austin  
- Dallas  
- Houston  

These filters allow focused analysis based on location.

---

## 📊 3. Count of AgentID by Years of Experience (Horizontal Bar Chart)

This chart displays the number of agents associated with each experience level (1–20 years).

### Insight:
Most experience categories contain **15–20 agents**, indicating a well-distributed mix of junior, mid-level, and senior agents.

---

## 🥧 4. Count of PropertyID by City (Donut Chart)

Distribution of properties across cities:

- **Dallas – 49.69% (~4.97K properties)**  
- **Houston – 25.26% (~2.53K properties)**  
- **Austin – 25.05% (~2.51K properties)**  

### Insight:
Dallas has the **largest property market**, holding nearly half of all properties.

---

## 🗺 5. Count of AgentID by City (Map Visual)

A geographic view showing where agents are located across Texas cities:

- Austin  
- Dallas  
- Houston  

Larger circles represent higher agent counts.

### Insight:
Dallas appears to have the strongest agent concentration.

---

## 📈 6. Count of AgentID by City (Bar Chart)

Shows the total number of agents per city:

- **Austin – ~300 agents**  
- **Dallas – ~300 agents**  
- **Houston – ~300 agents**

### Insight:
All three cities have an **almost equal number of agents**, ensuring balanced market servicing.

---

## 📝 Overall Insights

- Agent distribution across cities is nearly equal.  
- Dallas dominates in property volume, followed by Houston and Austin.  
- Experience levels are well-distributed among agents (1–20 years).  
- Map visual provides a clear picture of geographic agent coverage.  
- Average market value (~492K) indicates mid-to-high property pricing.

---



<h1>📌 Conclusion</h1>

This analysis highlights the rapid adoption of digital payments in India, with strong growth across states, particularly urban regions. Insights support better product strategies and targeted financial services.
