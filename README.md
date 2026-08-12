# 🚗 Infosys Urban Pulse – Smart City Mobility Intelligence

A multi-domain **Data Analytics and Business Intelligence project** focused on transforming transportation, ride-hailing, weather, and micro-mobility data into actionable smart-city insights using **Power BI, Power Query, and DAX**.

The project demonstrates an end-to-end analytics workflow covering **data cleaning, exploratory analysis, data modeling, KPI development, relational data integration, and interactive dashboard development**.

---

## 🛠️ Tech Stack & Tools

* **Business Intelligence:** Power BI
* **Data Preparation:** Power Query
* **Data Analysis & KPIs:** DAX
* **Data Sources:** CSV / Relational Datasets
* **Data Modeling:** Star Schema / Fact & Dimension Modeling
* **Visualization:** Power BI Interactive Visuals
* **Version Control:** Git & GitHub

---

## 🎯 Project Objectives

* Analyze mobility and transportation patterns across multiple domains.
* Clean and transform raw datasets into analysis-ready data.
* Build scalable **Fact and Dimension tables** using dimensional modeling.
* Establish relationships between datasets using primary and foreign keys.
* Develop meaningful **business KPIs and calculated measures using DAX**.
* Identify trends in trip demand, revenue, cancellations, weather conditions, and micro-mobility usage.
* Build interactive dashboards that support **data-driven smart-city decision making**.

---

## 🗓️ Project Roadmap

### 📌 Week 1 – Data Exploration & Basic Cleaning

#### 🔍 Exploratory Data Analysis

* Inspected raw datasets for:

  * Missing values
  * Duplicate records
  * Invalid entries
  * Data-type inconsistencies
  * Structural anomalies
* Analyzed initial distributions and trends.
* Identified important fields and relationships across datasets.

#### 🧹 Basic Data Cleaning

* Standardized column names and text values.
* Converted fields into appropriate data types.
* Standardized date and time formats.
* Removed irrelevant and corrupted records.
* Handled duplicate records and basic missing values.
* Created preliminary visualizations to understand dataset behavior.

---

### 📌 Week 2 – Advanced Data Cleaning, Modeling & KPI Development

#### 🧹 Deep Data Cleaning

Performed advanced transformations including:

* Missing-value treatment and imputation.
* Outlier identification and treatment.
* Conditional transformations.
* Data normalization and standardization.
* Derived columns for analytical requirements.
* Validation of cleaned datasets.

#### 🏗️ Data Modeling

Designed a structured **Star Schema** to improve analytical performance and maintainability.

The model separates transactional data from descriptive attributes using:

* **Fact Tables**

  * Trip / Ride Facts
  * Weather Facts
  * Micro-Mobility Usage Facts

* **Dimension Tables**

  * Date Dimension
  * Location Dimension
  * Vehicle Dimension
  * Customer / Rider Dimension
  * Driver Dimension
  * Weather Dimension
  * Station Dimension

Relationships were established using appropriate **primary keys and foreign keys**.

#### 📊 KPI Development

Developed business-focused DAX measures such as:

* Total Rides
* Total Revenue
* Average Ride Distance
* Average Ride Duration
* Cancellation Rate
* Driver Performance
* Peak Hour Demand
* Fleet Utilization
* Weather Impact on Rides
* Customer / Rider Metrics
* Micro-Mobility Usage

KPI cards were created to provide an executive-level overview of important performance indicators.

---

## 📊 Week 3 – Interactive Multi-Domain Dashboards

### 🚗 Ride-Hailing Dashboard

Provides insights into ride-hailing operations and customer demand.

#### Key Analysis

* Total trips and revenue
* Ride demand trends
* Peak hours and high-demand periods
* Driver performance
* Average trip distance and duration
* Cancellation patterns
* Revenue distribution
* Geographic demand patterns
* Vehicle-type performance

---

### ☀️ Weather Intelligence Dashboard

Analyzes weather conditions and their relationship with mobility patterns.

#### Key Analysis

* Temperature trends
* Precipitation patterns
* Weather-condition distribution
* Seasonal variations
* Daily and monthly weather trends
* Relationship between weather and trip demand
* Weather impact on transportation activity

---

### 🛴 Micro-Mobility Dashboard

Analyzes shared micro-mobility usage such as bikes, scooters, and other lightweight transportation modes.

#### Key Analysis

* Total micro-mobility trips
* Fleet utilization
* Vehicle-type performance
* Popular start and end stations
* Peak rental periods
* Trip duration
* Distance traveled
* Station-level demand
* Usage trends over time

---

## 🏗️ Data Architecture

