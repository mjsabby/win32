---
Description: Creates a mesh object using a declarator.
ms.assetid: ff977517-0a46-4c32-8d5e-f5fc3c1718c1
title: D3DXCreateMesh function
ms.topic: article
ms.date: 05/31/2018
topic_type:
- APIRef
- kbSyntax
api_name:
- D3DXCreateMesh
api_type:
- LibDef
api_location:
- d3dx9.lib
- d3dx9.dll
---

# D3DXCreateMesh function

Creates a mesh object using a declarator.

## Syntax


```C++
HRESULT D3DXCreateMesh(
  _In_        DWORD               NumFaces,
  _In_        DWORD               NumVertices,
  _In_        DWORD               Options,
  _In_  const LPD3DVERTEXELEMENT9 *pDeclaration,
  _In_        LPDIRECT3DDEVICE9   pD3DDevice,
  _Out_       LPD3DXMESH          *ppMesh
);
```



## Parameters

<dl> <dt>

*NumFaces* \[in\]
</dt> <dd>

Type: **[**DWORD**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Number of faces for the mesh. The valid range for this number is greater than 0, and one less than the maximum DWORD (typically 65534), because the last index is reserved.

</dd> <dt>

*NumVertices* \[in\]
</dt> <dd>

Type: **[**DWORD**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Number of vertices for the mesh. This parameter must be greater than 0.

</dd> <dt>

*Options* \[in\]
</dt> <dd>

Type: **[**DWORD**](https://msdn.microsoft.com/en-us/library/Aa383751(v=VS.85).aspx)**

Combination of one or more flags from the [**D3DXMESH**](https://msdn.microsoft.com/en-us/library/Bb205370(v=VS.85).aspx) enumeration, specifying options for the mesh.

</dd> <dt>

*pDeclaration* \[in\]
</dt> <dd>

Type: **const [**LPD3DVERTEXELEMENT9**](d3dvertexelement9.md)\***

Array of [**D3DVERTEXELEMENT9**](d3dvertexelement9.md) elements, describing the vertex format for the returned mesh. This parameter must map directly to a flexible vertex format (FVF).

</dd> <dt>

*pD3DDevice* \[in\]
</dt> <dd>

Type: **[**LPDIRECT3DDEVICE9**](https://msdn.microsoft.com/library/Bb174336(v=VS.85).aspx)**

Pointer to an [**IDirect3DDevice9**](https://msdn.microsoft.com/library/Bb174336(v=VS.85).aspx) interface, the device object to be associated with the mesh.

</dd> <dt>

*ppMesh* \[out\]
</dt> <dd>

Type: **[**LPD3DXMESH**](id3dxmesh.md)\***

Address of a pointer to an [**ID3DXMesh**](id3dxmesh.md) interface, representing the created mesh object.

</dd> </dl>

## Return value

Type: **[**HRESULT**](https://msdn.microsoft.com/en-us/library/Bb401631(v=MSDN.10).aspx)**

If the function succeeds, the return value is D3D\_OK. If the function fails, the return value can be one of the following: D3DERR\_INVALIDCALL, E\_OUTOFMEMORY.

## Requirements



|                    |                                                                                        |
|--------------------|----------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3DX9Mesh.h</dt> </dl> |
| Library<br/> | <dl> <dt>D3dx9.lib</dt> </dl>   |



## See also

<dl> <dt>

[Mesh Functions](dx9-graphics-reference-d3dx-functions-mesh.md)
</dt> <dt>

[**D3DXDeclaratorFromFVF**](d3dxdeclaratorfromfvf.md)
</dt> </dl>

 

 




