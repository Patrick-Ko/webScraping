# webScraping

## Project Overview

This project demonstrates skills in web scraping, data extraction, and data storage. The primary objective is to scrape venue information from a specified webpage (https://sts.ug.edu.gh/timetable), structure the data, and store it in a DataFrame. The project also includes scraping multiple pages over a date range and saving the unique venue information to an Excel file.

## Table of Contents

1. [Project Setup](#project-setup)
2. [Scraping a Single Page](#scraping-a-single-page)
3. [Scraping Multiple Pages](#scraping-multiple-pages)
4. [Storing Data in a DataFrame](#storing-data-in-a-dataframe)
5. [Saving Data to Excel](#saving-data-to-excel)
6. [Conclusion](#conclusion)

## Project Setup

In this section, the necessary libraries required for web scraping, date handling, and data manipulation are imported. The libraries include `requests` for making HTTP requests, `BeautifulSoup` from `bs4` for parsing HTML content, `datetime` and `timedelta` for handling date ranges, and `pandas` for data manipulation and storage.

## Scraping a Single Page

This section involves defining a function `scrape_page` that takes a URL as input, fetches the webpage content, and parses the HTML to extract specific information. The function looks for all span elements with the class `text-warning` and extracts their text content. The function is then used to scrape a single page and print the extracted venue information.

## Scraping Multiple Pages

Here, a function `generate_dates` is defined to generate a range of dates between a specified start and end date. This function is then used to scrape multiple pages over the generated date range. For each date, the date is formatted into a URL, the page is scraped, and the venue information is extracted. The extracted information is cleaned and stored in a set to ensure uniqueness.

## Storing Data in a DataFrame

In this section, the unique venue information stored in a set is converted into a sorted list. A Pandas DataFrame is then created from this list, with a single column named "Venue". This DataFrame is used to store and manipulate the extracted data.

## Saving Data to Excel

Finally, the DataFrame containing the unique venue information is saved to an Excel file named `uniqueVenues.xlsx`. This allows for easy sharing and analysis of the extracted data using spreadsheet software.

## Conclusion

This project demonstrates the ability to:
- Scrape data from the web using `requests` and `BeautifulSoup`.
- Handle date ranges and generate URLs dynamically.
- Extract and clean data.
- Store data in a Pandas DataFrame.
- Save data to an Excel file.

Feel free to explore the code and use it as a reference for web scraping projects. For any questions or suggestions, please contact me at [komladogbatse28@gmai.com](mailto:komladogbatse28@gmai.com).

---

Thank you for visiting this repository!