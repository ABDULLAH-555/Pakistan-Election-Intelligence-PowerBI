**Strategic Election Intelligence Dashboard (1970 - 2024) 🗳️📈**

**Project Overview**
This repository contains a high-performance Power BI dashboard analyzing 54 years of Pakistan's electoral history. The project transforms raw data from the Gallup Pakistan Elections Database into a strategic intelligence tool, focusing on the competitive shifts and geospatial trends of the 2024 General Elections.

**Key Features**
Historical Ribbon Analysis: Visualizes power shifts across 11 general elections.

Geospatial Mapping: Interactive district-level winners with dynamic turnout gauges.

AI-Driven Root Cause Analysis: Utilizes Decomposition Trees to drill down into 2024 vote distributions.

Battleground Metrics: Custom DAX measures identifying high-competition seats based on victory margins.

Technical Architecture
Data Engineering
Normalization: Processed and cleaned datasets involving 400+ political entities.

Geospatial Cleaning: Developed a unified "Full Location" string to ensure 100% mapping accuracy for Pakistani districts.

Analytical Logic (DAX)
Highlights of the custom logic implemented:

Winning Margin: CALCULATE(MAX(Votes) - RunnerUpVotes)

Dynamic Year Headers: FORMAT(MAX(Year), "0")

Winning Party Identifier: Logical branching to isolate winners at the constituency level.

UI/UX Design
Aesthetic: Dark Mode "Command Center" theme.

Interactivity: Cross-filtering, Sync Slicers, and Drill-through to candidate-specific details.

**How to View**
Download the .pbix file.

Open with Power BI Desktop.

(Optional) View the PDF export in the Screenshots/ folder for a quick overview.
