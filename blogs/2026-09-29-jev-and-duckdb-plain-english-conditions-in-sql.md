---
title: "Jev and DuckDB: Plain-English Conditions in SQL"
url: "https://duckdb.org/2026/09/29/jev.html"
date: "2026-09-29"
author: "Geertjan Wielenga, Gábor Szárnyas"
feed_url: "https://duckdb.org/feed.xml"
---
Say you have a Parquet file of 50,000 support tickets and want to know which customers are angry. A LIKE pattern won't find that. The usual options are to label data and train a classifier, or to send each row to a chat LLM and parse the text it returns.
