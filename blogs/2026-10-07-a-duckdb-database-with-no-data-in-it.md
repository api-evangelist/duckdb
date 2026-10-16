---
title: "A DuckDB Database with No Data in It"
url: "https://duckdb.org/2026/10/07/view-only-mode.html"
date: "2026-10-07"
author: "The DuckDB team"
feed_url: "https://duckdb.org/feed.xml"
---
A DuckDB database file does not have to contain any data. It can store nothing but view definitions that point at files stored somewhere else, such as Parquet on object storage. The file stays a few hundred kilobytes no matter how large the data it describes, and anyone who attaches it sees a set of named relations that are ready to query.
