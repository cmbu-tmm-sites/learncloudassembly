---
title: "Image Mappings"
weight: 50
---

A [vRealize Automation](https://www.vmware.com/products/vrealize-automation.html) image map is where you use natural language to define target deployment operating systems for a specific [cloud account](/Infrastructure/Connections/Cloud-Accounts/)/region.

{{< img src="/Infrastructure/Configure/Image-Mappings/imagemapping-concept.png" alt="Image mapping to instance types in native clouds" >}}

Create mapping relationship between images in multiple clouds, apply image level constraints to control placement per image and apply image level CloudConfig customizations.

An image mapping associates a defined image name with a machine [cloud template](Design/Cloud_Templates/). 

{{< img src="/Infrastructure/Configure/Image-Mappings/imagemapping-display.png" alt="Image Mapping List" >}}

You can create one or more image names and map to a metadata file that contain pre-defined value sets. 
For example, an image might map to an OVA file that contains pre-populated cost or region specifications to import into the [cloud template](Design/Cloud_Templates/). Image mappings are regional settings.

{{< img src="/Infrastructure/Configure/Image-Mappings/imagemapping-details.png" alt="Image Mapping Details" >}}