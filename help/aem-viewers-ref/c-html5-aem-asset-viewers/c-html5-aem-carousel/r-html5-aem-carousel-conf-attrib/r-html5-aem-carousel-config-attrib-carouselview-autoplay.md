---
description: Configuration attribute for Carousel Viewer.
seo-description: Configuration attribute for Carousel Viewer.
seo-title: CarouselView.autoplay
solution: Experience Manager
title: CarouselView.autoplay
topic: Dynamic media
uuid: 12730b17-110e-405b-97fe-e70fab89c703
---

# CarouselView.autoplay{#carouselview-autoplay}

Configuration attribute for Carousel Viewer.

 `[CarouselView.|<containerId>_carouselView.]autoplay=[0|1][,duration][,direction]`

<table id="table_441553CD34C94A58A9D7CBF772DEDDB6"> 
 <tbody> 
  <tr> 
   <td colname="col1"> <p> <span class="codeph">[0|1][,duration][,direction]</span> </p> </td> 
   <td colname="col2"> <p> Specifies on/off, duration to display each banner in the carousel and direction of auto-loop. </p> <p>Set to <span class="codeph"> 0</span> for auto-loop off. </p> <p>Set <span class="codeph"> 1</span> to auto-loop on with transition duration in seconds controlled by <span class="codeph"> duration</span>. </p> <p>The direction of auto-loop is controlled with <span class="codeph"> direction</span>. The <span class="codeph"> direction</span> has the range between <span class="codeph"> 1</span> right-to-left and <span class="codeph"> 0</span> left-to-right. </p> </td> 
  </tr> 
 </tbody> 
</table>

## Properties {#section-1e637b22e8a44d759d588e47576891e6}

Optional.

## Default {#section-71fb773f814649b2885aefee68073641}

`1,9`

## Example {#section-bce98c31f08a4a0ab262fab7f95ba020}

```
autoplay=1,2,1
```

