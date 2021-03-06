---
description: Apply PDF job options. A job options file or PDF preset is a file generated by Illustrator in the Save As PDF options dialog or PDF presets in InDesign.
seo-description: Apply PDF job options. A job options file or PDF preset is a file generated by Illustrator in the Save As PDF options dialog or PDF presets in InDesign.
seo-title: joboption
solution: Experience Manager
title: joboption
topic: Scene7 Image Serving - Image Rendering API
uuid: 7288cf29-850f-4121-8425-5f995daac22d
---

# joboption{#joboption}

Apply PDF job options. A job options file or PDF preset is a file generated by Illustrator in the Save As PDF options dialog or PDF presets in InDesign.

 ` joboption= *`value`*`

<table id="simpletable_BA7B58BE0B0740298D45DDEBE7832D93"> 
 <tr class="strow"> 
  <td class="stentry"> <p><span class="codeph"> <span class="varname"> value</span></span> </p> </td> 
  <td class="stentry"> <p>The IPSID of the job options file. </p></td> 
 </tr> 
</table>

The job options file can be uploaded and published by IPS/SPS. The PDF options contained in the job options file are used when the PDF is generated.

The following options are currently supported:

<table id="simpletable_7E0AE8A06AE54A02AF0107FBEDF73D61"> 
 <tr class="strow"> 
  <td class="stentry"> <p>General </p></td> 
  <td class="stentry"> <p> Compatibility </p> <p> Object Level Compression </p> <p> Embed thumbnails </p> <p> Optimize for fast web view </p> </td> 
 </tr> 
 <tr class="strow"> 
  <td class="stentry"> <p>Images </p></td> 
  <td class="stentry"> <p> Downsample, Resolution, Threshold, and Compression for color, gray, and mono </p> </td> 
 </tr> 
 <tr class="strow"> 
  <td class="stentry"> <p>Fonts </p></td> 
  <td class="stentry"> <p> Embed all fonts </p> <p> Embed OpenType fonts </p> <p> Subset embedded fonts when percent of characters used is less than: </p> <p> Always Embed List </p> <p> Never Embed List </p> </td> 
 </tr> 
 <tr class="strow"> 
  <td class="stentry"> <p>Color </p></td> 
  <td class="stentry"> <p> Color Strategy(Tag only images is treated as tag everything) </p> <p> Document Rendering Intent </p> <p> Only the following working spaces are supported for 4.2.5. </p> <p> 
    <ul id="ul_3F3EFDFB6A3340978AE31DEDF0FDA2C8"> 
     <li id="li_17A9FA99D6CA4C5182E383A85F0E3C90"> RGB <p> 
       <ul id="ul_1DD0C264DA1248319E751ADD18140C6D"> 
        <li id="li_B91B4D0C1D80442EB8690933AFA1F093"> e-sRGB </li> 
        <li id="li_D7F8C500DF5E4CBC8FFA4FEFB8E4E036"> scRGB with encoding range [-4.0, 4.0] </li> 
        <li id="li_942CD69732984E16A71C2F75EC5B5245"> Lab D50 </li> 
        <li id="li_7063B9E98D1E4946AC8F0EF7BC988806"> PCS XYZ </li> 
        <li id="li_5809447576B147B68630C4B7EC2E7870"> Flat XYZ </li> 
        <li id="li_3B5DA42A04124A6BAA12343AFC19F620">Linear ROMM-RGB </li> 
        <li id="li_DEC3028FA9C34176B761D12B7179B44F">ROMM-RGB </li> 
        <li id="li_3E7E7C4A680C4E3EADE0A26048ECF1F4"> sYCC 8-bit </li> 
        <li id="li_16A615C9A74D443AB3C63B3FE3AB5443"> e-sYCC 8-bit </li> 
       </ul> </p> </li> 
     <li id="li_AFA6D4D8C0624AA495E2EB2F0F0C7F7B">Gray <p> 
       <ul id="ul_945389DD426F44C09EB9C7F23933CB77"> 
        <li id="li_DB0AE3DFFC184480BB91666FF1BB4776">Gray Gamma 1.8 </li> 
        <li id="li_755C556ED94740D1BD30EBE67018E074">Gray Gamma 2.2 </li> 
        <li id="li_67437440AFB54B7686333A55233AA87F">Dot Gain 10% </li> 
        <li id="li_0D6CA6004EC84048B5F2198406F4F343">Dot Gain 15% </li> 
        <li id="li_1AFD11C23AB147978559D8F00BFB3142">Dot Gain 20% </li> 
        <li id="li_6CD5ACEF6B0B49E8BACA8264FE0E9C44"> Dot Gain 25% </li> 
        <li id="li_AB5F1FA7111041BD82353E02A284A546">Dot Gain 30% </li> 
        <li id="li_7433278AE8054AD28BD38A0A6E4EF7EF"> sGray </li> 
       </ul> </p> </li> 
    </ul> </p> <p> Preserve CMYK values for calibrated CMYK color spaces </p> </td> 
 </tr> 
 <tr class="strow"> 
  <td class="stentry"> <p>Advanced </p></td> 
  <td class="stentry"> <p>Preserve OPI comments is always turned on. </p></td> 
 </tr> 
 <tr class="strow"> 
  <td class="stentry"> <p>Standards </p></td> 
  <td class="stentry"> <p>Compliance standard. </p></td> 
 </tr> 
</table>

