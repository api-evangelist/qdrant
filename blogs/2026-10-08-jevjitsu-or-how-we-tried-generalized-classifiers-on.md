---
title: "Jevjitsu: Or, How We Tried Generalized Classifiers on Everything"
url: "https://qdrant.tech/blog/jevjitsu/"
date: "2026-10-08"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
Classification is one of the oldest problems in machine learning. Unlike modern decoding transformers, most classification models were non-autoregressive by nature. Before Jev, the common approaches were training your own classifier, which needs labels, using a zero-shot classifier (compared in this Hugging Face benchmark ), or prompting an LLM with some hacky type safety on top.
