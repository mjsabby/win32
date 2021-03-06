---
Description: The ISmartRenderEngine interface provides methods that support smart recompression in DirectShow Editing Services (DES). The smart render engine exposes this interface.
ms.assetid: 0e03708f-e471-4188-a212-ec5e951d20fa
title: ISmartRenderEngine interface
ms.topic: interface
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- ISmartRenderEngine
api_type: 
- COM
api_location: 
- strmiids.lib
- strmiids.dll
---

# ISmartRenderEngine interface

> [!Note]  
> \[Deprecated. This API may be removed from future releases of Windows.\]

 

The `ISmartRenderEngine` interface provides methods that support smart recompression in [DirectShow Editing Services](directshow-editing-services.md) (DES). The smart render engine exposes this interface.

## Members

The **ISmartRenderEngine** interface inherits from the [**IUnknown**](https://msdn.microsoft.com/en-us/library/ms680509(v=VS.85).aspx) interface. **ISmartRenderEngine** also has these types of members:

-   [Methods](#methods)

### Methods

The **ISmartRenderEngine** interface has these methods.



| Method                                                                | Description                                                                          |
|:----------------------------------------------------------------------|:-------------------------------------------------------------------------------------|
| [**GetGroupCompressor**](ismartrenderengine-getgroupcompressor.md)   | Retrieves the compression filter for the specified group.<br/>                 |
| [**SetFindCompressorCB**](ismartrenderengine-setfindcompressorcb.md) | Not implemented.<br/>                                                          |
| [**SetGroupCompressor**](ismartrenderengine-setgroupcompressor.md)   | Specifies a compression filter to use when rendering the specified group.<br/> |



 

## Remarks

> [!Note]  
> The header file Qedit.h is not compatible with Direct3D headers later than version 7.

 

> [!Note]  
> To obtain Qedit.h, download the [Microsoft Windows SDK Update for Windows Vista and .NET Framework 3.0](https://go.microsoft.com/fwlink/p/?linkid=129787). Qedit.h is not available in the Microsoft Windows SDK for Windows 7 and .NET Framework 3.5 Service Pack 1.

 

## Requirements



|                    |                                                                                         |
|--------------------|-----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>Qedit.h</dt> </dl>      |
| Library<br/> | <dl> <dt>Strmiids.lib</dt> </dl> |



## See also

<dl> <dt>

[Rendering a Project](rendering-a-project.md)
</dt> </dl>

 

 




