# Samsung Supply Chain & Logistics Dashboard

## Project Overview

This project is an interactive **Power BI dashboard** designed to analyze Samsung's supply chain and logistics performance. It brings together information about suppliers, inventory, shipments, customers, procurement, production, and sales to help users monitor key performance indicators (KPIs) and identify potential operational issues.

## Dashboard Preview

The dashboard provides a high-level overview of revenue, profit, order quantity, inventory value, shipment quantity, delivery quantity, supplier lead time, inventory stock, shipment delays, and revenue by customer.

> **Note:** The dashboard is a portfolio/demo project. Confirm the source and business meaning of the data before interpreting it as official Samsung reporting.

## Objectives

- Monitor revenue, profit, and profit margin.
- Review supplier lead times.
- Track inventory value and stock levels by product.
- Analyze shipment volume and delivery quantities.
- Identify carriers with higher shipment delays.
- Compare revenue across customers or sales channels.
- Present supply chain metrics in a single, interactive report.

## Tools & Technologies

- **Microsoft Power BI Desktop** — data modeling, DAX measures, visuals, and dashboard design
- **CSV files** — source data
- **Power Query** — data import and transformation (where used)
- **DAX** — measures and KPI calculations (where used)

## Dataset Structure

The project archive contains the following CSV files:

### Dimension tables

| File | Purpose |
|---|---|
| `dim_customer.csv` | Customer details |
| `dim_date.csv` | Calendar/date attributes for time-based analysis |
| `dim_facility.csv` | Facility or location information |
| `dim_product.csv` | Product details |
| `dim_supplier.csv` | Supplier details |

### Fact tables

| File | Purpose |
|---|---|
| `fact_inventory.csv` | Inventory and stock-related records |
| `fact_procurement.csv` | Procurement and purchasing records |
| `fact_production.csv` | Production-related records |
| `fact_sales.csv` | Sales and revenue records |
| `fact_shipment.csv` | Shipment and delivery records |

The exact fields, relationships, and calculation logic should be verified in the supplied data model and Power BI report.

## Dashboard Highlights

### KPI cards
- Gross revenue
- Total revenue
- Profit
- Profit margin
- Perfect order percentage
- Shipment count

### Analytical visuals
- **Supplier lead time:** compares average lead time across suppliers.
- **Inventory stock:** compares inventory value or stock levels across products.
- **Shipment delays:** compares shipment delay metrics across carriers.
- **Revenue comparison:** shows revenue by customer or sales channel.
- **Quantity indicators:** summarizes order, shipment, and delivered quantities.

### Navigation
The report design includes navigation sections for:
- Supplier information
- Inventory information
- Shipment information
- Customer information

## How to Use

1. Download or clone this repository.
2. Extract the project ZIP archive.
3. Open the `.pbix` file in **Power BI Desktop**.
4. If Power BI requests the source files, update the data-source paths to the extracted CSV files.
5. Select **Home → Refresh** to load the data.
6. Explore the report visuals and use available filters or slicers to investigate the metrics.

## Suggested Repository Structure

```text
samsung-supply-chain-dashboard/
├── README.md
├── dashboard/
│   └── Samsung_Supply_Chain_Dashboard.pbix
├── data/
│   ├── dim_customer.csv
│   ├── dim_date.csv
│   ├── dim_facility.csv
│   ├── dim_product.csv
│   ├── dim_supplier.csv
│   ├── fact_inventory.csv
│   ├── fact_procurement.csv
│   ├── fact_production.csv
│   ├── fact_sales.csv
│   └── fact_shipment.csv
└── images/
    └── dashboard-preview.png
```

*This is a suggested structure; rename folders and files to match the actual repository contents.*

## Business Value

This dashboard demonstrates how a BI report can bring multiple supply chain data areas together to support:
- Operational performance monitoring
- Inventory visibility
- Supplier and carrier comparisons
- Revenue and profitability analysis
- Faster identification of potential delays or unusual results

## Validation Notes

Before publishing or using the dashboard for business decisions:

- Verify the definitions and formulas behind each KPI.
- Confirm whether values such as revenue, profit, margin, lead time, and delay are calculated at the correct granularity.
- Check relationships between dimension and fact tables to avoid duplicate counting.
- Validate units, date ranges, missing values, and outliers.
- Confirm that the data is authorized for public sharing and does not contain confidential information.

## Disclaimer

This is an independent dashboard project created for learning and portfolio demonstration. Unless separately authorized, it should not be represented as an official Samsung report or as containing verified internal Samsung data. Samsung is referenced only to describe the subject of the dashboard.

## Author

**Kiran M**  
MBA — Finance & Business Analytics

For questions or suggestions, feel free to open an issue in the repository.
