---
description: null
seo-description: null
seo-title: FlyoutZoomView.zoomfactor
solution: Experience Manager
title: FlyoutZoomView.zoomfactor
topic: Dynamic media
uuid: 58d49de7-4828-46ae-b2e7-eb9398e98a99
---

# FlyoutZoomView.zoomfactor{#flyoutzoomview-zoomfactor}

 ` [FlyoutZoomView.|<containerId>_flyout.]zoomfactor= *`primaryFactor`*[,[ *`secondaryFactor`*][, *`upscale`*]]`

<table id="table_9B98C97485DD4DEB8A6ECBCE8DF6B886"> 
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> <span class="varname"> primaryFactor</span> </span> </p> </td> 
   <td colname="col2"> <p> Specifies the image magnification for the flyout view, relative to the main view. Must be an integer or floating point value <span class="codeph"> 1.0</span> or larger. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"> <span class="varname"> secondaryFactor</span> </span> </p> </td> 
   <td colname="col2"> <p> An optional secondary factor can be specified which is accessible by clicking or tapping on the main view when the highlight is active. Clicking or tapping a second time reverts to the primary zoom factor. A value of <span class="codeph"> -1</span> disables the secondary zoom factor. </p> </td> 
  </tr> 
  <tr> 
   <td colname="col1"> <p><span class="codeph"><span class="varname"> upscale</span></span> </p> </td> 
   <td colname="col2"> <p>Specifies how the component handles small images. </p> <p>If set to <span class="codeph"> 1</span> the component upscales the main image so that it fits within the main view. Also, it upscales the zoom image so that it completely fills the configured flyout window area. </p> <p>If set to <span class="codeph"> 0</span> small images are displayed at their original resolution and display centered in the main view area and inside the flyout window. You can configure extra white space that appears around the image with a background or similar CSS property of the <span class="codeph"> s7flyoutzoomview</span> and <span class="codeph"> s7flyoutzoom</span> CSS classes in the main view and flyout window, respectively. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Properties {#section-5526a5d19e7e4ee2a35b1c4816ed4202}

Optional.

## Default {#section-a08032f0fcf041c09e63c0238a339fc9}

`3,-1,1`

## Example {#section-0338be21edd04ff1a3bed5c8319b61a4}

`zoomfactor=2,3,0` 
