---
title: "Oxidizing Cross-Encoders"
url: "https://qdrant.tech/blog/oxidizing-cross-encoders/"
date: "2026-09-25"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
We rewrote cross-encoder inference in Rust, benchmarked it against Python, and on a small reranking model it came out only 1.1x faster at the median. That is not a sign of a slow Rust implementation. The Python libraries we compared against, fastembed and sentence-transformers , hand the same work to the same C++ engine, onnxruntime , so all three spend almost all of their time in the same compiled code.
