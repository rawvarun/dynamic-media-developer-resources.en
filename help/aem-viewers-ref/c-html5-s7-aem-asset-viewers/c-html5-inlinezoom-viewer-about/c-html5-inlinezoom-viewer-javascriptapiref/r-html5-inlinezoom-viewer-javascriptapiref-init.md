---
description: JavaScript API reference for Inline Zoom Viewer.
seo-description: JavaScript API reference for Inline Zoom Viewer.
seo-title: init
solution: Experience Manager
title: init
topic: Dynamic media
uuid: a3bd0cd1-e4cb-4b09-a78f-0958b55a79e4
---

# init{#init}

JavaScript API reference for Inline Zoom Viewer.

 `init()`

Starts the initialization of the viewer so that the viewer code can find it by its ID. By this time the container DOM element must be created.

If the container element is not a part of the web page layout just yet (for example, it may be hidden using `display:none` style assigned to it), the viewer suspends its initialization process until the moment when the web page brings the container element back to the layout. When this occurs, the viewer load automatically resumes.

Only call this method once during the viewer life cycle; subsequent calls are ignored.

## Parameters {#section-ad069aaaf4f145f2b50ae5ac89ca1ed2}

None.

## Returns {#section-1d3cf85bc7cc4dfe9670e038d02b9101}

`{Object}` A reference to the viewer instance.

## Example {#section-9e9332aa86b74a5fb321375c03fdc5b3}

```
<instance>.init()
```

