---
description: The eCatalog Search Viewer supports Adobe Analytics tracking out of the box.
seo-description: The eCatalog Search Viewer supports Adobe Analytics tracking out of the box.
seo-title: Support for Adobe Analytics tracking
solution: Experience Manager
title: Support for Adobe Analytics tracking
topic: Dynamic media
uuid: 2e1e2bc6-5372-4ba2-b6d7-8b760b1b0a8a
index: y
internal: n
snippet: y
---

# Support for Adobe Analytics tracking{#support-for-adobe-analytics-tracking}

The eCatalog Search Viewer supports Adobe Analytics tracking out of the box.

## Out-of-the-box tracking {#section-ba994f079d0343c8ae48adffaa3195a3}

The eCatalog Search Viewer supports [!DNL Adobe Analytics] tracking out-of-the-box. To enable tracking, pass the proper company preset name as `config2` parameter.

The viewer also sends a single tracking HTTP request to the configured Image Server with the viewer type and version information.

## Custom tracking {#section-cda48fc9730142d0bb3326bac7df3271}

To integrate with third-party analytics systems it is necessary to listen to the `trackEvent` viewer callback and process the `eventInfo` argument of the callback function as necessary. The following code is an example of such handler function:

```
var eCatalogSearchViewer = new s7viewers.eCatalogSearchViewer({ 
 "containerId":"s7viewer", 
"params":{ 
 "asset":"Viewers/Pluralist", 
 "serverurl":"http://s7d1.scene7.com/is/image/" 
}, 
"handlers":{ 
 "trackEvent":function(objID, compClass, instName, timeStamp, eventInfo) { 
  //identify event type 
  var eventType = eventInfo.split(",")[0]; 
  switch (eventType) { 
   case "LOAD": 
    //custom event processing code 
    break; 
   //additional cases for other events 
} 
} 
} 
});
```

The viewer tracks the following SDK user events:

<table id="table_5D090E6614974D968E1A93B5727D859C"> 
 <thead> 
  <tr> 
   <th colname="col1" class="entry"> <p>SDK user event </p> </th> 
   <th colname="col2" class="entry"> <p>Sent when... </p> </th> 
  </tr> 
 </thead>
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> LOAD </span> </p> </td> 
   <td colname="col2"> <p>viewer is loaded first. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> SWAP </span> </p> </td> 
   <td colname="col2"> <p>an asset is swapped in the viewer using the <span class="codeph"> setAsset() </span> API. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> ZOOM </span> </p> </td> 
   <td colname="col2"> <p> an image is zoomed. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> PAN </span> </p> </td> 
   <td colname="col2"> <p>an image is panned. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> SWATCH </span> </p> </td> 
   <td colname="col2"> <p> an image is change by clicking or tapping on a swatch. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> PAGE </span> </p> </td> 
   <td colname="col2"> <p> a current frame is changed in the main view. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> ITEM </span> </p> </td> 
   <td colname="col2"> <p>an info panel pop-up is activated. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> HREF </span> </p> </td> 
   <td colname="col2"> <p>a user navigates to a different page because of clicking the image map. </p> </td> 
  </tr> 
 </tbody> 
</table>
