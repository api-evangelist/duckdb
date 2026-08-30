---
title: "DuckDB Table Functions in Java"
url: "https://duckdb.org/2026/08/25/table-functions-in-java.html"
date: "2026-08-25"
author: "Geertjan Wielenga, Alex Kasko"
feed_url: "https://duckdb.org/feed.xml"
---
In a large organization, data is spread across many systems, including relational databases, document stores, message queues, data lakes, and cloud data warehouses. Some of these systems can be reached only through a vendor SDK, usually provided in Java, or a SOAP endpoint, and many sit behind custom authentication or single sign-on that is awkward to satisfy from anything but a JVM client. The layer that ties these together is often a JVM-based distributed query engine, such as Trino , that can run a single query joining across multiple data sources.
