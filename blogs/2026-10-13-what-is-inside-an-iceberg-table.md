---
title: "What Is Inside an Iceberg Table?"
url: "https://duckdb.org/2026/10/13/inside-iceberg-table.html"
date: "2026-10-13"
author: "The DuckDB team"
feed_url: "https://duckdb.org/feed.xml"
---
An Apache Iceberg table looks like a regular table when you query it, but underneath it is a small tree of files: one JSON file at the top, a few layers of Avro files in the middle, and Parquet files at the bottom. When something is slow or looks wrong, it helps to know what is in that tree. DuckDB can read all three formats, so you can inspect every layer with plain SQL.
