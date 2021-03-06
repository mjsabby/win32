---
title: ID3DX11EffectPass IsValid method
description: Test a pass to see if it contains valid syntax.
ms.assetid: 3c6ddcef-1303-4161-889c-c3ca271b6ad0
keywords:
- IsValid method Direct3D 11
- IsValid method Direct3D 11 , ID3DX11EffectPass interface
- ID3DX11EffectPass interface Direct3D 11 , IsValid method
topic_type:
- apiref
api_name:
- ID3DX11EffectPass.IsValid
api_location:
- N/A
- N/A.dll
api_type:
- COM
ms.topic: article
ms.date: 05/31/2018
---

# ID3DX11EffectPass::IsValid method

Test a pass to see if it contains valid syntax.

## Syntax


```C++
BOOL IsValid();
```



## Parameters

This method has no parameters.

## Return value

Type: **[**BOOL**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)**

**TRUE** if the code syntax is valid; otherwise **FALSE**.

## Remarks

> [!Note]  
> The DirectX SDK does not supply any compiled binaries for effects. You must use Effects 11 source to build your effects-type application. For more information about using Effects 11 source, see [Differences Between Effects 10 and Effects 11](d3d11-graphics-programming-guide-effects-differences.md).

 

## Requirements



|                    |                                                                                                                                              |
|--------------------|----------------------------------------------------------------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx11effect.h</dt> </dl>                                                    |
| Library<br/> | <dl> <dt>N/A (An Effects 11 library is available online as shared source.)</dt> </dl> |



## See also

<dl> <dt>

[ID3DX11EffectPass](id3dx11effectpass.md)
</dt> </dl>

 

 





