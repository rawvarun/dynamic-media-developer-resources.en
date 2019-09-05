---
description: All fonts referenced in the RTF string must be available in the font map file of the default catalog or the current image catalog, otherwise an error is returned.
seo-description: All fonts referenced in the RTF string must be available in the font map file of the default catalog or the current image catalog, otherwise an error is returned.
seo-title: Font handling
solution: Experience Manager
title: Font handling
topic: Scene7 Image Serving - Image Rendering API
uuid: 10082c23-d041-4259-aa87-9b847d4ffb1b
index: y
internal: n
snippet: y
---

# Font handling{#font-handling}

All fonts referenced in the RTF string must be available in the font map file of the default catalog or the current image catalog, otherwise an error is returned.

Best quality for italic and bold-face text is achieved by registering the corresponding font files. If not available, the server can synthesize bold and/or italic font faces from the standard face. (See ` [attribute::SynthesizeFontStyles](../../../../../is_api/image_catalog/image-serving-api-ref/c-image-catalog-reference/c-attributes-reference/r-synthesizefontstyles.md#reference-1b12ba881b9146c793bcb07407cacb15)`.)

The font face specified with `attribute::DefaultFont` is used when none are specified explicitly in the RTF string.

Image Serving supports TrueType, OpenType, Adobe Type 1 (Windows only) fonts.

## Photofont® font support {#section-74560ae898cf4708aba4c8b4093f5f00}

`textPs=` supports Photofont® fonts, with the following restrictions:

* `\cf` is ignored in text spans that specify a Photofont font; Photofont font faces have predefined colors 
* Synthesized font styles are not supported; use of `\b` and `\i`require corresponding font map entries, otherwise an error is returned 

* Vertical text flow is not supported 
* Photofont fonts with 16 bit images are not supported 
* Photofont fonts with multiple glyphs per image are not supported 
* Naïve color conversion is applied unless the Photofont glyph images embed color profiles; in this case, relative colorimetric render intent and blackpoint compensation are always applied

Refer to ` [www.photofont.com](http://www.photofont.com)` for additional information.

## See also {#section-6cb8a802aa044836bbe449d559093f3a}

[Font Map Reference](../../../../../is_api/image_catalog/image-serving-api-ref/c-image-catalog-reference/c-font-map-reference/c-font-map-reference.md#concept-f81f319d03c646c5a8ef87b3277dd37d), [attribute::SynthesizeFontStyles](../../../../../is_api/image_catalog/image-serving-api-ref/c-image-catalog-reference/c-attributes-reference/r-synthesizefontstyles.md#reference-1b12ba881b9146c793bcb07407cacb15), [attribute::DefaultFont](../../../../../is_api/image_catalog/image-serving-api-ref/c-image-catalog-reference/c-attributes-reference/r-defaultfont.md#reference-48b763ac254545e89a25c76ff7581107), [ [!DNL www.photofont.com] ](http://www.photofont.com) 