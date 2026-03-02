**Exploring London’s Public Transport Usage with Snowflake SQL**

London is one of the world’s busiest and most diverse metropolitan regions, home to millions of residents and commuters who rely on an extensive public transportation network. To understand how Londoners travel across the city, this project analyzes long-term journey data from Transport for London (TfL) using Snowflake SQL as the core analytics engine.
This project breaks down how Londoners use different transport services over time, with Snowflake SQL powering all queries. By analyzing total usage, popularity trends, and yearly fluctuations, the project provides clear insights into the city’s transportation dynamics, from buses and trams to the iconic Underground and Emirates Airline cable car.
The dataset, stored in a Snowflake database (TFL.JOURNEYS), contains monthly journey volumes across multiple transport modes and provides a clear look into usage patterns, peak periods, and long-term ridership changes.

**Key Questions Answered**

1️. Which transport modes have the highest total journey volumes?

A full aggregation reveals London’s most frequently used services.

Output:
most_popular_transport_types.csv

2️. When was the Emirates Airline cable car most popular?

By ranking monthly ridership for this unique transport service, we identify its top-performing months.

Output:
emirates_airline_popularity.csv

3️. Which years recorded the lowest Underground & DLR usage?

Yearly totals help uncover dips in the network — whether influenced by major events, disruptions, or long-term trends.

Output:
least_popular_years_tube.csv

**Dataset**

The repository includes a local export of the Snowflake table:

tfl_journeys_final.csv

Columns include:

MONTH – Month number (1–12)

YEAR – Calendar year

DAYS – Number of days in the month

REPORT_DATE – Reported date

JOURNEY_TYPE – Mode of transport

JOURNEYS_MILLIONS – Monthly journeys (in millions)

**Files Included**

**Main Files**

tfl_analysis.ipynb — Notebook containing the Snowflake SQL analysis

SQL_Queries.sql — All Snowflake SQL queries used in the project

README.md — Project overview

**Dataset**

tfl_journeys_final.csv — Clean TfL journey data

**Generated Outputs**

most_popular_transport_types.csv

emirates_airline_popularity.csv

least_popular_years_tube.csv




