---
title: glNormal3sv function
description: Sets the current normal vector.
ms.assetid: 59cdebc9-594a-429f-ba5d-7c63a533cc11
keywords:
- glNormal3sv function OpenGL
topic_type:
- apiref
api_name:
- glNormal3sv
api_location:
- Opengl32.dll
api_type:
- DllExport
ms.topic: article
ms.date: 05/31/2018
---

# glNormal3sv function

Sets the current normal vector.

## Syntax


```C++
void WINAPI glNormal3sv(
   const GLshort *v
);
```



## Parameters

<dl> <dt>

*v* 
</dt> <dd>

A pointer to an array of three elements: the x, y, and z coordinates of the new current normal.

</dd> </dl>

## Return value

This function does not return a value.

## Remarks

The current normal is set to the given coordinates whenever you call the **glNormal3sv** function.

Byte, short, or integer arguments are converted to floating-point format with a linear mapping that maps the most positive representable integer value to 1.0, and the most negative representable integer value to -1.0.

Normals specified by using **glNormal3sv** need not have unit length. If normalization is enabled, then normals specified with **glNormal3sv** are normalized after transformation. You can control normalization by using [**glEnable**](glenable.md) and [**glDisable**](gldisable.md) with the argument GL\_NORMALIZE. By default, normalization is disabled. You can update the current normal at any time. In particular, you can call **glNormal3sv** between a call to [**glBegin**](glbegin.md) and the corresponding call to [**glEnd**](glend.md). The following functions retrieve information related to **glNormal3sv**:

[**glGet**](glgetbooleanv--glgetdoublev--glgetfloatv--glgetintegerv.md) with argument GL\_CURRENT\_NORMAL

[**glIsEnable**](glisenabled.md) with argument GL\_NORMALIZE

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

[**glIndex**](glindex-functions.md)
</dt> <dt>

[**glTexCoord**](gltexcoord-functions.md)
</dt> <dt>

[**glVertex**](glvertex-functions.md)
</dt> </dl>

 

 





