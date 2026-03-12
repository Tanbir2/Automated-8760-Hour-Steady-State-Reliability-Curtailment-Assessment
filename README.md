# Automated 8760-Hour Steady-State Reliability & Curtailment Assessment

## Project Overview

This project was developed for **ENEL 678** to build an automated **Python–PSS®E framework** for performing large-scale steady-state reliability analysis of the **Southeast Alberta transmission network**.

With increasing integration of **renewable energy resources (wind and solar)**, power systems face operational challenges such as **thermal congestion, voltage violations, and generation curtailment requirements**.

This project performs **8760-hour AC power flow simulations** using hourly generation profiles to evaluate network constraints and determine the required curtailment needed to maintain reliable system operation.

---

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

---

## Workflow

```mermaid
graph LR
    subgraph A [Input Layer]
        A1[AESO Hourly Profiles]
        A2[PSS/E Base Case]
        A3[Mapping Tables]
    end

    subgraph B [Processing Engine]
        B1[8760 Hourly Simulation Loop]
        B2[N-0/N-1 Contingency Analysis]
        B3[Automated Curtailment Logic]
    end

    subgraph C [Outputs]
        C1[Congestion Ranking]
        C2[Curtailment Reports]
        C3[Voltage Heatmaps]
    end

    A --> B
    B --> C
