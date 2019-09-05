---
description: Font metrics file path. Path and name of a font metrics file, including file suffix.
seo-description: Font metrics file path. Path and name of a font metrics file, including file suffix.
seo-title: MetricsPath
solution: Experience Manager
title: MetricsPath
topic: Scene7 Image Serving - Image Rendering API
uuid: a7b30dfb-0d34-41a6-b215-f653f861987a
index: y
internal: n
snippet: y
---

# MetricsPath{#metricspath}

Font metrics file path. Path and name of a font metrics file, including file suffix.

Used for Adobe Type 1 fonts. If not specified, the server will attempt to find a font metrics file in the same folder in which the principal font file is located. An error will occur if a required font metrics file cannot be found at render time.

## Properties {#section-955268c581574875b05253d9e14544f3}

Text string. Optional for Adobe Type 1 files. Must be empty or a valid Image Server file path, either absolute or relative to `attribute::RootPath`.

## Default {#section-a6ffbd6879c642caa5a2fd4ed14a3a85}

None.

## See also {#section-a3a87a03d8e14876b7dbc2d4ad45c5ef}

[attribute::RootPath](r_rootpath.md#reference_17D57E5967BE403B8408FA7214017494) 