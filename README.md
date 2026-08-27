# 🗳️ Strategic Election Intelligence Dashboard — Pakistan (1970–2024)

> **A Power BI-based electoral intelligence dashboard analyzing 54 years of Pakistan's electoral history, with a strategic focus on constituency-level competition, political shifts, turnout, and the 2024 General Elections.**

---

## 📌 Project Overview

The **Strategic Election Intelligence Dashboard** transforms historical electoral data from the **Gallup Pakistan Elections Database** into an interactive business-intelligence and analytical platform.

Spanning **11 General Elections from 1970 to 2024**, the dashboard combines historical election analysis, constituency-level results, geospatial visualization, DAX-driven metrics, and interactive Power BI features to identify **political power shifts, competitive constituencies, winning margins, turnout patterns, and 2024 electoral trends**.

The project demonstrates an end-to-end workflow covering **data cleaning, transformation, modeling, analytical logic, visualization, and dashboard UX design**.

---

## 🎯 Project Objectives

* Analyze Pakistan's electoral history from **1970–2024**
* Identify long-term **political power shifts**
* Analyze constituency-level winners and vote distributions
* Identify **highly competitive/battleground constituencies**
* Compare winning margins between candidates
* Analyze voter turnout across districts
* Provide interactive **geospatial election intelligence**
* Enable drill-down analysis of candidates, parties, constituencies, and elections
* Build a reusable analytical framework using **Power BI and DAX**

---

## 📊 Key Features

### 🏛️ Historical Election Analysis

A **Ribbon Chart** visualizes the evolution of political parties across 11 General Elections, allowing users to track changes in electoral dominance and political positioning over time.

**Coverage:**

`1970 → 1977 → 1985 → 1988 → 1990 → 1993 → 1997 → 2002 → 2008 → 2013 → 2018 → 2024`

---

### 🗺️ Geospatial Election Intelligence

Interactive district-level mapping provides a geographical view of electoral outcomes.

The dashboard enables users to:

* Identify district-level winners
* Analyze turnout geographically
* Compare electoral performance
* Explore regional voting patterns
* Filter results dynamically by election year and political entity

A standardized **Full Location** field was engineered to improve geographic matching and ensure reliable mapping across Pakistani districts.

---

### 🌳 AI-Style Root Cause Analysis

Power BI **Decomposition Trees** are used to break down 2024 electoral results into multiple analytical dimensions.

Users can drill from high-level vote distributions into factors such as:

**Election → Province → District → Constituency → Party/Candidate → Votes**

This provides an exploratory approach to understanding the drivers behind electoral outcomes.

---

### ⚔️ Battleground / Competitive Seat Analysis

Custom DAX measures identify constituencies where electoral competition was particularly close.

The dashboard evaluates:

* Winning votes
* Runner-up votes
* Winning margin
* Candidate competitiveness
* Constituency-level vote distribution

This makes it possible to identify **battleground constituencies** where relatively small vote differences determined the outcome.

---

## ⚙️ Technical Architecture

### 🔹 Data Engineering

The dataset required substantial preprocessing and normalization before visualization.

Key data-engineering tasks included:

* Data cleaning and standardization
* Handling inconsistent political entity names
* Normalizing election-year structures
* Processing **400+ political entities**
* Standardizing constituency and district information
* Cleaning geographic identifiers
* Creating unified location fields
* Preparing data for Power BI's data model

### 🔹 Geospatial Data Cleaning

A unified **Full Location** field was developed to improve district-level mapping consistency.

This helped resolve variations in location naming and enabled more reliable geographic visualization across the dashboard.

---

## 🧮 Analytical Logic — DAX

Several custom DAX measures were developed to power the dashboard's analytical layer.

### Winning Margin

The dashboard calculates the difference between the winning candidate's votes and the runner-up's votes:

```DAX
Winning Margin =
[Winning Votes] - [Runner Up Votes]
```

### Dynamic Year Header

The dashboard dynamically displays the selected election year:

```DAX
Dynamic Year Header =
FORMAT(MAX('Election Data'[Year]), "0")
```

### Winning Party Identification

Logical DAX expressions were implemented to identify the winning political party at constituency level based on vote performance.

These measures allow the dashboard to dynamically respond to filters and drill-down selections.

---

## 🎨 UI/UX Design

