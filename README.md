# Automated 8760-Hour Steady-State Reliability & Curtailment Assessment

## Project Overview

The aim of the project is to to build an automated **Python–PSS®E framework** for performing large-scale steady-state reliability analysis of the **Southeast Alberta transmission network**.

With increasing integration of **renewable energy resources (wind and solar)**, power systems face operational challenges such as **thermal congestion, voltage violations, and generation curtailment requirements**.

This project performs **8760-hour AC power flow simulations** using hourly generation profiles to evaluate network constraints and determine the required curtailment needed to maintain reliable system operation.


## Key Features

- **8760-Hour Automated Simulation**
  - Hourly AC power flow simulation for a full year.

- **N-0 / N-1 Contingency Analysis**
  - Detects system violations under normal and contingency conditions.

- **Automated Congestion Relief (ACCOR)**
  - Automatically calculates generation curtailment required to resolve overloads.

- **Data-Driven Grid Insights**
  - Congestion ranking of transmission elements
  - Voltage violation heatmaps
  - Curtailment logs

## Workflow



## Project Structure

- data/ – Stores AESO hourly profiles and PSS®E cases.
- scripts/ – Contains automation routines, contingency analysis modules, and curtailment logic.
- outputs/ – Stores results such as curtailment logs, congestion rankings, and voltage heatmaps.
- docs/ – Technical documentation detailing methodology, assumptions, and implementation.

## Outputs

- Transmission Congestion Rankings – Identify the most constrained elements in the network.
- Generation Curtailment Logs – Track renewable energy curtailment to maintain reliability.
- Voltage Violation Heatmaps – Visualize areas of concern in the network.
- Annual Reliability Insights – Summarize system performance over the full year.

## Project Status
Work in Progress
- Current tasks:
  - Building 8760-hour automation framework,
  - Integrating violation detection and curtailment logic

- Next steps: validation, performance analysis, and reporting.

## Tech Stack
- Simulation: PSS®E
- Automation: Python, PSS®E API
- Data Processing: Pandas, NumPy
- Visualization: Matplotlib, Streamlit
