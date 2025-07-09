# Supply Chain Management Data Analysis

## Overview
This project analyzes a supply chain dataset to uncover actionable insights for optimizing supply chain operations. The dataset includes information on product types, SKUs, pricing, availability, revenue, customer demographics, stock levels, lead times, shipping details, manufacturing costs, defect rates, and more. The analysis is performed using Python in a Jupyter Notebook, leveraging libraries such as `pandas`, `matplotlib`, `seaborn`, and `numpy`. The project generates at least 15 insights through statistical analysis, aggregations, and visualizations.

## Dataset
The dataset is provided in a CSV file named `supply_chain_data.csv`. It contains the following key columns:
- **Product type**: Type of product (haircare, skincare, cosmetics)
- **SKU**: Stock Keeping Unit identifier
- **Price**: Product price
- **Availability**: Product availability
- **Number of products sold**: Quantity sold
- **Revenue generated**: Total revenue per SKU
- **Customer demographics**: Target customer group (Male, Female, Non-binary, Unknown)
- **Stock levels**: Current stock
- **Lead times**: Time taken by suppliers to deliver
- **Shipping times**: Time for shipping
- **Shipping carriers**: Carrier used (Carrier A, B, C)
- **Shipping costs**: Cost of shipping
- **Supplier name**: Supplier identifier
- **Location**: Supplier location (Mumbai, Kolkata, Bangalore, Chennai, Delhi)
- **Manufacturing costs**: Cost of production
- **Inspection results**: Quality check outcome (Pass, Fail, Pending)
- **Defect rates**: Percentage of defective products
- **Transportation modes**: Mode of transport (Road, Rail, Air, Sea)
- **Routes**: Transportation route (Route A, B, C)
- **Costs**: Transportation costs

## Insights
The analysis provides the following insights:
1. **Revenue by Product Type**: Skincare products generate the highest revenue, followed by haircare and cosmetics.
2. **Top SKUs by Revenue**: Identifies top 5 SKUs contributing the most to revenue (e.g., SKU51, SKU98).
3. **Average Price by Product Type**: Skincare products have the highest average price.
4. **Defect Rates by Product Type**: Haircare products show the highest defect rates, indicating quality control issues.
5. **Supplier Performance**: Supplier 1 contributes the most to revenue.
6. **Lead Time by Supplier**: Supplier 2 has the longest average lead times, potentially impacting efficiency.
7. **Shipping Costs by Carrier**: Carrier A has the highest average shipping costs.
8. **Transportation Mode Costs**: Air transport is the most expensive mode.
9. **Inspection Results and Defects**: Products with "Fail" inspection results have higher defect rates.
10. **Stock Levels vs. Availability**: Moderate positive correlation between stock levels and availability.
11. **Customer Demographics**: Non-binary customers contribute significantly to revenue.
12. **Manufacturing Costs by Supplier**: Supplier 4 has the highest average manufacturing costs.
13. **Lead Time vs. Shipping Time**: Weak correlation, indicating production delays do not always affect shipping.
14. **Route Efficiency**: Route B has the highest transportation costs, suggesting optimization potential.
15. **Production Volumes vs. Defect Rates**: Weak negative correlation, indicating higher volumes do not necessarily increase defects.
16. **Bonus Insight - Location Impact**: Mumbai-based suppliers contribute significantly to revenue but have varied lead times.

## Prerequisites
To run the analysis, ensure you have the following installed:
- Python 3.8+
- Jupyter Notebook or JupyterLab
- Required Python libraries:
  ```bash
  pip install pandas matplotlib seaborn numpy
  ```

## Setup and Running the Project
1. **Clone or Download the Repository**:
   - If using a version control system, clone the repository. Otherwise, download the project files.
2. **Place the Dataset**:
   - Ensure the `supply_chain_data.csv` file is in the same directory as the Jupyter Notebook (`supply_chain_analysis.ipynb`).
3. **Open the Notebook**:
   - Launch Jupyter Notebook:
     ```bash
     jupyter notebook
     ```
   - Navigate to and open `supply_chain_analysis.ipynb`.
4. **Run the Notebook**:
   - Execute each cell sequentially to load the data, perform the analysis, and generate visualizations.

## Project Structure
- `supply_chain_data.csv`: Input dataset.
- `supply_chain_analysis.ipynb`: Jupyter Notebook containing the analysis code and visualizations.
- `README.md`: This file, providing project documentation.

## Outputs
- **Console Outputs**: Printed insights such as revenue by product type, defect rates, supplier performance, etc.
- **Visualizations**: Bar plots showing:
  - Revenue by product type
  - Defect rates by product type
  - Shipping costs by carrier
  - Transportation costs by mode
  - Revenue by customer demographics
  - Defect rates by inspection results
  - Lead time by supplier
  - Transportation costs by route


## Usage Notes
- The notebook assumes the CSV file is named `supply_chain_data.csv` and is located in the same directory.
- Data cleaning steps handle missing values and ensure numeric columns are properly formatted.
- Visualizations are displayed inline and saved to a file for reference.
- For deeper analysis, consider adding time-series analysis (if timestamps are available) or combining multiple variables (e.g., supplier and product type).

## Future Improvements
- Incorporate predictive modeling to forecast demand or defect rates.
- Analyze time-series trends if additional temporal data is provided.
- Optimize routes and carriers based on cost and time trade-offs.
- Explore supplier reliability by combining lead time and defect rate metrics.

## License
This project is for educational and analytical purposes. Ensure you have permission to use the dataset for your specific use case.