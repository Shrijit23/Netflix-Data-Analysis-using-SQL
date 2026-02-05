# Netflix-Data-Analysis-using-SQL

<img width="2226" height="678" alt="logo" src="https://github.com/user-attachments/assets/7c88b479-22bc-4a15-90df-22b81da7fcbd" />

This project analyzes Netflix Movies and TV Shows data using SQL to extract meaningful business insights. It involves database design, data import, and writing optimized SQL queries to explore content trends, genres, countries, ratings, and release patterns, demonstrating real-world data analysis skills.

Project Overview

This project performs a detailed SQL-based analysis of Netflix’s Movies and TV Shows dataset to uncover meaningful patterns and answer practical business-driven questions. The aim is to explore Netflix’s content library from multiple angles such as content type, ratings, countries, genres, duration, release trends, and keyword-based categorization.

The analysis demonstrates how structured query language can be used to transform raw data into actionable insights that support decision-making in content strategy and platform growth.

Project Objectives

Compare the distribution of Movies and TV Shows on Netflix
Determine the most frequently used ratings across content types
Analyze content by release year, country, and duration
Identify trends related to directors, actors, and genres
Categorize content based on keywords found in descriptions

Dataset Details

Source: Kaggle – Netflix Movies and TV Shows Dataset
Format: CSV
Records: 8,000+ entries
Description: Includes metadata such as title, type, director, cast, country, rating, duration, genre, and description

Database Schema

The dataset is stored in a single relational table named netflix:

DROP TABLE IF EXISTS netflix;
CREATE TABLE netflix (
    show_id VARCHAR(5),
    type VARCHAR(10),
    title VARCHAR(250),
    director VARCHAR(550),
    casts VARCHAR(1050),
    country VARCHAR(550),
    date_added VARCHAR(55),
    release_year INT,
    rating VARCHAR(15),
    duration VARCHAR(15),
    listed_in VARCHAR(250),
    description VARCHAR(550)
);

Business Questions Addressed:

1.The project answers several real-world analytical questions, including:
2.Distribution of Movies versus TV Shows
3.Most common ratings for each content type
4.Movies released in a specific year
5.Top countries contributing the highest number of titles
6.Longest movie available on Netflix
7.Content added within the last five years
8.Titles directed by a specific director
9.TV shows with more than five seasons
10.Genre-wise content distribution
11.Year-wise average content release in India (Top 5 years)
12.Movies classified as documentaries
13.Content entries missing director information
14.Movies featuring a specific actor in the last decade
15.Top actors in Indian-produced movies
Content classification based on keywords such as kill and violence
Each query is written using SQL features like CTEs, window functions, string manipulation, filtering, aggregation, and date functions.

Key Findings & Insights

Netflix hosts a wide variety of content across genres, regions, and formats
Movies make up a larger portion of the catalog compared to TV shows
Certain ratings dominate specific content types, indicating target audience preferences
India shows notable year-wise growth in content releases
Keyword-based classification helps identify the nature and tone of available content

Conclusion

This project provides a comprehensive view of Netflix’s content ecosystem using SQL. The insights derived from this analysis can help understand audience targeting, regional growth, and content trends. It also highlights the effectiveness of SQL as a core tool for data analysis and business intelligence.


