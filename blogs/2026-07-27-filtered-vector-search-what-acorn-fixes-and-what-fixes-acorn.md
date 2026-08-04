---
title: "Filtered Vector Search: What ACORN Fixes, and What Fixes ACORN"
url: "https://qdrant.tech/blog/filtered-vector-search-acorn/"
date: "2026-07-27"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
Filtered vector search breaks when metadata filters turn a healthy nearest-neighbor graph into scattered islands. HNSW’s m parameter controls how many links each point gets; at Qdrant’s default m=16 , the collection we benchmark below averaged about 21 links per node on layer 0. Filter out 96% of the points and fewer than one link per node survives on average, so traversal gets stranded before it reaches the true nearest matches.
