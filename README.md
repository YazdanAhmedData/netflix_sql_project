# Netflix SQL Practice Project | Catalogue Data Exploration

This repository contains a SQL-based exploration of Netflix movie and TV-show catalogue metadata. It addresses common SQL practice questions involving content types, ratings, release years, countries, genres, cast, directors, and text-based categorization.

> **Portfolio note:** This repository overlaps substantially with [Netflix Content Analysis](https://github.com/YazdanAhmedData/netflix_project_sql). For a recruiter-facing portfolio, consider maintaining one canonical Netflix project with the strongest queries, documentation, and validated findings rather than presenting two near-identical projects as separate case studies.

## Objective
Practise SQL by answering structured questions from netflix_titles.csv and translating the outputs into understandable observations about the catalogue. This dataset describes catalogue metadata, not Netflix's internal viewing behaviour, revenue, or recommendation algorithms.

## Dataset
- netflix_titles.csv — movie and TV-show metadata
- Common fields include type, title, director, cast, country, date added, release year, rating, duration, and listed genres.

Inspect the schema and data types before running queries. Multi-value fields and missing values can affect counts.

## Questions Covered
- Movie versus TV-show counts
- Rating distributions
- Content by release year and country
- Longest movie and TV shows with many seasons
- Genre distributions
- Director and actor filtering
- Missing director values
- Keyword-based title/description categorization

## Files
| File | Purpose |
|---|---|
| Schemas.sql | Schema setup |
| Business Problems Netflix.sql | Business questions |
| Solutions of 15 business problems.sql | Query solutions |
| netflix_titles.csv | Dataset |
| logo.png | Project image asset |

## How to Run
1. Clone or download this repository.
2. Create the table using Schemas.sql in a compatible SQL environment.
3. Load the CSV using the import method supported by your database.
4. Run the statements in Solutions of 15 business problems.sql.
5. Review the query assumptions, especially date formats, delimited country/genre fields, and null values.

Database-specific syntax may require adjustment depending on the SQL engine.

## Interpretation Limits
- Catalogue metadata does not show actual audience views or profitability.
- Multi-country and multi-genre titles can be counted differently depending on query logic.
- Keyword searches are heuristic and should not be treated as a reliable content-classification model.
- Report only numerical findings that have been reproduced by running the SQL.

## Skills Demonstrated
SQL schema design · Querying · Aggregation · Filtering · Data exploration · Text handling · Data-quality checks

## Author
**Yazdan Ahmed**  
[GitHub Portfolio](https://github.com/YazdanAhmedData)
