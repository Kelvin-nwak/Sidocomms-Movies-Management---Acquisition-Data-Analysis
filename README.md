# Sidocomms Movies Management - Acquisition Data Analysis

## Project Overview
This project provides a detailed analysis of **Sidocomms Movies Management** data in response to questions from a potential acquirer, **Elijah Moneybags**. The objective is to demonstrate an in-depth understanding of the business and its assets by leveraging SQL to extract key information from the Movies Database.

## Requirements
- **SQL Database**: Ensure you have a SQL-compatible database (e.g., MySQL, PostgreSQL).
- **Movies Database**: Use the provided `sample_data.sql` file in the `data/` directory to set up the database with necessary tables and data.

## Questions and SQL Queries
The project is organized to answer specific questions using multi-table SQL queries. Each query joins at least two tables to provide comprehensive insights.

### Query Descriptions
Each query is documented below, with additional explanations in their respective `.sql` files within the `SQL/` directory.

#### 1. List of Store Managers and Store Addresses
Retrieve the names of store managers along with each store's full address, including street, district, city, and country.

![SQL/query1_store_managers.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/31f2c47eaf0b43b59462f26397bbc1bfb56fdf5b/SQL/Q1.jpg)

#### 2. Inventory Details by Store
Provide a list of inventory items stocked in each store, with details such as store ID, inventory ID, film name, rating, rental rate, and replacement cost.

![SQL/query1_store_managers.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q2.jpg)

#### 3. Inventory Summary by Rating and Store
Roll up the inventory data to give a summary-level overview, showing the count of inventory items by rating at each store.

![SQL/query3_inventory_summary.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q3.jpg)

#### 4. Replacement Cost Analysis by Store and Category
Analyze the diversification of inventory based on replacement costs. Display the count of films, average replacement cost, and total replacement cost per store and film category.

![SQL/query4_replacement_cost_analysis.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q4.jpg)

#### 5. Customer Details with Store and Address
List all customer names, their associated store, active status, and full address, including street, city, and country.

![SQL/query5_customers.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q5.jpg)

#### 6. Customer Lifetime Value Analysis
Identify the most valuable customers by calculating the total number of rentals and the total payments collected. Order this by total lifetime value, showing the most valuable customers at the top.

![SQL/query6_customer_value.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q6.jpg)

#### 7. Board of Advisors and Investors
Provide a list of board members, specifying whether each is an investor or advisor. Include the associated company for each investor.

![SQL/query7_advisors_investors.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q7.jpg)

#### 8. Awarded Actors Coverage Analysis
Determine the coverage of awarded actors in the inventory. Calculate the percentage of actors with awards for whom there are films in the inventory, broken down by actors with two types of awards and those with only one award.

![SQL/query8_awarded_actors_coverage.sql](https://github.com/Kelvin-nwak/Sidocomms-Movies-Management---Acquisition-Data-Analysis/blob/b449e6801b9dd10a1d2bf2083e98202e7d87aed8/SQL/Q8.jpg)

## Setup Instructions
1. **Database Setup**: Use the provided `sample_data.sql` file to create and populate the Movies Database.
    ```bash
    mysql -u [username] -p [database_name] < data/sample_data.sql
    ```
2. **Execute Queries**: Run the SQL queries individually in your SQL client or terminal to retrieve answers to each question.

## Usage
- **Extract Data**: Execute each SQL file to extract the specific data needed for the analysis.
- **Analyze**: Review and analyze the output from each query to gain insights into Sidocomms Movies Management’s inventory, customer base, financials, and other key aspects.

## Contributing
Pull requests are welcome. For significant changes, please open an issue first to discuss your ideas.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
