---
title: "DuckDB and Hugging Face: Querying Datasets Directly"
url: "https://duckdb.org/2026/09/25/hugging-face.html"
date: "2026-09-25"
author: "The DuckDB team"
feed_url: "https://duckdb.org/feed.xml"
---
Hugging Face is where much of the machine learning community publishes and finds its datasets, while DuckDB is the in-process analytical database that queries files like CSV and Parquet directly, with no server or warehouse to install or run. Did you know that, since DuckDB v0.10.3 (released on May 22, 2024), you can point a SELECT at a dataset on the Hugging Face Hub , using the DuckDB hf:// protocol, and query it, without downloading it first? This post covers how that integration works and the use cases it fits.
