---
description: null
seo-description: null
seo-title: CarouselView.iscommand
solution: Experience Manager
title: CarouselView.iscommand
topic: Dynamic media
uuid: 005b130c-9316-4cf9-ae59-9f8ef381dda3
---

# CarouselView.iscommand{#carouselview-iscommand}

 ` [CarouselView.|<containerId>_carouselView.]iscommand= *`isCommand`*`

<table id="table_06B5F795889E402FB6BCEA4D882E1422"> 
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph"><span class="varname"> iscommand</span></span> </p> </td> 
   <td colname="col2"> <p> The Image Serving command string that is applied to the banner image. If specified in the URL all occurrences of <span class="codeph"> &amp;</span> and <span class="codeph"> =</span> must be HTTP-encoded as <span class="codeph"> %26</span> and <span class="codeph"> %3D</span>, respectively. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Properties {#section-1e637b22e8a44d759d588e47576891e6}

Optional.

## Default {#section-71fb773f814649b2885aefee68073641}

None.

## Example {#section-bce98c31f08a4a0ab262fab7f95ba020}

When specified in the viewer URL:

`iscommand=op_sharpen%3d1%26op_colorize%3d0xff0000`

When specified in the config data:

`iscommand=op_sharpen=1&op_colorize=0xff0000` 
