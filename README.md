# 🚚 Supply Chain OS — Logistics & Warehouse Intelligence Platform

[![Streamlit App](https://static.streamlit.io/badges/streamlit_badge_black_white.svg)](https://supplyd.streamlit.app/)
[![Python](https://img.shields.io/badge/Python-3.9%2B-blue.svg)](https://www.python.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

An enterprise-grade Data Engineering and Analytics platform built with Python, SQLite, Plotly, and Streamlit. **Supply Chain OS** ingests relational supply chain datasets in real-time, executing SQL analytical transformations to deliver interactive metrics on logistics spend, transit delays, warehouse inventory health, and predictive delay simulation.

🔗 **Live Application:** [https://supplyd.streamlit.app/](https://supplyd.streamlit.app/)

---

## 📊 Modules & Capabilities

### 1. 📌 Executive Logistics Control Center
* **KPI Metrics**: Real-time tracking of active shipments, overall on-time delivery percentage, average transit delays, and total freight expenditure.
* **Cost vs. Distance Analysis**: Scatter visualizer evaluating logistics cost trajectories across multiple transportation modes.
* **Delay Root-Cause Breakdown**: Interactive pie distribution highlighting core operational bottlenecks (weather, customs, carrier availability, etc.).

### 2. 🚛 Delivery Delay & Carrier Performance
* **Modal Delay Diagnostics**: Comparative breakdown of average transit delays grouped by transport modes (*Road, Air, Rail, Express Highway*).
* **Customer Satisfaction Scoring**: Box plots analyzing correlation between shipment delays and post-delivery satisfaction ratings.

### 3. 📦 Warehouse Inventory Analytics
* **Valuation by Category**: Aggregated stock valuation metrics across product categories.
* **Safety Stock & Reorder Analysis**: Bivariate analysis comparing available inventory against dynamic reorder thresholds.

### 4. ⚡ Real-Time Delay Risk Simulator
* **Interactive Parameter Tuning**: Adjust shipment distance, transport mode, and priority level using live input controls.
* **Predictive Delay Calculation**: Algorithmic delay estimation engine assisting logistics dispatchers in proactive risk management.

---

## 🛠️ Tech Stack & Architecture

* **Frontend UI**: [Streamlit](https://streamlit.io/) with custom CSS injection for dark mode & high-contrast typography.
* **Database / Execution Engine**: In-memory `sqlite3` relational database execution engine.
* **Data Processing**: `pandas`, `numpy`.
* **Data Visualization**: `plotly.express`, `plotly.graph_objects`.

---

## 📁 Project Directory Structure

```text
├── app.py                          # Primary Streamlit application entry point
├── requirements.txt                 # Application dependencies
├── README.md                        # Documentation
└── data/                            # Relational CSV datasets
    ├── 1_warehouses_large.csv
    ├── 2_suppliers_large.csv
    ├── 3_products_large.csv
    ├── 4_inventory_large.csv
    ├── 5_orders_large.csv
    ├── 6_order_items_large.csv
    ├── 7_carriers_large.csv
    ├── 8_shipments_large.csv
    ├── 9_delivery_tracking_large.csv
    └── 10_returns_damages_large.csv
