# SummerAnalytics2025
# Dynamic Pricing for Urban Parking Lots

Capstone Project – Summer Analytics 2025 

---

## Overview

Urban parking spaces in cities are limited and often priced inefficiently. Static pricing leads to either congestion during peak hours or underutilization during low demand. This project aims to design an intelligent, real-time dynamic pricing engine for 14 urban parking lots using real-time simulation, machine learning logic, and demand theory, with the goal of optimizing occupancy and pricing based on actual and predicted demand.

---

## Tech Stack

| Component              | Stack/Tool               |
|------------------------|--------------------------|
| Programming Language   | Python 3                 |
| Data Manipulation      | Pandas, NumPy            |
| Streaming Engine       | [Pathway](https://pathway.com) |
| Visualization          | Bokeh                    |
| Notebook Environment   | Google Colab             |
| Version Control        | Git + GitHub             |

---

## Project Architecture (Mermaid Diagram)

```mermaid
graph TD
    A[Raw CSV Dataset] --> B[Data Preprocessing (Pandas)]
    B --> C[Model 1: Linear Pricing]
    B --> D[Model 2: Demand-Based Pricing]
    B --> E[Model 3: Competitive Geo Pricing]
    C --> F[Price Stream Generator]
    D --> F
    E --> F
    F --> G[Pathway Engine]
    G --> H[Bokeh Dashboard (Real-time Visualization)]
