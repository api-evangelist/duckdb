---
title: "Asynchronous I/O in DuckDB: Work, Thread, Work"
url: "https://duckdb.org/2026/07/31/asynchronous-io.html"
date: "2026-07-31"
author: "{\"twitter\" => \"holanda_pe\", \"picture\" => \"/images/blog/authors/pedro_holanda.jpg\"}"
feed_url: "https://duckdb.org/feed.xml"
---
It doesn't matter how fast query operators are in a database system if we can't pull in the data quickly. For most of DuckDB's history, however, this problem was largely avoided by pruning data early. By pushing down filters and projections, we could ensure that we only read what we actually needed.
