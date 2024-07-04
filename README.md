# Netflix Content Analysis

## Overview

This project analyzes the Netflix Titles dataset to uncover insights into the content available on Netflix. The dataset includes various attributes such as title type, director, cast, country of production, release year, rating, duration, genres, and a brief description. 

## Dataset

The Netflix Titles dataset is a comprehensive compilation of movies and TV shows available on Netflix. The dataset contains 8809 entries and 12 columns:
- `show_id`: A unique identifier for each title.
- `type`: The category of the title (Movie or TV Show).
- `title`: The name of the movie or TV show.
- `director`: The director(s) of the movie or TV show.
- `cast`: The list of main actors/actresses in the title.
- `country`: The country or countries where the movie or TV show was produced.
- `date_added`: The date the title was added to Netflix.
- `release_year`: The year the movie or TV show was originally released.
- `rating`: The age rating of the title.
- `duration`: The duration of the title in minutes for movies and seasons for TV shows.
- `listed_in`: The genres the title falls under.
- `description`: A brief summary of the title.

## Use Case - Content Analysis

- **Trend Analysis**: Analyzing the number of movies and TV shows added over the years and their release dates.
- **Duration Analysis**: Finding trends in the duration of movies.
- **Content Ratings**: Analyzing the different content ratings.
- **Geographical Distribution**: Visualizing the geographical distribution of content.
- **Genre Popularity**: Analyzing genre popularity over time.

## Data Cleaning and Processing

1. **Importing Data**: The Netflix_titles.csv file was imported from Kaggle.com.
2. **Removing Empty Columns**: Extra empty columns were removed using Power Query Editor.
3. **Adding Columns**: Added columns for `Year_added` and `Month_added` to capture when content was added to Netflix.
4. **Handling Missing Values**: Checked for missing values and sorted the percentile of missing values using conditional formatting.
5. **Extracting Duration**: Created additional columns `duration_movies` and `duration_tv` by extracting values from the `duration` column.

## Data Visualization - Pivot Tables

- **Content Distribution**: A pie chart showing that 70% of content on Netflix is movies and the rest are TV shows.
- **Directors with Most Content**: A bar chart showing Rajiv Chailaka as the director with the most content.
- **Yearly and Monthly Distribution**: Line and stacked column charts showing content added during 2019-2021 and monthly trends.
- **Release Year**: A bar chart showing that most content is new.
- **Rating Analysis**: A bar chart showing that the majority of the content is TV-MA.

## Duration Analysis

- **Movies Duration**: A histogram showing that 48% of the movies are 90-120 minutes long.
- **TV Shows Seasons**: A histogram showing that 67% of the shows have only 1 season.

## Geographical Analysis

- **Country Analysis**: Converted the `country` column using text to columns with a delimiter comma to take all countries into consideration. Created geographical maps and bar charts showing most production in the USA and India.

## Genre Analysis

- **Genres Distribution**: Converted the `listed_in` column using text to columns with a delimiter comma to analyze all genres separately. Created bar charts showing that 31% of the content falls under the genre International Movies.

## Dashboards

### Overview Dashboard
Charts included:
- Content distribution
- Monthly content added
- Yearly content added
- Release date
- Rating analysis
- Duration analysis for movies
- Directors with most content

Slicers: type, year, month, release_year, rating

### Geographical Dashboard
Charts included:
- Geographical analysis map
- Top countries

Slicers: type, year, release_year, country

### Genre Dashboard
Charts included:
- Genre by count

Timeline included for years, quarters, months, and days

Slicers: type, title

## Acknowledgements

This project uses the Netflix Titles dataset from Kaggle. The data was used to explore and visualize trends, duration, ratings, geographical distribution, and genre popularity of Netflix content.

## Getting Started

1. **Clone the repository**: 
   ```sh
   git clone https://github.com/yourusername/Netflix_Content_Analysis.git
