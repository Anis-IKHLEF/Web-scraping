Description

This script performs the following tasks:

Scrapes Amazon Bestsellers: It starts by scraping the main Amazon Bestsellers page (https://www.amazon.fr/gp/bestsellers/?ref_=nav_em_cs_bestsellers_0_1_1_2) to retrieve links to the top categories.

Navigates through each category: It extracts the product data for each category and page of bestsellers.

Extracts product details: For each product, it retrieves the following:

Product Name

Rating (if available)

Price (if available)

Handles pagination: The script follows pagination links to scrape products across multiple pages within each category.

Stores data in JSON: After collecting the product information, it stores the data in a JSON format file for further use.

How It Works

Scraping Amazon Categories:

The script fetches the main bestsellers page and identifies all the available product categories by looking for anchor tags with the class a-link-normal.

Iterating Through Products:

For each category, the script fetches the products listed in that category by visiting the category page.

For each product, it retrieves the name, rating, and price if available. If no price is found, it assigns the price as None.

Handling Pagination:

The script handles pagination to ensure that all pages in a category are scraped.

Saving Data in JSON:

All collected data is stored in a file.json file, formatted in a structured and readable way using Python's json.dump() method.

NB : The website might change the selectors, you to change it if necessary.
