---
description: JavaScript API reference for Basic Zoom Viewer
seo-description: JavaScript API reference for Basic Zoom Viewer
seo-title: setHandlers
solution: Experience Manager
title: setHandlers
topic: Dynamic media
uuid: 775e1561-3709-41e1-9146-dcc85f8a250d
index: y
internal: n
snippet: y
---

# setHandlers{#sethandlers}

JavaScript API reference for Basic Zoom Viewer

 `setHandlers(handlers)`

Specifies zero or more callback handlers. A call to this method fully overwrites event handlers that were previously assigned for that viewer instance. Must be called before `init()`.

## Parameter {#section-b60f082cca1542748b605689b1d43f8a}

<table id="table_98A620DAE2C340FA97BF7204AE023CC8"> 
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> <span class="varname"> handlers </span> </span> </p> </td> 
   <td colname="col2"> <p> <span class="codeph"> {Object} </span> JSON object with viewer event callbacks, where the property name is the name of the supported viewer event and the property value is a JavaScript function reference to an appropriate callback. </p> <p>See <a href="../../../c-html5-s7-aem-asset-viewers/c-html5-20-basic-zoom-viewer-about/c-html5-20-basic-zoom-viewer-event-callbacks.md#concept-8ba57cf86537401999514e1b221ec734" format="dita" scope="local"> Event callbacks </a> for more information about viewer events. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Returns {#section-1d3cf85bc7cc4dfe9670e038d02b9101}

None.

## Example {#section-9e9332aa86b74a5fb321375c03fdc5b3}

```
<instance>.setHandlers({ 
 "initComplete":function() { 
  console.log("init complete"); 
} 
})
```
