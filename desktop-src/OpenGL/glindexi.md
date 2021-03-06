---
title: glIndexi function
description: The glIndexi function sets the current color index.
ms.assetid: c57d2316-4081-40d8-af50-ae0299597803
keywords:
- glIndexi function OpenGL
topic_type:
- apiref
api_name:
- glIndexi
api_location:
- opengl32.dll
api_type:
- DllExport
ms.topic: article
ms.date: 05/31/2018
---

# glIndexi function

The **glIndexi** function sets the current color index.

## Syntax


```C++
void WINAPI glIndexi(
   GLint c
);
```



## Parameters

<dl> <dt>

*c* 
</dt> <dd>

The new value for the current color index.

</dd> </dl>

## Return value

This function does not return a value.

## Remarks

The **glIndexi** function updates the current (single-valued) color index. It takes one argument: the new value for the current color index.

The current index is stored as a floating-point value. Integer values are converted directly to floating-point values, with no special mapping.

Index values outside the representable range of the color-index buffer are not clamped. However, before an index is dithered (if enabled) and written to the framebuffer, it is converted to fixed-point format. Any bits in the integer portion of the resulting fixed-point value that do not correspond to bits in the framebuffer are masked out.

The current index can be updated at any time. In particular, **glIndexi** can be called between a call to [**glBegin**](https://docs.microsoft.com/windows/desktop/OpenGL/glbegin) and the corresponding call to [**glEnd**](glend.md).

The following function retrieves information related to **glIndexi**:

[**glGet**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md) with argument GL\_CURRENT\_INDEX

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                              |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                    |
| Header<br/>                   | <dl> <dt>Gl.h</dt> </dl>         |
| Library<br/>                  | <dl> <dt>Opengl32.lib</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Opengl32.dll</dt> </dl> |



## See also

<dl> <dt>

[**glBegin**](glbegin.md)
</dt> <dt>

[**glColor**](glcolor-functions.md)
</dt> <dt>

[**glEnd**](glend.md)
</dt> <dt>

[**glGet**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md)
</dt> </dl>

 

 