### Command Center Theme

The dashboard uses a **dark-mode strategic command-center aesthetic**, designed to resemble an electoral intelligence and analytical operations interface.

### Interactive Features

* 🎛️ Dynamic slicers
* 🔄 Synchronized slicers
* 🔍 Cross-filtering
* 🧭 Drill-through navigation
* 📊 Interactive charts
* 🗺️ Geographic visualization
* 🌳 Decomposition Tree analysis
* 👤 Candidate-level detail views
* 📈 Dynamic KPI cards

The design prioritizes **information density, analytical clarity, and interactive exploration**.

---

## 🛠️ Technology Stack

| Category            | Technologies                                |
| ------------------- | ------------------------------------------- |
| BI & Visualization  | **Microsoft Power BI**                      |
| Data Transformation | **Power Query**                             |
| Analytical Language | **DAX**                                     |
| Data Source         | **Gallup Pakistan Elections Database**      |
| Data Cleaning       | Power Query / Data Transformation           |
| Visualization       | Power BI Charts, Maps & Decomposition Trees |
| Data Modeling       | Power BI Data Model                         |
| Geospatial Analysis | District / Constituency Location Mapping    |

---

## 📈 Analytical Highlights

The dashboard provides insights into:

* **54 years** of Pakistan's electoral history
* **11 General Elections**
* **400+ political entities**
* Constituency-level electoral outcomes
* District-level winners
* Winning margins
* Runner-up performance
* Voter turnout
* Political party transitions
* Regional electoral patterns
* 2024 competitive constituencies

---

## 📂 Project Structure

```text
Strategic-Election-Intelligence/
│
├── 📊 Power BI/
│   └── Election_Intelligence_Dashboard.pbix
│
├── 📸 Screenshots/
│   └── dashboard-overview.pdf
│
├── 📁 Dataset/
│   └── election-data.*
│
└── 📄 README.md
```

> Dataset files may be excluded from the repository depending on licensing and redistribution restrictions.

---

## 🚀 How to View the Dashboard

### Option 1 — Power BI Desktop

1. Download or clone this repository.
2. Open the `.pbix` file using **Power BI Desktop**.
3. Refresh the dataset if required.
4. Interact with slicers, maps, charts, and drill-through pages.

### Option 2 — PDF Preview

A PDF export is available in the `Screenshots/` directory for users who want to quickly review the dashboard without opening Power BI.

---

## 🔍 Dashboard Navigation

The dashboard is structured around several analytical perspectives:

**Historical Overview**

→ Explore electoral changes across decades.

**2024 Election Intelligence**

→ Analyze constituency-level results and party performance.

**Geospatial Analysis**

→ Explore district-level winners and turnout.

**Battleground Analysis**

→ Identify closely contested constituencies using winning margins.

**Candidate Analysis**

→ Drill through to candidate-specific electoral performance.

---

## 💡 What This Project Demonstrates

This project showcases practical capabilities in:

* Data cleaning & transformation
* Data modeling
* Power BI dashboard development
* Advanced DAX
* Geospatial analytics
* Electoral data analysis
* Interactive visualization
* KPI development
* Analytical storytelling
* Dashboard UX/UI design
* Large-scale historical data analysis

---

## 👨‍💻 Project Focus

**Domain:** Political & Electoral Data Analytics
**Platform:** Microsoft Power BI
**Analysis Period:** 1970–2024
**Primary Focus:** Pakistan General Elections
**Dashboard Type:** Interactive Strategic Intelligence Dashboard

---

## ⭐ Project Value

Rather than presenting election results as static tables, this project converts historical electoral data into an **interactive intelligence system** where users can move from national-level trends to districts, constituencies, candidates, and competitive margins.

The goal is to demonstrate how **data engineering + analytical modeling + DAX + visualization** can transform complex historical datasets into actionable analytical insights.

---

## 📌 Data Source

Electoral data was sourced from the **Gallup Pakistan Elections Database**.

Please refer to the original data provider for information regarding data ownership, methodology, and permitted use.

---

## 📬 Feedback & Collaboration

If you have suggestions, identify data-quality issues, or would like to collaborate on extending the dashboard with additional electoral or demographic analysis, feel free to open an issue or submit a pull request.

---

### ⭐ If you find this project useful, consider starring the repository!
