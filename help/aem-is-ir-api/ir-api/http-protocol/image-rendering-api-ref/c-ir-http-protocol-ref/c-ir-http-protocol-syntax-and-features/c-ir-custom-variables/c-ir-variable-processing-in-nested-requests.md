---
description: $var$ references may occur anywhere within the curly braces of a nested Image Serving or Image Rendering request, including to the left of the '?' separating the path from the query.
seo-description: $var$ references may occur anywhere within the curly braces of a nested Image Serving or Image Rendering request, including to the left of the '?' separating the path from the query.
seo-title: Variable processing in nested requests
solution: Experience Manager
title: Variable processing in nested requests
topic: Scene7 Image Serving - Image Rendering API
uuid: 2f3fefac-d45e-4c53-854f-1fe16d0cedd9
---

# Variable processing in nested requests{#variable-processing-in-nested-requests}

$var$ references may occur anywhere within the curly braces of a nested Image Serving or Image Rendering request, including to the left of the '?' separating the path from the query.

The server substitutes these references with values (either from the url or from `catalog::Modifier` of the main image catalog) before further parsing and processing of the nested request.

In addition, all `$ *[!DNL var]*=` definitions from the url and `catalog::Modifier` are forwarded to all nested Image Serving and Image Rendering requests. This ensures that all variable definitions are available to all templates, regardless of nesting level.

Regardless of the nesting level, only single-pass HTTP-encoding must be applied to variable values which are to be substituted anywhere in nested Image Rendering or Image Serving requests. 
