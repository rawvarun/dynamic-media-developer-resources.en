---
description: Generates a new password.
seo-description: Generates a new password.
seo-title: generatePassword
solution: Experience Manager
title: generatePassword
topic: Scene7 Image Production System API
uuid: e3367bfc-d437-4a61-83e8-69830154dc61
---

# generatePassword{#generatepassword}

Generates a new password.

 Syntax 

## Authorized User Types {#section-88f7dc11e5c74be281399d8f2e3c9555}

* `IpsUser` 
* `IpsAdmin` 
* `IpsCompanyAdmin` 
* `TrialSiteUser` 
* `ImagePortalAdmin` 
* `ImagePortalUser` 
* `ImagePortalContrib` 
* `ImagePortalContribUser`

## Parameters {#section-d516615c906240819a284786efb19863}

**Input (generatePasswordParam)**

None.

**Output (generatePasswordParam)** 

|  Name  | Type  | Required  | Description  |
|---|---|---|---|
|  ` *`password`*`  | `xsd:string`  | Yes  | A new password.  |

## Examples {#section-f580fefdccec46fe95359e3aef0ed17f}

This code sample generates a password. It is unusual because the request is simply a parameter without any enclosed elements or values. IPS returns a strong password.

**Request** 

```java
<generatePasswordParam xmlns="http://www.scene7.com/IpsApi/xsd">
</generatePasswordParam>
```

**Response** 

```java
<generatePasswordReturn xmlns="http://www.scene7.com/IpsApi/xsd">
   <password>1\7aQRn]</password>
</generatePasswordReturn>
```

