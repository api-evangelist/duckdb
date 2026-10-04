---
title: "Faster String Aggregations with Dimension Tables"
url: "https://duckdb.org/2026/10/02/dimension-tables.html"
date: "2026-10-02"
author: "DuckDB Team"
feed_url: "https://duckdb.org/feed.xml"
---
Analytical workloads are full of repeated strings: product names, country names, station names, user agents, category labels. Take DuckDB's public train services dataset, which has one row for every stop a Dutch railway train makes. The data comes from the open datasets published by the Rijden de Treinen (Are the trains running?) application .
