---
title: "Persistent Databases in the Browser with DuckDB-Wasm and OPFS"
url: "https://duckdb.org/2026/09/18/opfs-wasm.html"
date: "2026-09-18"
author: "Carlo Piovesan, Geertjan Wielenga"
feed_url: "https://duckdb.org/feed.xml"
---
When DuckDB-Wasm was launched in 2021, databases could not be persisted: everything lived in the Wasm heap and vanished when the tab closed. Keeping data meant serializing tables to Parquet, storing the bytes in IndexedDB, and re-registering them on the next page load. This was doable, but had to be handled at the application layer and was not offered out of the box by DuckDB-Wasm.
