# Amazon Sale Data Analysis

## Project Overview

The Amazon Sale Analysis project is designed to analyze sales data from Amazon to identify key trends, performance metrics, and factors influencing sales. This project provides insights into customer behavior, product performance, and market dynamics using various data visualization techniques.

## Dataset

The dataset used in this analysis contains information about Amazon sales, including product details, quantities sold, order fulfillment, shipping details, and customer categories.

## Project Structure

- `Amazon Sale Report.csv`: The dataset file containing Amazon sales data.
- `analysis.ipynb`: Jupyter notebook with the code for data cleaning, transformation, analysis, and visualization.
- `README.md`: This file, providing an overview and documentation of the project.

## Steps Involved in the Project

1. **Data Loading and Cleaning:**
   - Loaded the dataset from a CSV file.
   - Removed unnecessary columns (`'New'`, `'PendingS'`).
   - Handled missing values by dropping rows with null entries.

2. **Data Transformation:**
   - Converted the `'ship-postal-code'` column to integer type.
   - Converted the `'Date'` column to datetime type.
   - Renamed columns for consistency.

3. **Descriptive Analysis:**
   - Generated summary statistics for key numerical columns (`'Qty'`, `'Amount'`).

4. **Categorical Analysis:**
   - Visualized the count of different product sizes using count plots.
   - Analyzed the total quantity sold by size category.
   - Visualized the distribution of courier statuses and fulfillment methods.
   - Created histograms for product categories.

5. **Geographical Analysis:**
   - Plotted the count of buyers by state and highlighted the top 10 states with the most buyers.

6. **Insights Extraction:**
   - Derived key insights from visualizations to understand buyer preferences and behaviors.

## Key Insights

- The majority of buyers prefer M-Size products.
- Most orders are fulfilled by Amazon and shipped via courier.
- Retail buyers constitute 99.2% of the customer base.
- Maharashtra has the highest number of buyers.

## Visualizations

- **Countplot of Sizes:**
  ![Countplot of Sizes](images/countplot_sizes.png)
  - Shows that most people buy M-Size items.

- **Bar Plot of Quantity by Size:**
  ![Bar Plot of Quantity by Size](images/barplot_qty_size.png)
  - Indicates that M-Size has the highest quantity sold.

- **Countplot of Courier Status by Status:**
  ![Countplot of Courier Status](images/countplot_courier_status.png)
  - Visualizes that most orders are shipped.

- **Histogram of Sizes:**
  ![Histogram of Sizes](images/histogram_sizes.png)
  - Plots the distribution of different sizes.

- **Histogram of Categories:**
  ![Histogram of Categories](images/histogram_categories.png)
  - Plots the distribution of product categories.

- **Pie Chart of B2B Data:**
  ![Pie Chart of B2B Data](images/piechart_b2b.png)
  - Shows that 99.2% of buyers are retailers.

- **Pie Chart of Fulfillment:**
  ![Pie Chart of Fulfillment](images/piechart_fulfillment.png)
  - Indicates that most orders are fulfilled by Amazon.

- **Scatter Plot of Category vs. Size:**
  ![Scatter Plot of Category vs. Size](images/scatterplot_category_size.png)
  - Visualizes the relationship between product category and size.

- **Countplot of Ship-State:**
  ![Countplot of Ship-State](images/countplot_ship_state.png)
  - Highlights that most buyers are from Maharashtra.

- **Countplot of Top 10 States:**
  ![Countplot of Top 10 States](images/countplot_top10_states.png)
  - Plots the distribution of buyers for the top 10 states.

## Conclusion

This project provides a comprehensive analysis of Amazon sales data, offering valuable insights into customer behavior and sales performance. The visualizations and insights derived from this analysis can help in understanding market trends and making informed business decisions.

## How to Run the Project

1. Clone this repository.
2. Install the required Python libraries:
   ```bash
   pip install pandas seaborn matplotlib
   ```
3. Run the Jupyter notebook `analysis.ipynb` to see the analysis and visualizations.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Feel free to customize this README file further based on your specific needs and project details.