The project follows a dimensional modeling approach based primarily on a **Star Schema**.

```text
                    ┌──────────────────┐
                    │   Date Dimension │
                    └────────┬─────────┘
                             │
                             ▼
┌─────────────────┐   ┌──────────────────┐   ┌──────────────────┐
│ Location Dim.   │──▶│                  │◀──│ Vehicle Dimension│
└─────────────────┘   │   FACT TRIPS     │   └──────────────────┘
                      │                  │
┌─────────────────┐   │                  │   ┌──────────────────┐
│ Customer Dim.   │──▶│                  │◀──│ Driver Dimension │
└─────────────────┘   └──────────────────┘   └──────────────────┘
                             │
                             ▼
                    ┌──────────────────┐
                    │ Weather Dimension│
                    └──────────────────┘
```

---

## 📂 Project Structure

```text
InfosysUrban-Pulse/
│
├── datasets/
│   ├── raw/
│   │   └── Original, untouched datasets
│   │
│   └── processed/
│       ├── Cleaned datasets
│       ├── Fact tables
│       └── Dimension tables
│
├── dashboards/
│   ├── ride_hailing.pbix
│   ├── weather.pbix
│   └── micro_mobility.pbix
│
├── documentation/
│   ├── data_dictionary.md
│   ├── data_model.md
│   └── kpi_definitions.md
│
└── README.md
```

---

## 🔄 End-to-End Analytics Workflow

```text
Raw Data
   ↓
Data Exploration
   ↓
Data Cleaning
   ↓
Data Transformation
   ↓
Fact & Dimension Creation
   ↓
Data Modeling
   ↓
Relationship Mapping
   ↓
DAX KPI Development
   ↓
Interactive Visualizations
   ↓
Dashboard Development
   ↓
Business & Smart-City Insights
```

---

## 📈 Key Business Insights

The dashboards are designed to help identify:

* Transportation demand patterns.
* Peak mobility periods.
* High-performing vehicle categories.
* Revenue and trip trends.
* Driver and operational performance.
* Cancellation behavior.
* Effects of weather on mobility demand.
* Micro-mobility fleet utilization.
* High-demand stations and locations.
* Seasonal and time-based mobility trends.

---

## 💡 Smart-City Applications

The insights generated from the project can support:

* **Transportation Planning** – Identify areas and periods with high mobility demand.
* **Fleet Optimization** – Improve allocation of vehicles across locations.
* **Infrastructure Planning** – Identify high-demand mobility zones.
* **Weather-Aware Operations** – Understand how weather conditions influence transportation demand.
* **Resource Allocation** – Support better deployment of drivers and shared vehicles.
* **Urban Mobility Management** – Enable data-driven planning for sustainable transportation systems.

---

## 🚀 Getting Started

### 1. Clone the Repository

```bash
git clone https://github.com/your-username/InfosysUrban-Pulse.git
cd InfosysUrban-Pulse
```

### 2. Open the Dashboards

Navigate to the `dashboards/` directory and open the required `.pbix` file using **Power BI Desktop**.

### 3. Explore the Data Model

Open the **Model View** in Power BI to inspect:

* Fact tables
* Dimension tables
* Relationships
* Primary and foreign keys
* Star-schema structure

### 4. Explore the Dashboards

Use slicers, filters, drill-downs, and interactive visuals to analyze mobility patterns across different dimensions.

---

## 📌 Project Highlights

* ✅ Multi-domain data analytics
* ✅ End-to-end Power BI workflow
* ✅ Data cleaning and transformation
* ✅ Star-schema data modeling
* ✅ Fact and Dimension table design
* ✅ Relational dataset integration
* ✅ Advanced DAX measures
* ✅ Interactive KPI dashboards
* ✅ Ride-hailing analytics
* ✅ Weather intelligence
* ✅ Micro-mobility analytics
* ✅ Smart-city mobility insights

---

## 🧑‍💻 Skills Demonstrated

**Power BI • Power Query • DAX • Data Cleaning • Data Transformation • Data Modeling • Star Schema • SQL Concepts • KPI Development • Business Intelligence • Data Visualization • Exploratory Data Analysis • Dashboard Design**

---

## 📄 Project Status

🚧 **Project Status: In Progress**

The project is being developed incrementally across data preparation, modeling, KPI development, and dashboard implementation phases.

---

## 👨‍💻 Author

**A Jeevan Reddy**
BTech – Computer Science & Engineering (Artificial Intelligence)

**Areas of Interest:**
Data Analytics • Business Intelligence • Full-Stack Development • Artificial Intelligence • Machine Learning

---

⭐ If you find this project useful, consider giving the repository a **star**!
