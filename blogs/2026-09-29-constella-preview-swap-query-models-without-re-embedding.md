---
title: "Constella Preview: Swap Query Models Without Re-Embedding"
url: "https://qdrant.tech/blog/constella-research-preview/"
date: "2026-09-29"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
As query traffic grows, so does the compute bill for embedding it. On a low-power device, a large model may not fit in memory. A smaller query model could reduce that cost, but switching usually means re-embedding the collection.
