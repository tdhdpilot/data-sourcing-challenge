# data-sourcing-challenge

## Module 6 Challenge

### Instructions

This Challenge has three parts, and must be completed in order:

- Part 1: Access the New York Times API.

- Part 2: Access The Movie Database API.

- Part 3: Merge and Clean the Data for Export.

#### Part 1

The New York Times API is accessed to retrieve movie reviews meeting specific criteria.

- A query URL is constructed based on the API documentation.
- A loop is created to iterate through multiple pages of results.
- Results are retrieved using GET requests, and a 12-second interval is implemented between queries.
- A try-except clause handles errors and retrieves reviews from the response.
- The extracted data is previewed and converted into a Pandas DataFrame.
- Titles and keywords are extracted from the DataFrame.

#### Part 2

The TMDB API is accessed to retrieve additional details about the movies mentioned in the New York Times reviews.

- Titles extracted from Part 1 are used to search for corresponding movies in TMDB.
- Details about the movies, such as genres, languages, and production countries, are extracted and stored.
- Data retrieval is handled in a try-except block to manage errors and ensure robustness.
- Results are previewed and converted into a DataFrame for further analysis

#### Part 3

The data retrieved from both APIs are merged and cleaned before export.

- Data from both APIs are merged on the movie titles column.
- Columns containing lists are cleaned by removing brackets and quotation marks.
- Duplicate rows are removed, and the index is reset.
- The final DataFrame is exported to a CSV file without the index.

### Sources

- Class Lessons
- Instructor
- Teacher Assistant
- Classmates
- Xpert Learning Assistant
- Co-Pilot
- Tutor
- NYT API - https://developer.nytimes.com/docs/articlesearch-product/1/overview
- TMDB Movie API - https://developer.themoviedb.org/docs/search-and-query-for-details
