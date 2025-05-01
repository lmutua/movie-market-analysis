# Movie Market Analysis Project
# Overview

This project analyzes historical movie industry data to uncover drivers of box office success and return on investment (ROI) for SilverScreen Studios' market entry strategy. The analysis combines exploratory visualizations with statistical techniques to identify high-performing genres, optimal release periods, and financially viable production strategies.

## Business Problem  
Entering the movie production industry involves substantial financial investment and uncertainty. SilverScreen Studios requires a data-driven approach to reduce risks and optimize decision-making. Understanding the influence of factors such as directors, studios, genres, and release months on financial performance is essential to formulating a successful market entry strategy. This analysis seeks to determine what types of movies and release strategies yield the highest return on investment (ROI), and which market players and genres consistently lead in revenue generation.

# Objectives

    1. Identify top-performing directors and genres, and evaluate their impact on the movie market.  
    2. Analyze the most successful studios and the revenue they generate.  
    3. Determine which types of movies generate the highest ROI using budget and gross revenue data.  
    4. Investigate whether the release month significantly affects movie revenue. 

# Project Structure

movie-market-analysis/
├── zippedData   # Raw data files(bom.movie_gross.csv,im.db.zip,rt.movie_info.tsv.gz,rt.reviews.tsv.gz,tmdb.movies.csv.gz,tn.movie_budgets.csv.gz)
├── Movie_market_analysis_notebook.ipynb 
├── README.md     
└── images       
└── release_mon_analysis.ipynb       

# Data Sources
The datasets used in this analysis are compiled from reputable online movie databases and stored in the zippedData folder. They cover various dimensions of the movie industry such as:

    1. Box Office Mojo (box office gross performance)

    2. Rotten Tomatoes (movie metadata and reviews)

    3. The Movie Database (TMDB) (extensive movie metadata)

    4. The Numbers (production budgets and worldwide gross)

    5. IMDB database (movie basics, directors, ratings)
    
# Key Findings
The analysis uses a Heatmap to display the top 10 directors. This heatmap visualizes the distribution of genres for the top 10 directors based on the number of movies they’ve directed. The plot shows the number of movies each of the top directors has directed in each genre.

    1. X-axis: Genres
    2. Y-axis: Top 10 Directors
    3. Color intensity: Represents the number of movies directed by each director in each genre.
    4. Annotations: The number of movies is displayed within each cell, with values formatted to two decimal places.

It also provides insights into the genres that top directors prefer or tend to direct more frequently, helping to identify genre trends across different directors.
This is represented as below:

    1. The more intense the color, the greater the number of movies a director has made in that genre.
    2. The plot helps in identifying any directors with a specialization in particular genres, or if a director has ventured across multiple genres.

# Statistical Approaches
Three statistical approaches were used in this analysis to assess whether the release month has a significant effect on worldwide box office revenue:

    1. One-way ANOVA test # To determine whether there are statistically significant in mean worldwide gross revenue across the twelve release months
    
    2. Independent t-test # To compare the average worldwide gross revenue between movies released in May and November because the 2 months are strategically important in the film industry calendar
    
    3. Linear regression modeling # To explore the relationship between a movie’s production budget and its box office performance, a linear regression model was used

# Recommendations

From the analysis done it is seen that having top directors to work on a film makes the movie more popular. Good directors would make popular movies hence the company would generate more by investing in good directors.

# Conclusion:
The findings were that there is a general positive correlation between domestic and foreign gross. This means that movies that perform well domestically tend to also perform well in foreign markets, and vice versa. The correlation appears to be relatively strong, as the points are clustered around the line of best fit, suggesting a clear relationship between the two variables.

A limitation to this is that while most movies follow the general trend, there are some outliers. Some movies have high domestic gross but relatively low foreign gross, while others have high foreign gross but lower domestic gross

# How to Run the Analysis

    1. Clone this repository
   
    2. Extract zippedData directory to get datasets

    4. Open and run the Jupyter notebook:

       jupyter notebook Movie_market_analysis_notebook.ipynb

# Dependencies

    1. Pandas

    2. Numpy

    3. Matplotlib

    4. Seaborn

    5. Scipy

    6. Statsmodels

    7. Sqlite3


# Contributors

    1. Kelvin Kipkorir

    2. Raphael Muthenya    

    3. Lucy Mutua

    4. Charles Mutembei

    5. Andrew Chege

    6. Sharon Aoko
