---
description: Illumination map selector. Specifies the illumination map this material prefers to be rendered with.
seo-description: Illumination map selector. Specifies the illumination map this material prefers to be rendered with.
seo-title: illum
solution: Experience Manager
title: illum
topic: Scene7 Image Serving - Image Rendering API
uuid: f633c505-e3b2-49a0-9483-4c27fbed2fac
index: y
internal: n
snippet: y
---

# illum{#illum}

Illumination map selector. Specifies the illumination map this material prefers to be rendered with.

 `illum=-1|0|1|2`

If the specified illumination map is not available in the target vignette, the nearest available map is used instead.

`illum=-1` specifies that the illumination map is selected automatically based on the `gloss=` value.

## Properties {#section-aace8466566e4cf1a0c5a6c0167245c9}

Material attribute. Ignored if the vignette does not define multiple illumination maps.

## Default {#section-c96ecfb232074e80b6a29076f5199403}

`illum=-1`

## See also {#section-9132e60381c64aa3a8ed1319690db55e}

[gloss=](../../../../../ir_api/http_protocol/image-rendering-api-ref/c-ir-http-protocol-ref/c-ir-http-protocol-command-reference/r-ir-http-gloss.md#reference-325aef2ee51e4e1584a06047427340ca) 