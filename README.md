# Automated 8760-Hour Steady-State Reliability & Curtailment Assessment

## Overview
This project, developed for **ENEL 678**, implements an automated **Python–PSS®E framework** to perform large-scale steady-state reliability assessments of the **Southeast Alberta transmission grid**.

With increasing integration of **renewable energy resources (wind and solar)**, modern power systems face operational challenges such as **thermal congestion** and **voltage stability risks**.

This project performs **8760-hour AC power-flow simulations** using hourly generation profiles to identify network bottlenecks and evaluate the curtailment required to maintain reliable grid operation.

---

## Key Features

- **8760-Hour Automation**  
  Automated hourly simulation loop using AESO generation profiles.

- **N-0 / N-1 Contingency Analysis**  
  Detects transmission bottlenecks and reliability violations.

- **Automated Congestion Relief (ACCOR)**  
  Calculates required generation curtailment to resolve overloads.

- **Data-Driven Insights**  
  Generates congestion rankings and voltage violation heatmaps.

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
        B1[8760 Hourly Loop]
        B2[N-0/N-1 Analysis]
        B3[Automated ACCOR Curtailment]
    end

    subgraph C [Outputs]
        C1[Congestion Ranking]
        C2[Curtailment Logs]
        C3[Voltage Heatmaps]
    end

    A --> B
    B --> C

##Tech Stack
Simulation

PSS®E (AC Power Flow & Contingency Analysis)

Automation

Python

PSS®E API

Data Processing

Pandas

NumPy

Visualization

Matplotlib

Streamlit

##Project Structure
project-root
│
├── data/        # AESO hourly profiles and PSS/E base cases
├── scripts/     # Python automation and simulation scripts
├── outputs/     # Generated results (curtailment logs, rankings, heatmaps)
└── docs/        # Technical documentation

##Outputs

The framework generates:

Transmission congestion rankings

Generation curtailment logs

Voltage violation heatmaps

Annual reliability insights

These outputs help analyze how renewable generation impacts grid reliability and transmission constraints.

##Project Status

 Work in Progress

Current development stage includes:

Technical design roadmap

AESO data preparation

8760-hour automation framework

Violation detection and ACCOR integration

    A --> B
    B --> C
