---
title: "DuckDB Now Ships inside dbt v2"
url: "https://duckdb.org/2026/09/22/dbt-fusion.html"
date: "2026-09-22"
author: "Geertjan Wielenga"
feed_url: "https://duckdb.org/feed.xml"
---
dbt is the tool many data teams use to manage their SQL transformations: you write each model as a SELECT statement, and dbt works out the order to run them in from the references between models, builds the resulting tables and views in your database, and can test them along the way. dbt-duckdb , the dbt adapter for DuckDB, received its first pull request on August 27, 2021, and in the meantime has 1.4k stars on GitHub . Since then, dbt users have been able to install one Python package (dbt-duckdb, via pip ), point it at a file (a local DuckDB database), and have a working project (models bui
