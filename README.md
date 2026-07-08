# Enterprise Logistics & Fleet Operations Performance Analytics
## 📌 Project Overview
This project delivers an enterprise-grade end-to-end data analytics solution designed for a major logistics and supply chain network operating across multiple metropolitan markets. Processing datasets across corporate finances, route configurations, asset telemetry, fuel expenditures, and safety compliance, this multi-page dashboard empowers executives, fleet managers, and supply chain directors to transition from reactive planning to data-driven operational optimization.
The final system diagnoses critical trade-offs between rapid business scaling, asset health, fuel efficiency, and fulfillment reliability.  
## 📊 Dashboard Architecture & Core Insights
### 1. Executive & Financial Overview
* Macro Profitability: Tracks a $298.62M total revenue engine operating at a highly efficient 65.18% profit margin, yielding a net profit of $194.64M.
* Growth Velocities: Implements year-over-year (YoY) delta tracking showing stable month-over-month trends alongside a massive 53.03% YoY net profit expansion, signaling aggressive corporate scaling.
* Strategic Assets: Isolates top revenue lanes (e.g., Route RTE00044 at $11.2M) and tier-1 accounts (e.g., First Group at $10.4M) to secure core business revenue.  
### 2. Operations & Fleet Performance
* Capacity Utilization: Monitors asset wear across 120M total miles driven with a steady fleet utilization baseline of 83.04%.
* Bottleneck Detection: Uncovers an operational risk with a 31.78% increase in downtime peaking sharply in Q4 (19.0K hours), correlating directly with a 46.73% YoY surge in maintenance costs ($4.33M).
* Asset Lifecycle Management: Categorizes real-time truck statuses (92 Active, 15 In-Maintenance, 13 Inactive) and flags outlier vehicles like TRK00073 ($77K in maintenance costs) for replacement reviews.
### 3. Driver, Fuel & Safety Analytics 
* Cost Optimization: Pinpoints fuel as the primary operational cost driver at $95.59M (consuming over 90% of the company's $103.98M cost structure).
* Risk Mitigation: Audits 170 safety incidents and identifies high-risk drivers (e.g., David Miller with 7 violations) to direct targeted safety coaching and insurance risk management.
### 4. Customer, Route & Demand Analytics
* Fulfillment Reliability: Highlights a critical supply chain bottleneck with an aggregate On-Time Delivery (OTD) rate of 56%.
* Geographic Variances: Maps delivery performance geographically to show strong logistics hubs like Phoenix (70% OTD) versus underperforming corridors like Indianapolis (44% OTD).
* Contract Optimization: Segments 171K total deliveries across contract vehicles to balance stable Contract agreements (64.4K) against volatile Spot market lanes (53.7K).
## 💾 Relational Data Schema
The analytics system maps business realities by creating a cohesive data model across these primary flat files:
* customers.csv / facilities.csv: Corporate accounts, client tier types, and shipping/receiving facility nodes.
* routes.csv / trips.csv: Spatial data mapping corridors, planned trip intervals, and actual travel parameters.  delivery_events.csv: Event logs calculating time stamps, fulfillment delays, and granular OTD anomalies.
* fuel_purchases.csv / driver_monthly_metrics.csv: Financial ledgers recording transactional fuel consumption, average MPG, and miles by operator.
* maintenance_records.csv / safety_incidents.csv: Logs capturing active/inactive truck durations, breakdown types, costs, and safety violations.
## 🛠️ Data Modeling & Technical Stack
* BI & Visualization: Power BI Desktop / DAX (Data Analysis Expressions)
* Data Modeling: Star Schema / Snowflake relational structure linking dimensional tables (Drivers, Customers, Vehicles, Routes) to transactional Fact tables (Trips, Deliveries, Maintenance, Fuel).
* Time-Intelligence Functions: Extensively applied in DAX to generate dynamic rolling Month-over-Month (MoM) and Year-over-Year (YoY) financial variances.
## Dashboard
<img width="510" height="311" alt="image" src="https://github.com/user-attachments/assets/b4290831-8eb0-4aa8-807b-4ef7a7511d9b" />
<img width="514" height="317" alt="image" src="https://github.com/user-attachments/assets/90e775d7-d587-4b65-bfeb-664299f478f7" />
<img width="510" height="304" alt="image" src="https://github.com/user-attachments/assets/c7c0f3b9-0a39-4fc3-afa9-cf7053bce74c" />
<img width="510" height="317" alt="image" src="https://github.com/user-attachments/assets/4663774b-9052-43f2-bb18-9abd416b8be0" />
<img width="518" height="361" alt="image" src="https://github.com/user-attachments/assets/24edb10b-030c-4ee3-bd05-81895ff499f4" />
## Datasets Used
