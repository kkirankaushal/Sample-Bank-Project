# 🏦 Bank Transaction Analytics Dashboard

An interactive Tableau dashboard analyzing transaction patterns across U.S. states, merchant types, industries, and payment modes. This project provides actionable insights into consumer behavior, digital adoption, and state-level payment dynamics for banking and fraud intelligence teams.

---

## 📊 Dashboard Objectives

The dashboard is designed to address key business and operational questions:

1. **Transaction Distribution Across States**  
   Visualize state-by-state transaction volume and hotspots.

2. **Transaction Mode Analysis**  
   Understand usage patterns of Online, Offline, and Hybrid (OfflineWithHash) payment modes.

3. **Top Performing Merchants**  
   Identify the most active merchants by transaction volume.

4. **Industry-wise Trends**  
   Explore how different industries contribute to transaction volume and mode preference.

5. **Payment Method Distribution**  
   Analyze overall distribution and adoption of payment modes.

---

## 🗂️ Data Overview

The dashboard is built on aggregated transactional data grouped across multiple dimensions:

| Table | Description |
|-------|-------------|
| `agg_merchant` | Aggregated data by merchant name |
| `agg_industry` | Aggregated data by industry name |
| `agg_mop` | Aggregated by mode of payment (MOP) |
| `agg_state` | Aggregated by U.S. state |
| `agg_source` | Source-type level aggregation (e.g., platform/channel) |
| `agg_sic` | Aggregation by SIC code categories |
| `agg_merchant_industry` | Merged view of merchant and industry impact |
| `agg_state_industry` | State-level industry-specific breakdowns |

> Total Rows Processed: **281,197**

---

## 📍 Key Visuals in the Dashboard

- 🗺️ **Map**: Transaction counts by state with color-coded intensities  
- 📊 **Bar Charts**:
  - Transactions by mode for each state
  - Top 20 merchants by volume
  - Mode of payment share (%)
  - Industry-wise transaction comparison
- 📈 **Heatmaps**:
  - Industry vs State distribution matrix

---

## 🛠 Tools & Technologies

- **Tableau** (Desktop) – Interactive dashboard and visualizations
- **Microsoft Excel** – Source file for aggregated datasets
- **Python (Optional pre-aggregation)** – For advanced transformations (not included here)

---

## 💡 Insights Enabled

- Detect high-transaction states and their payment preferences
- Compare digital vs offline payment adoption regionally
- Identify merchants and industries driving volume
- Monitor transactional risk areas based on merchant/industry clusters

---

## 📁 Repository Structure

```bash
Bank-Transaction-Dashboard/
│
├── README.md
├── all_aggregated_tables.xlsx     # Source Excel file (aggregated sheets)
├── Bank_Transaction_Dashboard.twbx  # Tableau packaged workbook
└── Screenshots/
    └── dashboard-preview.png
