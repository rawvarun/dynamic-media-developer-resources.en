---
description: HTTP response header element. Optional in <rule> elements.
seo-description: HTTP response header element. Optional in <rule> elements.
seo-title: header
solution: Experience Manager
title: header
topic: Scene7 Image Serving - Image Rendering API
uuid: 89ec0f27-fc12-47c2-b9dd-e0ee768587b5
---

# header{#header}

HTTP response header element. Optional in `<rule>` elements.

## Attributes {#section-6e903ab4c64f4b1488b8ae74274f50a6}

**`Name` = "*text*"** : Required. Specifies the name of the HTTP header.

**`Action` = "set" | `"add"`**: Optional. Default is `"set"`, which replaces any current header value. Specify `"add"` to append the header value, separated with a comma.

## Data {#section-a387f541396c49d99c29692a38032914}

Header value.

## Description {#section-fb2a8ad79bc5414d8bb0d0e8199f3269}

Allows adding new HTTP response headers as well as adding or replacing values of pre-defined headers. Names and values must conform to HTTP standards. No additional encoding will be applied.

Image Serving substitution variables may be used in the header name and the header value. This allows controlling both strings from the request.

## Example {#section-cb5b738b9b93407cb2f4d35af3e59c02}

The following rule applies a custom header when the header value is specified in the request as a variable:

```
<rule OnMatch="continue">
   <expression>\$Edge-Control=</expression>
   <header Name="Edge-Control">$Edge-Control$</header>
</rule>

```

This rule is triggered by the following request, setting the HTTP response header `Edge-Control::no-store`:

`http://server/is/image/cat/id?$Edge-Control=no-store` 
