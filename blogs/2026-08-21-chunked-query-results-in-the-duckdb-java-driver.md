---
title: "Chunked Query Results in the DuckDB Java Driver"
url: "https://duckdb.org/2026/08/21/chunked-query-results-java-driver.html"
date: "2026-08-21"
author: "Geertjan Wielenga, Alex Kasko"
feed_url: "https://duckdb.org/feed.xml"
---
DuckDB is a columnar, vectorized database. Every operator inside the engine works on data chunks: batches of column vectors, 2,048 rows at a time. That is a big part of why DuckDB is fast: the engine amortizes interpretation overhead over thousands of values instead of paying it once per value.
