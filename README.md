# Airline-Data-Management-and-Analysis-Using-Power-BI-
Airline data analysis and interactive dashboard built with Power BI, featuring data modeling, DAX, visualizations, and Row-Level Security.

# ✈️ Airline Data Management and Analysis Using Power BI

## 📌 Project Overview

This project focuses on **airline data management, analysis, and visualization using Microsoft Power BI**. The objective was to transform raw airline-related data into a structured and interactive analytical solution that can provide insights into flight operations, passenger information, ticket bookings, airline performance, and destinations.
---
The project demonstrates an end-to-end Power BI workflow, including **data cleaning and preparation, relational data modeling, calculated columns, DAX measures, interactive visualizations, drillthrough analysis, dashboard creation, Power BI Service deployment, and Row-Level Security (RLS)**.

## 🎥 Project Explanation

A video explanation of the project is available here: [https://www.loom.com/share/4d6b9c8566024e9bb07b336b9b860352]

---

## 🎯 Objectives

The main objectives of this project were to:

* Clean and prepare airline datasets for analysis.
* Build a relational data model using `FlightID`.
* Establish appropriate one-to-many relationships between datasets.
* Create calculated columns and DAX measures.
* Analyze passenger and ticket-booking information.
* Build interactive dashboards with slicers and drillthrough functionality.
* Identify airline, flight, destination, and booking trends.
* Implement Row-Level Security (RLS) for controlled data access.
* Publish the final dashboard to Power BI Service.

---

## 📊 Dataset Description

The project uses three main datasets/tables:

### 1. Flight_Information

Contains information related to individual flights.

**Columns:**

* `FlightID`
* `FlightNumber`
* `Airline`
* `Destination`
* `Status`

### 2. Passenger_Information

Contains passenger information associated with flights.

**Columns:**

* `PassengerID`
* `FlightID`
* `SeatNumber`

### 3. Ticket_Information

Contains information about ticket bookings.

**Columns:**

* `TicketID`
* `FlightID`
* `BookingStatus`

The tables are connected through the common `FlightID` field to create a relational data model.

---

## 🧹 Data Preparation & Cleaning

The first stage of the project involved preparing the data for analysis.

The following data-cleaning operations were performed:

* Removed duplicate records.
* Handled missing values.
* Formatted columns appropriately.
* Prepared the datasets for further modeling and visualization.

This ensured that the data was structured properly before creating relationships and analytical calculations.

---

## 🔗 Data Modeling

A relational data model was created using `FlightID` as the key connecting the different datasets.

Relationships were established between the flight, passenger, and ticket information tables with the appropriate **one-to-many cardinality**.

This model allowed information from different tables to be analyzed together within Power BI.

---

## ⚙️ Enhanced Data Insights

Additional columns and transformations were created to make the dataset more useful for analysis.

### Performance Status

A conditional column named `Performance Status` was created to categorize flights as:

* **Best**
* **To Be Improved**

### Flight Number Extraction

Flight numbers were extracted using Power BI's **Column From Examples** functionality.

These transformations helped prepare the data for subsequent calculations and visual analysis.

---

## 🧮 DAX Calculations

DAX (Data Analysis Expressions) was used to create measures and analytical outputs.

The project includes calculations for:

* Total passengers for a specific flight.
* Total tickets booked.
* A filtered table containing only the best-performing flights.

These calculations enabled the dashboard to dynamically analyze flight and booking-related metrics.

---

## 📈 Dashboard & Visualizations

An interactive Power BI dashboard was designed to provide a consolidated view of airline operations.

The dashboard includes:

### Passenger Analysis

A **column chart** was used to display passenger counts by airline.

### Ticket Booking Analysis

A **donut chart** was used to visualize ticket booking statuses.

### Flight Analysis

A stacked chart/matrix was created to analyze flights by:

* Airline
* Destination

### Interactive Filters

Slicers were added for:

* Airline
* Destination

These allow users to dynamically filter the dashboard and explore specific segments of the data.

### Drillthrough Analysis

A dedicated **drillthrough page** was created to provide airline-specific insights and allow users to move from high-level dashboard information into more detailed analysis.

---

## 🔐 Row-Level Security (RLS)

Row-Level Security was implemented to control access to the data.

The project configured RLS for **Airline A** and assigned a user to the corresponding role.

This ensures that users can be restricted to seeing only the data relevant to their assigned airline, demonstrating how Power BI can be used for secure business intelligence reporting.

---

## ☁️ Power BI Service

The completed dashboard was published to **Power BI Service**.

The final solution includes:

* KPI cards
* Interactive visuals
* Detailed tables
* Slicers
* Drillthrough functionality
* Row-Level Security

Publishing the dashboard to Power BI Service demonstrates how the analysis can be made available for business users while maintaining controlled access to sensitive or airline-specific information.

---

## 🔍 Key Insights & Findings

The analysis produced several notable findings:

* **Airline B** has the highest percentage of confirmed tickets.
* **Airline C** has the highest percentage of canceled tickets.
* **Airline D** has the highest number of flights.
* **Airline B** has the lowest number of flights.
* **Phoenix** is the most popular destination among passengers.
* **Airline A and Airline D** have the highest number of passengers.
* **Airline D** has the highest number of best/on-time flights.
* The dataset contains **184 flights** and **100 passengers**.
* **42.39% of flights are on time**.
* Row-Level Security was successfully implemented for Airline A.

These findings provide an overview of flight performance, passenger distribution, ticket booking behavior, and destination popularity within the dataset.

---

## 🛠️ Tools & Technologies

* **Microsoft Power BI**
* **Power Query** – Data cleaning and transformation
* **DAX** – Measures and calculations
* **Power BI Service** – Dashboard publishing and security configuration

---

## 📋 Project Workflow

The overall workflow followed in this project was:

```text
Raw Airline Data
       ↓
Data Cleaning & Preparation
       ↓
Data Modeling
       ↓
Calculated Columns & Transformations
       ↓
DAX Measures
       ↓
Interactive Visualizations
       ↓
Dashboard & Drillthrough
       ↓
Row-Level Security
       ↓
Power BI Service
       ↓
Business Insights
```

---

## 💡 Business Value

This project demonstrates how airline operational data can be transformed into an interactive business intelligence solution.

The dashboard enables users to examine airline performance, passenger distribution, ticket booking status, destinations, and flight performance from different perspectives. The addition of drillthrough functionality and Row-Level Security makes the solution more suitable for controlled, business-oriented reporting.

---

## 🎓 Learning Outcomes

Through this project, I gained practical experience in:

* Data cleaning and preparation using Power BI.
* Building relational data models.
* Creating one-to-many relationships.
* Creating calculated columns.
* Writing DAX measures.
* Designing interactive dashboards.
* Using slicers and drillthrough pages.
* Publishing reports to Power BI Service.
* Implementing Row-Level Security.
* Extracting and communicating business insights from data.

---

## 📌 Conclusion

The project demonstrates an end-to-end approach to **airline data analysis using Power BI**, starting from data preparation and relational modeling and progressing to DAX calculations, interactive dashboards, drillthrough analysis, and secure report sharing through Row-Level Security.

The resulting dashboard provides useful insights into airline operations and demonstrates how Power BI can be used to convert structured operational data into interactive and business-oriented analytical reports.
