---
Description: Retrieves the major version number of the template.
ms.assetid: efde3a7c-48e0-4bfe-9118-3098c7ef8771
title: Template.MajorVersion property
ms.topic: article
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- Template.MajorVersion
api_type:
- COM
api_location:
- Capicom.dll
---

# Template.MajorVersion property

\[The **MajorVersion** property is available for use in the operating systems specified in the Requirements section. Instead, use the [**X509Extension Class**](https://msdn.microsoft.com/library/x5x51x86(v=VS.100).aspx) in the [**System.Security.Cryptography.X509Certificates**](https://msdn.microsoft.com/library/73091bzx(v=VS.71).aspx) namespace by calling the constructor that takes an OID as a parameter, and then use the OID for Certificate Template to retrieve the certificate extension template.\]

The **MajorVersion** property retrieves the major version number of the template.

## Syntax


```VB
Template.MajorVersion As Long
```



## Property value

The major version number of the template.

## Requirements



|                            |                                                                                        |
|----------------------------|----------------------------------------------------------------------------------------|
| Redistributable<br/> | CAPICOM 2.0 or later on Windows Server 2003 and Windows XP<br/>                  |
| DLL<br/>             | <dl> <dt>Capicom.dll</dt> </dl> |



## See also

<dl> <dt>

[**Template**](template.md)
</dt> </dl>

 

 




