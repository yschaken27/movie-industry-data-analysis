# Movie Industry Data Analysis

## Project Overview

This project investigates how psychological characteristics of movie reviews and Oscar recognition are associated with international box office performance.

Using data from Metacritic, The Numbers and an Oscar awards dataset, the project combines data engineering, relational database design and statistical analysis to explore patterns in the international movie industry.

## Research Question

**How are movie review characteristics and awards associated with international box office performance?**

The analysis addresses three sub-questions:

1. Which psychological characteristics of reviews relate to international box office performance?
2. How are movie review characteristics associated with Oscar nominations?
3. To what extent is Oscar recognition associated with international box office performance?

## Technologies Used

- **Python:** Data cleaning, transformation and statistical analysis
- **pandas:** Data manipulation and integration
- **SQL:** Querying and joining relational datasets
- **PostgreSQL:** Relational database management
- **Neon:** Cloud-hosted PostgreSQL database
- **Statistical methods:** Pearson and Spearman correlations, logistic regression and hypothesis testing
- **Database design:** Entity Relationship Diagrams (ERD), primary keys, foreign keys and normalization

## Data Engineering Workflow

The project follows an Extract, Transform and Load (ETL) workflow:

1. **Extract:** Import movie metadata, expert reviews, consumer reviews, box office data and Oscar records.
2. **Transform:** Clean review data, standardize movie titles, match films across sources and create a shared movie identifier.
3. **Load:** Store the prepared tables in a PostgreSQL database hosted on Neon.
4. **Query:** Combine related tables using SQL.
5. **Analyse:** Retrieve analysis-ready dataframes through Python encapsulators and evaluate the research hypotheses.

## Database Architecture

A central `movie_master` table connects the datasets through a shared `movie_id`.

The relational schema includes movie metadata, sales, box office revenue, expert reviews, consumer reviews, sentiment variables, genres, cast and Oscar nominations.

Bridge tables support many-to-many relationships, while normalization reduces unnecessary duplication and improves data consistency.

## Key Findings

- **Review sentiment:** Positive emotional language showed a weak positive association with international box office revenue for both expert and consumer reviews.
- **Oscar nominations:** More positive and fewer negative review characteristics were associated with a higher likelihood of Oscar nomination, although the explanatory power of these models was limited.
- **International box office:** Oscar-nominated films earned substantially higher average international revenue than non-nominated films in the analysed sample.
- **Business implications:** Review sentiment and award recognition can provide useful signals for international marketing and forecasting, but should be combined with other variables.

## Limitations

The findings indicate associations rather than proven causal effects. Review characteristics and awards explain only part of the variation in movie performance. Other factors, including production budget, marketing expenditure, genre and release timing, should be considered in future models.

## Skills Demonstrated

Data cleaning · Data integration · ETL · Relational database design · SQL querying · Python data analysis · Statistical testing · Business insight generation

## Project Context

Academic project completed for the Database Management course within the MSc Digital Driven Business programme at Amsterdam University of Applied Sciences.

