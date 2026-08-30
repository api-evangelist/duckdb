---
title: "How DuckDB Runs Recursive CTEs Faster"
url: "https://duckdb.org/2026/08/25/how-duckdb-runs-recursive-ctes-faster.html"
date: "2026-08-25"
author: "Denis Hirn"
feed_url: "https://duckdb.org/feed.xml"
---
When I implemented DuckDB's first recursive CTE operator in 2020, correctness determined the design: evaluate the non-recursive term once, then evaluate the recursive term until the next working table is empty. That established the right semantic contract, but reusable runtime state was scoped too narrowly. Across iterations, the recursive input changes while most of the machinery that evaluates it remains reusable.
