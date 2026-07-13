---
title: "Qdrant Beats Elastic’s DiskBBQ at 2x Throughput, Half the Latency, and 1/3 the Compute"
url: "https://qdrant.tech/blog/benchmark-elastic-diskbbq/"
date: "2026-07-08"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
TL;DR Elastic recently published a benchmark claiming that their proprietary, disk-based index (dubbed “DiskBBQ”) delivers up to 7x higher throughput than Qdrant when deployed on nodes with network-attached storage. Elastic set out to benchmark DiskBBQ against a Qdrant cluster configured for disk-based retrieval, but their methodology omitted the exact features Qdrant built for this workload. Instead of enabling our documented two-stage retrieval and async disk scoring, they effectively ran a stress test on unbounded sequential disk access and reported the resulting I/O bottleneck as a baselin
