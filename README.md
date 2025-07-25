# Retail-Sales-Dashboard Using R Programming
Retail Sales Dashboard
This project provides an interactive retail sales dashboard built using R and Shiny. It offers various insights into sales performance, customer behavior, and product trends based on a sample sales dataset.

Features
Overall Sales Summary: Displays key metrics such as total sales, total orders, total units sold, and total products sold.

Top Products Analysis: Identifies the top 5 products by sales.

Sales vs. Returns by Product Category: Visualizes the sales and returns for different product lines, helping to identify categories with high return rates.

Customer Behavior Analysis: Lists the top 10 customers based on their total sales.

Monthly Sales Trend: Shows the sales performance over time, allowing for the identification of seasonal trends or significant changes.

Regional Sales Performance: Breaks down sales by country, highlighting top-performing regions.

Project Structure
sales_data_sample.csv: The raw dataset containing sales information.

retail_sales_dashboard.Rmd: An R Markdown file that contains the R code for data loading, pre-processing, analysis, and generating the plots.

app.R: The Shiny application script that builds the interactive dashboard, integrating the analysis and visualizations from retail_sales_dashboard.Rmd.

Retail_Sales_Dashboard.Rproj: RStudio project file for easy project management.

category_sales_vs_returns.png: Generated plot showing sales vs returns by product category.

sales_over_time.png: Generated plot showing monthly sales over time.

sales_by_country.png: Generated plot showing sales by country.

Setup and Usage
To run this project locally, you will need R and RStudio installed.

Prerequisites
R: Download and install R from CRAN.

RStudio: Download and install RStudio Desktop from RStudio.

Installation
Clone the repository (or download the files):
If this were a Git repository, you would clone it. Since you've provided the files, ensure all the files (sales_data_sample.csv, retail_sales_dashboard.Rmd, app.R, Retail_Sales_Dashboard.Rproj) are in the same directory.

Install R Packages:
Open app.R in RStudio. You might need to install the required R packages. Run the following commands in the R console:

install.packages(c("shiny", "dplyr", "ggplot2", "tidyr", "scales"))

Running the Dashboard
Open the Project:
Open the Retail_Sales_Dashboard.Rproj file in RStudio. This will set your working directory correctly.

Run the Shiny App:
Open the app.R file. Click the "Run App" button in the top-right corner of the RStudio script editor, or run the following command in the R console:

shiny::runApp("app.R")

This will launch the interactive sales dashboard in your default web browser or in RStudio's Viewer pane.

Data Source
The dashboard uses sales_data_sample.csv, which is a sample retail sales dataset.

Analysis Details
The retail_sales_dashboard.Rmd file contains the detailed R code for:

Loading and initial inspection of the sales_data_sample.csv.

Calculating summary statistics.

Performing data transformations (e.g., converting ORDERDATE to Date objects).

Aggregating data for top products, customer behavior, monthly trends, and regional sales.

Generating static plots using ggplot2 (these are then integrated into the Shiny app).

The app.R file then takes these pre-calculated summaries and reactive elements to create the interactive user interface.
