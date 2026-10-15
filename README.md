# 🏥 Hospital Operations Analytics using MySQL & SQL

## 📌 Project Overview

This project focuses on analyzing hospital operations using a relational database built in **MySQL**. It explores patient demand, appointment patterns, treatment performance, doctor workload, room utilization, and appointment-related operational issues.

The project demonstrates a practical SQL data analysis workflow, including relational database design, importing structured data, joining tables, aggregating records, filtering results, and extracting meaningful operational insights.

---

## 🎯 Problem Statement

Hospitals manage large amounts of connected information about patients, appointments, doctors, treatments, and rooms. Without structured analysis, it can be difficult to understand demand, monitor waiting times, allocate resources, and identify appointment management issues.

This project uses SQL queries to explore these operational patterns and support more informed, data-driven planning.

---

## 🎯 Project Objectives

* Design a relational database for hospital patient-care operations.
* Import and manage structured hospital data using MySQL.
* Analyze appointment demand by city, service type, priority, and booking channel.
* Understand patient appointment frequency and booking behaviour.
* Evaluate treatment outcomes, waiting time, and treatment duration.
* Assess doctor workload and room utilization.
* Identify cancellations, no-shows, rescheduling, and repeat treatment attempts.
* Use SQL joins, aggregations, filtering, and subqueries to derive insights.

---

## 🛠️ Technologies Used

* MySQL
* MySQL Workbench
* SQL
* CSV files for structured data import
* Relational database design
* Entity-Relationship (ER) modeling

---

## 🗄️ Database Overview

The project uses a database named `hospital_analytics` with **5 relational tables**.

| Table | Description |
|---|---|
| `patients` | Patient details such as name, age, gender, city, patient type, preferred time slot, and registration date |
| `appointments` | Appointment date, patient, doctor, service type, priority, estimated cost, and booking channel |
| `doctors` | Doctor name, specialty, hire date, rating, employment type, and active status |
| `rooms` | Room type, floor, equipment type, capacity, maintenance date, and availability |
| `treatments` | Appointment, doctor, room, treatment date, status, attempt number, treatment duration, waiting time, and treatment cost |

### 📊 Dataset Size

The project presentation describes the following synthetic dataset:

* **400 Patients**
* **3,000 Appointments**
* **3,500 Treatments**
* **80 Doctors**
* **50 Rooms**

Primary and foreign keys connect the tables to support relational analysis.

---

## 🔍 SQL Analysis Performed

### 1. Basic Analysis & Data Exploration

* Counted the total number of patients.
* Analyzed appointment counts across medical service types.
* Used aggregate functions to summarize hospital data.

### 2. Patient & Appointment Demand

* Compared appointment volume across cities.
* Analyzed appointments by service type and priority.
* Explored differences in demand across locations and services.

### 3. Patient Appointment Behaviour

* Identified patients with higher cumulative estimated appointment value.
* Found patients with exactly one appointment.
* Explored patient appointment frequency and booking behaviour.

### 4. Treatment Performance

* Calculated average, minimum, and maximum treatment duration.
* Calculated average, minimum, and maximum waiting time.
* Compared treatment usage across room types.

### 5. Doctor & Room Performance

* Compared doctor treatment counts.
* Reviewed doctor ratings alongside treatment assignments.
* Identified room types with higher treatment usage.

### 6. Appointment & Treatment Problems

* Counted rescheduled, cancelled, and no-show cases.
* Compared cancellation counts by doctor.
* Identified patterns that may need further operational investigation.

---

## 📈 Key Insights

The following findings are reported in the project presentation and apply to the synthetic dataset used:

* **Consultation** had the highest appointment volume, with **1,183 appointments**.
* **Diagnostic Test** had **627 appointments**, followed by **Follow-up** with **539**, **Procedure** with **439**, and **Emergency Care** with **212**.
* **Kochi** had the highest appointment volume among the displayed cities, with **440 appointments**. Pune had the lowest among those displayed, with **334**.
* Patient **P0216** had the highest cumulative estimated appointment value in the displayed top-10 results: **81,348.37**.
* Average treatment duration was **38.72 minutes**.
* Average waiting time was **15.62 minutes**.
* Treatment duration ranged from **5 to 173 minutes**, while waiting time ranged from **0 to 90 minutes**.
* **Observation rooms** had the highest reported treatment usage, with **902 treatments**.
* **Dr. Doctor_080** had the highest displayed treatment count, at **66**.
* The reported problem-status counts were **366 rescheduled**, **283 cancelled**, and **251 no-show** cases.
* Doctor **D033** had the highest displayed cancellation count, with **9**.

These results describe patterns in the supplied synthetic data; they do not establish the causes of operational issues or represent real hospital performance.

---

## 💼 Business Use Cases

### For Hospital Administrators

* Understand patient demand across cities and services.
* Support appointment scheduling and service planning.
* Identify operational patterns that may need attention.

### For Operations Teams

* Monitor waiting times and treatment duration.
* Review room utilization and doctor workload.
* Investigate cancellation, rescheduling, and no-show patterns.

### For Resource Planning

* Compare the use of different room types.
* Understand variation in doctor treatment assignments.
* Use data-driven findings to inform resource-allocation discussions.

---

## 🧠 SQL Concepts Demonstrated

* `SELECT` and `WHERE`
* `COUNT()`, `SUM()`, `AVG()`, `MIN()`, and `MAX()`
* `GROUP BY` and `HAVING`
* `ORDER BY` and `LIMIT`
* `INNER JOIN` and `LEFT JOIN`
* Filtering with `IN`
* Aggregations across related tables
* Primary keys and foreign keys
* Relational database design

---

## 🚀 How to Run the Project

1. Install **MySQL Server** and **MySQL Workbench**.
2. Clone or download this repository.
3. Open MySQL Workbench and connect to your MySQL server.
4. Create or import the `hospital_analytics` database schema.
5. Import the CSV files for the five tables, if they are included in the repository.
6. Verify that the data has been imported correctly and that primary-key and foreign-key relationships are configured.
7. Open the SQL analysis script and run the queries against the `hospital_analytics` database.
8. Review the query outputs and compare them with the findings in the project presentation.

*Note: To run the project from a fresh clone, the repository must include the required schema, data files, and SQL queries. Add these files if they are not already present.*

---

## 🔮 Future Improvements

* Add SQL scripts to create the database and tables from scratch.
* Include reproducible data-import instructions and validation queries.
* Add data-quality checks for missing values, duplicate IDs, and invalid dates.
* Build a Power BI dashboard to visualize hospital operational KPIs.
* Explore time-based trends if the dataset contains sufficient date information.
* Document query assumptions and metric definitions.

---

## 📚 Skills Demonstrated

* SQL Querying
* MySQL Database Management
* Relational Database Design
* Data Exploration
* Data Aggregation
* Joins and Subqueries
* Operational Data Analysis
* Business Insight Generation

---

## 👨‍💻 Authors

**Mohit Chaudhari**  
**Monesh Chaudhari**

**LinkedIn:** https://www.linkedin.com/in/mohit-chaudhari-028301259/

**GitHub:** https://github.com/Mohit242004

---

## ⭐ If you found this project useful, don't forget to Star this repository!
