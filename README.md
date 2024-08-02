# Steps
1. Importing the required libraries
2. Scraping from "https://en.wikipedia.org/wiki/List_of_largest_companies_in_the_United_States_by_revenue" for List of largest companies in US by revenue
3. As 3 tables are present and 2nd table is required
    As there are 2 tables with same class_='wikitable_sortable' can't use this method to find the tables so using indexing to find the table
4. Getting all the heading tags of the soup which is having th tag
5. Getting all the heading tags of the table which is having th tag
6. Extracting the th tags
7. Striping the th tags
8. Making a DataFrame out of the th titles extracted
9. Getting all the row data As the row data is having tr tag and then td using this method
10. As an empty row is there on top using indexing to remove that
    column_data[1:] is used
    Then entering the details into the DataFrame already created using df.loc method
11. Saving the scraped data into a CSV file
