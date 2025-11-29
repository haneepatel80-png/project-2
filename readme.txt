Power BI Data Modeling Project Overview This repository contains the Power BI data modeling project illustrating schema design, relationship management, model enhancement, and validation using a matrix visual.

Project Structure Data Import & Cleaning

Import all files using Power Query.

Ensure correct data types and remove blank rows.

Load cleaned data into the data model.

Model Construction & Relationships

Define primary and foreign keys manually.

Relationships:

Sales_Fact → Customer_Dim

Sales_Fact → Product_Dim

Sales_Fact → Region_Dim

Sales_Fact → Date_Dim

Returns_Fact → Sales_Fact

Returns_Fact → Date_Dim (inactive for ReturnDateKey)

Schema Design

Star schema centered on Sales_Fact.

Model Returns_Fact as snowflake or separate fact table.

Demonstrate cardinality (1:Many, Many:1, 1:1).

Advanced Model Settings

Relationship cardinalities and cross-filter directions.

Bidirectional filters as justified.

Filter ambiguity resolution.

Data Model Enhancements

Set appropriate data formats (currency, dates, etc.).

Define data categories for sorting.

Hierarchies:

Date_Dim: Year > Quarter > Month > Date

Region_Dim: Country > State > City

Product_Dim: Category > Subcategory > ProductName

Verification

Use Matrix visual for:

Sales by Product Category/Region

Returns by Fiscal Year/Reason

Revenue by Customer Segment

Deliverables .pbix Power BI file with:

Transformed tables via Power Query

All model relationships

Hierarchies and cleaned fields

Matrix table for verification

Project summary document (.docx/.txt) addressing:

Schema type and rationale

Relationship logic and filter flow

Issues encountered and solutions

Getting Started Clone this repository.

Open the .pbix file in Power BI Desktop.

Refer to the summary document for design and logic explanation.

Deadline Submission Date: May 10, 2025 (EOD)

License This project is licensed for educational and demonstration use. All original data sources respected.

This template follows standard repository documentation and can be expanded with sections for installation instructions, data sources, or additional visuals as needed.


Status

Co
