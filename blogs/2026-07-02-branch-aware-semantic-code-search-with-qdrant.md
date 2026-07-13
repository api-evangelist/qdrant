---
title: "Branch-Aware Semantic Code Search with Qdrant"
url: "https://qdrant.tech/blog/branch-aware-code-search/"
date: "2026-07-02"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
Most code search is lexical. You grep a string or jump to a definition, and because it runs on your checkout, it always reflects the branch you have open. Semantic code search goes further: you index the codebase as vectors and search by meaning, which is how you hand an AI agent the right context in one lookup instead of a long grep loop.
