# Country-GDP Data ETL Project

## Overview
This is a Coursera (IBM) Course project, which is an ETL (Extract, Transform, Load) pipeline focused on gathering and processing GDP data for various countries. The data is extracted from a Wikipedia page listing countries by nominal GDP in USD. The pipeline then transforms this data, converting GDP values from millions to billions, and finally loads the processed data into both a CSV file and a SQLite database.


## Features
- **Extract**: Utilizes Python libraries such as `requests` and `BeautifulSoup` to gather relevant information from the [List of countries by GDP (nominal)](https://web.archive.org/web/20230902185326/https://en.wikipedia.org/wiki/List_of_countries_by_GDP_%28nominal%29) Wikipedia page.
- **Transform**: Converts GDP values from millions to billions, refining the dataframe structure for better usability.
- **Load to CSV**: Saves the final dataframe as a CSV file at the specified path (`./Countries_by_GDP.csv`).
- **Load to Database**: Establishes a connection to the SQLite database (`World_Economies.db`) and loads the transformed data into the `Countries_by_GDP` table.
- **Run Query**: Executes a query on the database table, filtering countries with GDP over 100 billion USD.
- **Logging**: Captures key stages of the ETL process, including timestamps and messages, in the `etl_project_log.txt` log file.


## File Structure
- **etl_project_gdp.py**: Main script for the ETL process.
- **Countries_by_GDP.csv**: Final processed data saved as a CSV file.
- **World_Economies.db**: SQLite database file for structured data storage.
- **etl_project_log.txt**: Log file for recording the execution progress.


## Dependencies
- **pandas**: For data manipulation and storage.
- **numpy**: For numerical operations.
- **requests**: For making HTTP requests.
- **beautifulsoup4**: For web scraping.
- **sqlite3**: For database operations.


## Contribution
Contributions are welcome! Feel free to submit bug reports, feature requests, or pull requests. Your feedback and collaboration are highly appreciated!



