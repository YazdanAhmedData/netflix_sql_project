# 🎬 Netflix SQL Practice | Catalogue Data Exploration

![Netflix project logo](https://github.com/YazdanAhmedData/netflix_sql_project/blob/main/logo.png)

> **Portfolio recommendation:** this project overlaps substantially with [Netflix Content Catalogue Analysis](https://github.com/YazdanAhmedData/netflix_project_sql). For a recruiter-facing portfolio, consider combining the strongest schema, queries, screenshots and verified findings into one canonical Netflix project, and using this repository as a practice/archive project.

## Executive Summary
This repository contains a SQL-based exploration of Netflix movie and TV-show catalogue metadata. It addresses 15 business-style questions involving content type, ratings, release years, countries, genres, cast, directors, duration, missing fields and text-based categorisation.

The dataset describes catalogue metadata; it does **not** show internal viewing counts, watch time, recommendation performance or title profitability.

## Business Problem
The project demonstrates how a data analyst can turn an unstructured list of content metadata into a set of reproducible questions. It focuses on catalogue composition, the distribution of content attributes and data quality.

## Questions & Analytical Areas
- Movies versus TV shows.
- Most common ratings by type.
- Content by release year and country.
- Longest movie and TV shows with more than five seasons.
- Genre distribution and director/actor filtering.
- Indian catalogue entries and documentary titles.
- Missing director values.
- Keyword-based description exploration.

## KPI / Analysis Framework
| Measure | Definition | Business use |
|---|---|---|
| Content type mix | Count by movie / TV show | Catalogue composition |
| Rating distribution | Count by rating and type | Classification overview |
| Country/genre mix | Count titles by parsed value | Catalogue representation |
| Release-year distribution | Count by release year | Historical content profile |
| Additions by date | Count by catalogue-added date | Catalogue additions |
| Missing metadata | Null count/share by field | Data-quality review |
| Runtime / season count | Parsed duration values | Content characteristics |

## Business Insights & Interpretation
- Catalogue counts can describe the collection's composition, but they should not be described as popularity or audience demand.
- Country and genre fields can hold multiple values; normalising these fields changes the unit being counted.
- Release year and catalogue-added date answer different questions and should not be combined.
- Missing director information is a data-quality finding that may affect downstream analysis.
- Keyword-based categories are heuristic and should be labelled as such.

Publish numerical findings only after reproducing the results from the SQL scripts and checking the relevant denominator.

## Repository Files
| File | Purpose |
|---|---|
| `Schemas.sql` | Table/schema setup |
| `Business Problems Netflix.sql` | Business questions |
| `Solutions of 15 business problems.sql` | SQL solutions |
| `netflix_titles.csv` | Source dataset |
| `logo.png` | Project image asset |

## How to Run
1. Create the table by executing `Schemas.sql` in a compatible SQL environment.
2. Load `netflix_titles.csv` and verify data types.
3. Run `Solutions of 15 business problems.sql`.
4. Inspect the output for each query and validate date parsing and multi-value fields.
5. Save selected query results to include a verified findings table.

## SQL Skills Demonstrated
Schema design · Filtering · Aggregation · Window functions · CTEs · String parsing · Null checks · Date filtering · Top-N analysis · Business-question framing

## Quality Checks & Limitations
- Check for duplicate show IDs and missing values.
- Split country and genre values before counting each category.
- Confirm the date format expected by the database engine.
- Do not interpret catalogue metadata as audience engagement or revenue.
- Validate query output before including figures in a portfolio presentation.

## Next Steps
- Add screenshots of representative query outputs.
- Consolidate duplicate analysis with the canonical Netflix repository.
- Add a reproducible setup guide and data dictionary.
- Include three to five verified findings with the exact query behind each one.

## Author
**Yazdan Ahmed** · [GitHub Portfolio](https://github.com/YazdanAhmedData)
