---
description: Image Rendering configuration settings are stored in the Platform Server configuration file.
seo-description: Image Rendering configuration settings are stored in the Platform Server configuration file.
seo-title: Configuration files
solution: Experience Manager
title: Configuration files
topic: Scene7 Image Serving - Image Rendering API
uuid: 86263aac-bedd-4064-bad9-68d9c2e8c70f
index: y
internal: n
snippet: y
---

# Configuration files{#configuration-files}

Image Rendering configuration settings are stored in the Platform Server configuration file.

The platform server configuration file is located at [!DNL *[!DNL install_root]*/ImageServing/conf/PlatformServer.conf]. This file is a JAVA properties file. Care must be taken to follow the appropriate conventions, otherwise the Platform Server might fail to start. A double backslash (\\) or a single forward slash (/) must be used instead of a simple backslash (\) in Windows file paths, because the backslash is used as an escape character in this type of file. The file contains undocumented properties, which are for internal server use and must not be modified.

Refer to the [Configuration Settings Reference](../../../../../ir_api/server_admin/image-rendering-api-ref/c-ir-server-administration/c-ir-configuration-settings-reference/c-ir-configuration-settings-reference.md#concept-6947a512d4c94e9fb8a71b80243fee81) for a list of all Image Rendering configuration settings. 