# Supplier-Quality-and-Performance-Dashboard

## Project Overview
This project provides Enterprise Manufacturers Ltd. with a comprehensive overview of supplier quality performance, highlights key metrics, such as defect quantities, downtime, and their impacts on overall operations, centralizing critical supplier data to improve quality management and procurement efficiency. By analyzing these metrics, this dashboard offers valuable insights to help Enterprise Manufacturers Ltd:
- Identify top-performing and underperforming suppliers
- Enhance supplier qualit
- Optimize procurement processes
- Reduce downtime costs
- Improve overall operational efficiency

## Key features of the dashboard:
- Interactive visualizations
- Data-driven insights
- Customizable metrics
- User-friendly interface

## Tools and Data Source
- **Tools:** Power BI, DAX
- **Data Sources:** Supplier data was provided by Tina Okonkwo for Enterprise Manufacturers Ltd, a pseudo company. This dataset included columns such as date, vendor, plant location, category, material type, defect type, total defect quantity, and total downtime minutes

## Data Preparation Process
The data preparation process included normalizing and structuring the supplier data for more effective analysis. The following steps were taken:

**Normalization:** The original dataset was broken down into several tables for a more organized data model:

- **Vendor Table**: Contains unique vendors and their details.
- **Plant Table:** Lists plant locations associated with each vendor.
- **Category Table:** Specifies supplies categories.
- **Material Type Table:** Distinguishes various material types.
- **Defect Type Table:** Classifies types of defects.
- **Defect Table:** Logs defect occurrences with relevant metrics, such as quantity and downtime.

**Data Modeling:** Relationships were established between the facts and dimension tables using primary and foreign keys. 

