---
title: "From JSON Strings to Typed Columns"
url: "https://duckdb.org/2026/10/16/json-to-typed-columns.html"
date: "2026-10-16"
author: "The DuckDB team"
feed_url: "https://duckdb.org/feed.xml"
---
DuckDB's read_json turns JSON files into tables. It reads through part of the data to work out a schema, then gives you typed columns. However, a lot of JSON does not come as files.
