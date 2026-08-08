---
title: "Qdrant 1.19 - TurboQuant Datatype & Memory Tiers"
url: "https://qdrant.tech/blog/qdrant-1.19.x/"
date: "2026-08-05"
author: "info@qdrant.tech (Andrey Vasnetsov)"
feed_url: "https://qdrant.tech/blog/index.xml"
---
Qdrant 1.19.0 is out! Let’s look at the main features for this version: TurboQuant Datatype: A new storage format that compresses vectors to four bits without keeping their original full-precision representation, reducing storage by up to nine times compared to TurboQuant quantization. Memory Tiers: A single memory parameter unifies per-component memory tier placement, with three tiers: pinned , cached , and cold .