![image](https://github.com/user-attachments/assets/06ebff7c-6e08-4563-a1ad-e547bbbd9c89)

**Date Table Creation:** A custom date table was generated in Power BI using DAX measures to support time-based analysis. This table allows for tracking trends and patterns over time.

![image](https://github.com/user-attachments/assets/f723a253-f807-4c61-bf15-9d55c8775702)

## Data Analysis

## Overview

![2](https://github.com/user-attachments/assets/f9dddcd7-6488-4663-9140-223aa1662410)

### Key Metrics
- **Total Defects:** 2.60 billion
- **Downtime Hours:** 215.81 thousand hours
- **Downtime Cost:** $2.16 million (based on a $10 cost per hour)

### Monthly Trend
**Defect Quantity Trend Analysis:**
- The monthly trend graph compares defect quantities across two years, with notable peaks observed around **March** and **October**. These fluctuations suggest seasonal or cyclical issues in quality control that may be tied to supplier practices or external factors during these months.
- This visual can help stakeholders identify specific periods where defects consistently increase, guiding targeted quality improvement initiatives in these months.

### Impact Breakdown
**Impact Categories:**
- **Impact (31.71%):** The portion of defects that have a direct impact on operations, totaling over 415 million in 2018 and 414 million in 2019. This consistency suggests ongoing quality challenges that are yet to be resolved.
- **No Impact (39.86%):** Defects that do not directly affect operations, which increased significantly from 2018 to 2019, indicating improved resilience in some areas of the supply chain.
- **Rejected (28.43%):** Defects that led to outright rejection of materials or products, with a sharp increase from 310 million in 2018 to 434 million in 2019, suggesting stricter quality standards or worsening supplier quality.

### Worst Performers
**By Vendor:**
- **Avamm:** Top contributor to defects with 14.7 million defects and a high downtime impact of 1,164.82 hours.
- **Meejo** and **Yombu** also have significant defect contributions, suggesting these vendors require immediate quality assessments and possibly corrective actions.

**By Plant:**
- **Charles City** leads in defects with 99.39 million, followed by **Hingham** and **Twin Rocks**. These plants have considerable downtime impacts, pointing to potential operational inefficiencies or quality control issues specific to these locations.
  
**By Material:**
- **Corrugate** material has the highest defect rate, contributing 624.44 million defects and a downtime impact of 51,303.85 hours, followed by **Film and Raw Materials**. This indicates quality issues may stem from the sourcing or handling of these materials.

**By Category:**
- **Logistics** and **Mechanicals** are the categories with the highest defect counts, highlighting potential challenges in these areas.
- **Packaging** also contributes notably, suggesting that product handling and packaging might benefit from quality improvements.

## Vendor Performance Analysis

![3](https://github.com/user-attachments/assets/7c93b01f-5128-473d-a58b-29e3889c62c1)

### Key Insights

### Top Vendors with Highest Defects:
- **Yombu** Leads with 15.1 million defects, followed closely by **Avamm** (14.7 million) and **Meejo** (14.2 million).
- Other vendors with high defect quantities include **Zooxo** (13.8 million), Izio (13.7 million), and **Babbleset** (13.6 million).

### Defect Impact on Downtime:
**Risk Categories:**
This section helps in identifying and categorizing vendors based on their risk level to prioritize quality improvement initiatives.
- **High-Risk Vendors:** Vendors in this category, such as **Yombu** and **Avamm**, have a high defect quantity that correlates with extended downtime hours, leading to increased operational delays.
- **Medium Risk Vendors:** These vendors, including **Meejo** and **Zooxo**, show moderate defect quantities and downtime hours, which still affect overall efficiency but to a lesser extent than high-risk vendors.
- **Low-Risk Vendors:** Vendors in this category show lower defect quantities and minimal downtime impact, posing less risk to operational continuity.

### Impact, No Impact, and Rejected Categories:

**Vendor Impact:**
- **Yombu** has the highest impact, with over 6 million defects that directly affect operations.
- Other high-impact vendors include **Zooxo** (6.8 million), **Meejo** (5.2 million), and **Avamm** (3.3 million).
**No Impact:**
- Some vendors contribute to defects without impacting overall operations, such as **Izio** and **Wikibox**, allowing the team to identify areas where defects may be present but do not necessarily lead to downtime or rejection.
**Rejected:**
- Vendors like **Avamm** and **Meejo** have a high number of rejected units due to defects, signaling quality issues that may necessitate renegotiation or stricter quality control measures.

## Plant Performance Analysis

![image](https://github.com/user-attachments/assets/ed5e5ce3-a839-4cf6-9aff-86f111b4dd4c)

### Key Insights

**Top Plants with Highest Defects:**
- **Hingham** Leads with 100 million defects, closely followed by **Charles City** (99 million), **Twins Rock** (97 million), and **Henning**  (96 million).

### Geographical Distribution of Defects:**

**Defect Quantity by Plant Location (Map):**
- The map visualizes the spatial distribution of defects, enabling the team to analyze if certain regions or locations are more prone to defects, possibly due to environmental factors or supply chain challenges.

### Impact, No Impact, and Rejected Categories:
This section helps differentiate defects that cause operational impacts from those that do not, aiding in targeted quality control initiatives.

**Plant Impact:**
- **Charles City** and **Hingham** have the highest impact levels, each contributing over 30 million defects affecting operations.
- Other plants with substantial impacts include **Twin Rocks** and **Henning**.
**No Impact:**
- Some plants show defect quantities that do not significantly impact operations, enabling management to recognize defects that may not lead to operational downtime.
**Rejected:**
- Plants like **Twin Rocks** and **Riverside** have a high number of rejected units, suggesting issues with quality control that may need attention.

Here's an analysis of the **Material Performance Page** based on the dashboard image provided:

---

## Material Performance Page Analysis
![6](https://github.com/user-attachments/assets/9b5046cc-ce2d-487e-962d-d7f401dc6fdc)

### Key Insights

### Defect Quantity by Material Type
#### Top Material Types with Highest Defects
     **Raw Materials** are the most significant source of defects, with 0.77 billion defects.
    **Corrugate** follows closely with 0.62 billion defects.
    **Film**, **Carton**, and **Labels** also show notable defect quantities but at lower levels compared to the top two materials.
   - **Purpose**: This visualization helps identify which material types contribute the most to quality issues, assisting the team in targeting materials for quality improvement efforts.

2. **Defect Quantity by Defect Type**:
   - **Top Defect Types**:
     - **Not Certified** is the leading defect type, with 152 million instances.
     - Other significant defect types include **Bad Seams** (146 million), **Miscellaneous** (127 million), and **Foreign Material** (98 million).
     - Minor defect types such as **Warped** and **Out of Spec** still contribute meaningfully to overall defects.
   - **Purpose**: This chart breaks down defects by type, providing insights into the most prevalent quality issues. This can guide targeted interventions, such as certification improvements or better seam handling.

3. **Defect Quantity by Category**:
   - **Top Categories with Defects**:
     - **Mechanicals** is the category with the highest defect quantity, amounting to 0.82 billion.
     - **Logistics** and **Packaging** categories also show significant defect quantities, with 0.70 billion and 0.44 billion defects, respectively.
     - **Materials & Components** and **Goods & Services** categories have moderate defect quantities.
   - **Purpose**: This chart shows defect distribution across different categories, helping the team pinpoint which aspects of the supply chain or production processes require enhanced quality control measures.

4. **Monthly Trend of Defects**:
   - **Trend by Category**:
     - Mechanical defects show a sharp increase in certain months, peaking significantly, which might correspond with specific production cycles or seasonal factors.
     - Other categories like **Logistics** and **Packaging** exhibit lower but steady defect levels throughout the months.
   - **Purpose**: The monthly trend chart visualizes defect trends over time for each category, highlighting any seasonality or cyclical quality issues. This allows for proactive planning and mitigation strategies during peak defect periods.

---

### Summary
The Material Performance Page provides a comprehensive view of defect quantities by material type, defect type, and category, along with a trend analysis. It allows the team to identify problematic materials and defect types and analyze the trends, enabling more strategic planning and quality improvement initiatives.

Let me know if you'd like further analysis for additional sections!
