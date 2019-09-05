---
description: Some restrictions apply for nesting and embedding.
seo-description: Some restrictions apply for nesting and embedding.
seo-title: Restrictions
solution: Experience Manager
title: Restrictions
topic: Scene7 Image Serving - Image Rendering API
uuid: a0662205-b3fe-45f1-a1f5-480defdf28eb
index: y
internal: n
snippet: y
---

# Restrictions{#restrictions}

Some restrictions apply for nesting and embedding.

For good server performance, the resolution of images returned by nested requests should reasonably match the texture resolution of the object(s) to which the material is being applied.

Foreign images are cached locally. Any changes to such images will be detected only after the local cache entry becomes stale (based on the expires HTTP header). 