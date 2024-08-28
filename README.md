# Fluctuations of Ticket Prices

## Introduction
Methods used to extract and clean data from a travel website to analyze trends and price fluctuations before flight departures. The analysis aims to:
- Assess price fluctuations at time intervals leading up to  departure.
- Explore correlations between flight time windows, day of the week, fare class, ticket availability, and price fluctuations.
- Analyze the impact of the number of airlines operating the route vs ticket prices.
- Compare fare classes and flight windows.

## Installing Libraries
Libraries used for the project include:
- Selenium
- BeautifulSoup
- Pandas

## Bot Detection
To avoid the websites bot detection, URL manipulation and the `sleep()` function with random intervals were employed.

## Web Scraping Methods

### Selenium
Selenium WebDriver was used to navigate Webjet pages. Initial issues with Selenium were resolved by passing the Chrome driver path as a variable.

### BeautifulSoup
After navigating to the desired URL, the page's HTML was extracted and parsed using BeautifulSoup.

### Global Variables
Global variables were used to enhance code accessibility.

### For Loops
For loops were utilised to iterate through BeautifulSoup objects and extract the necessary elements.

## Creating DataFrames with Pandas
A custom function was created to:
- Generate data frames from lists stored in variables.
- Combine data frames using `pd.concat()`.
- Rename and reshape columns with `.rename()`.
- Convert string times to datetime with `pd.to_datetime()`.
- Clean and format data, replacing airline jargon with clear language and adjusting data types using `.astype()`.

## Cleaning Data
The data was cleaned by removing special characters, replacing jargon, and converting data to appropriate types.

## Quality Checks
Quality checks were conducted throughout the code. The final data frame was dynamically tested for:
- Null values using `isnull().any()`.
- Duplicate values using `.duplicated().any()`.
- NaN values using `isna().any()`.

## Preliminary Aggregation and Analysis
Initial analysis focused on identifying price trends and potential correlations in the data.

## Next Steps
- Expand the sample size to further analyze price fluctuations over time.
- Investigate correlations between various factors and ticket prices.
- Enhance statistical analysis and visualization to present insights.

## References


<p align="center">
Step 1: Brief Description <br/>
<img src="yourimageurl1" height="80%" width="80%" alt="Step 1"/>
<br />
<br />
Step 2: Brief Description <br/>
<img src="yourimageurl2" height="80%" width="80%" alt="Step 2"/>
<br />
<br />
Step 3: Brief Description <br/>
<img src="yourimageurl3" height="80%" width="80%" alt="Step 3"/>
</p>

<h2>Usage</h2>
Provide examples of how to run the project, including command-line instructions or steps to follow in a user interface.

<h2>Future Enhancements</h2>
- <b>Enhancement 1:</b> Planned or potential improvements.
- <b>Enhancement 2:</b> Any additional features you might add later.
