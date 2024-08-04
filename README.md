# internal-link-analysis-seo
This script uses pandas for data manipulation and analysis, and assumes you have your crawl data in a CSV file with at least two columns: source_url (the page where the link is located) and target_url (the page that is being linked to).

Load the Data: Load your crawl data from a CSV file. The crawl_data.csv should contain columns source_url and target_url.

Extract Categories: Define a function extract_category to extract the category or section of the site from the URLs. Modify this function based on the structure of your URLs.

Add Category Columns: Add new columns source_category and target_category to the DataFrame by applying the extract_category function to the source_url and target_url columns.

Group and Count Links: Group the data by source_category and target_category and count the number of links between each category.

Pivot Table: Create a pivot table to show the count of internal links from each source category to each target category.

Save and Display: Save the pivot table to a CSV file and display it for analysis.

This script will help you analyze the internal linking structure of your site, identify sections with the most internal links, and discover opportunities for improving internal linking. Adjust the extract_category function as needed to match your site's URL structure.
