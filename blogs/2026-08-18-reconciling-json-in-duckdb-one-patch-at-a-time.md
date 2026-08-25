---
title: "Reconciling JSON in DuckDB, One Patch at a Time"
url: "https://duckdb.org/2026/08/18/reconciling-json.html"
date: "2026-08-18"
author: "{\"picture\" => \"/images/blog/authors/mustafa_khan_atlan.jpg\"}"
feed_url: "https://duckdb.org/feed.xml"
---
Guest blog post by Mustafa Khan ( Atlan ). DuckDB's JSON extension already covers reading JSON, extracting paths, applying RFC 7396 merge patches, and the usual scalar accessors. The upcoming v2.0 release will extend it with four new scalar functions: json_merge_patch_diff computes the inverse of an RFC 7396 merge patch, json_deep_merge applies patches with skip-on- null semantics, json_normalize canonicalizes key order, and json_strip_nulls recursively removes null -valued keys.
