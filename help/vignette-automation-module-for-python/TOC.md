---
cloud: experience-cloud
product: adobe
archtype: end-user
user-guide-title: Dynamic Media Vignette Automation Module for Python
---

# Dynamic Media Vignette Automation Module for Python {#vignette-automation}

+ [Dynamic Media Vignette Automation Module for Python](c-vampyhome.md)
+ [Example Script](c-example-script.md)
+ Typical Script Workflow {#typical-script-workflow}
   + [Typical Script Workflow Overview](c-typical-script-workflow/c-typical-script-workflow.md)
   + [Gather Image and Data](c-typical-script-workflow/c-gather-image-and-data.md)
   + [Create a Vignette](c-typical-script-workflow/c-creating-a-vignette.md)
   + [Add Objects and Groups](c-typical-script-workflow/c-add-objects-and-groups.md)
   + Initialize Surface and Flat Objects {#initialize-surface-flat}
      + [Initialize Surface and Flat Objects](c-typical-script-workflow/c-init-surface-and-flat-objects/c-init-surface-and-flat-objects.md)
      + [Surface Objects](c-typical-script-workflow/c-init-surface-and-flat-objects/t-surface-objects.md)
      + [Flat Objects](c-typical-script-workflow/c-init-surface-and-flat-objects/t-flat-objects.md)
   + [Add Local Illumination Maps for Overlapping Objects](c-typical-script-workflow/c-add-local-illumination-maps.md)
   + [Configure Origin Points](c-typical-script-workflow/c-configure-origin-points.md)
   + [Configure the Decal Anchor Point](c-typical-script-workflow/c-configure-decal-anchor-point.md)
   + [Save the Vignette](c-typical-script-workflow/c-save-the-vignette.md)
+ s7vampy API Reference {#s7vampy-api-reference}
   + [s7vampy API Reference Overview](c-s7vampy-api-reference/c-s7vampy-api-reference.md)
   + Functions {#functions}
      + [Functions Overview](c-s7vampy-api-reference/c-functions/c-functions.md)
      + [create_path](c-s7vampy-api-reference/c-functions/r-s7vampy.create-path.md)
      + [create_vignette](c-s7vampy-api-reference/c-functions/r-s7vampy-create-vignette.md)
      + [s7vampy.create_rgb](c-s7vampy-api-reference/c-functions/r-s7vampy.create-rgb.md)
      + [s7vampy.create_rgba(image)](c-s7vampy-api-reference/c-functions/r-s7vampy.create-rgba.md)
      + [s7vampy.create_gray(image)](c-s7vampy-api-reference/c-functions/r-s7vampy.create-gray.md)
      + [extract_alpha](c-s7vampy-api-reference/c-functions/r-s7vampy-extract-alpha.md)
      + [invert_image](c-s7vampy-api-reference/c-functions/r-s7vampy-invert-image.md)
      + [merge_additive](c-s7vampy-api-reference/c-functions/r-s7vampy-merge-additive.md)
      + [merge_additive_mask](c-s7vampy-api-reference/c-functions/r-s7vampy-merge-additive-mask.md)
      + [s7vampy.add_alpha(image)](c-s7vampy-api-reference/c-functions/r-s7vampy-add-alpha.md)
      + [open_image](c-s7vampy-api-reference/c-functions/r-s7vampy.open-image.md)
      + [open_rla](c-s7vampy-api-reference/c-functions/r-s7vampy.open-rla.md)
      + [open_vignette](c-s7vampy-api-reference/c-functions/r-s7vampy-open-vignette.md)
   + Classes {#classes}
      + [Classes Overview](c-s7vampy-api-reference/c-classes/c-classes.md)
      + Exceptions {#exceptions}
         + [Exceptions](c-s7vampy-api-reference/c-classes/c-classes-exceptions/c-classes-exceptions.md)
         + [ArgumentError](c-s7vampy-api-reference/c-classes/c-classes-exceptions/r-exception-s7vampy.error.argumenterror.md)
      + Image Classes {#image-classes}
         + [Image Classes](c-s7vampy-api-reference/c-classes/c-classes-image/c-classes-image.md)
         + [Image](c-s7vampy-api-reference/c-classes/c-classes-image/r-class-s7vampy.image.image.md)
      + RLA Classes {#rla-classes}
         + [RLA (Run-Length Encoded, Version A) Classes](c-s7vampy-api-reference/c-classes/c-rla/c-rla.md)
         + [RLA](c-s7vampy-api-reference/c-classes/c-rla/r-class-s7vampy-rla.md)
      + Path Classes {#path-classes}
         + [Path Classes](c-s7vampy-api-reference/c-classes/c-path/c-path.md)
         + [Path](c-s7vampy-api-reference/c-classes/c-path/r-class-s7vampy-path-path.md)
         + [Contour](c-s7vampy-api-reference/c-classes/c-path/r-class-s7vampy-path-contour.md)
         + [Segment](c-s7vampy-api-reference/c-classes/c-path/r-class-s7vampy-path-segment.md)
      + Vignette Classes {#vignette-classes}
         + [Vignette Classes](c-s7vampy-api-reference/c-classes/c-vignette/c-vignette.md)
         + [Vignette](c-s7vampy-api-reference/c-classes/c-vignette/r-class-s7vampy-vignette-vignette.md)
      + View Classes {#view-classes}
         + [View Classes](c-s7vampy-api-reference/c-classes/c-view/c-view.md)
         + [View](c-s7vampy-api-reference/c-classes/c-view/r-s7vampy-view-view.md)
      + Object Classes {#object-classes}
         + [Object Classes](c-s7vampy-api-reference/c-classes/c-objects/c-objects.md)
         + [ObjectHierarchy](c-s7vampy-api-reference/c-classes/c-objects/r-s7vampy-obj-objecthierarchy.md)
         + [ObjectList](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-objectlist.md)
         + [Object](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-object.md)
         + [Group](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-group.md)
         + [BackgroundObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-backgroundobject.md)
         + [StaticObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-staticobject.md)
         + [StaticOverlapObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-staticoverlapobject.md)
         + [NonTexturableObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-nontexturableobject.md)
         + [SurfaceObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-surfaceobject.md)
         + [FlatObject](c-s7vampy-api-reference/c-classes/c-objects/r-class-s7vampy-obj-flatobject.md)
      + Origin Point Classes {#origin-point-classes}
         + [Origin Point Classes](c-s7vampy-api-reference/c-classes/c-origin-points/c-origin-points.md)
         + [OriginPoints](c-s7vampy-api-reference/c-classes/c-origin-points/r-class-s7vampy-origin-originpoints.md)
      + Illumination Map Classes {#illumination-map-classes}
         + [Illumination Map Classes](c-s7vampy-api-reference/c-classes/c-illumination-maps/c-illumination-maps.md)
         + [IlluminationMaps](c-s7vampy-api-reference/c-classes/c-illumination-maps/r-s7vampy-illum-illuminationmaps.md)