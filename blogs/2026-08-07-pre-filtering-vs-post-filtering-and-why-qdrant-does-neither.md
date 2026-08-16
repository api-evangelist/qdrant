---
title: "Pre-Filtering vs Post-Filtering (and Why Qdrant Does Neither)"
url: "https://qdrant.tech/blog/pre-filtering-vs-post-filtering/"
date: "2026-08-07"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
Adding a metadata filter to vector search can make good results disappear without making the query look broken. It still runs fast, returns something, and keeps the dashboards quiet, while some of the true nearest matches drop out. In the benchmark behind this post, a broad-value filter lowers recall to 90.8% and an AND filter over two broad values lowers it to 39.7%, while every other filter shape stays above 97%.
