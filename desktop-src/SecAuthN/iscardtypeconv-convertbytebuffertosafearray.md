---
Description: Converts a universal buffer of bytes (IStream object) into a SAFEARRAY of unsigned char (byte).
ms.assetid: b8d052e8-2f36-42cf-b88c-ace215a2fc68
title: ISCardTypeConv::ConvertByteBufferToSafeArray method
ms.topic: article
ms.date: 05/31/2018
topic_type: 
- APIRef
- kbSyntax
api_name: 
- ISCardTypeConv.ConvertByteBufferToSafeArray
api_type: 
- COM
api_location: 
- Scardssp.dll
---

# ISCardTypeConv::ConvertByteBufferToSafeArray method

\[The **ConvertByteBufferToSafeArray** method is available for use in the operating systems specified in the Requirements section. It is not available for use in Windows Server 2003 with Service Pack 1 (SP1) and later, Windows Vista, Windows Server 2008, and subsequent versions of the operating system. The [Smart Card Modules](https://msdn.microsoft.com/en-us/library/Dd627652(v=VS.85).aspx) provide similar functionality.\]

The **ConvertByteBufferToSafeArray** method converts a universal buffer of bytes (**IStream** object) into a SAFEARRAY of unsigned char (byte).

## Syntax


```C++
HRESULT ConvertByteBufferToSafeArray(
  [in]  LPBYTEBUFFER pbyBuffer,
  [out] LPSAFEARRAY  *ppbyArray
);
```



## Parameters

<dl> <dt>

*pbyBuffer* \[in\]
</dt> <dd>

Pointer to the **IStream** object to be converted.

</dd> <dt>

*ppbyArray* \[out\]
</dt> <dd>

Pointer to the SAFEARRAY to be returned.

</dd> </dl>

## Return value

The method returns one of the following possible values:



| Return code                                                                                   | Description                                                                                      |
|-----------------------------------------------------------------------------------------------|--------------------------------------------------------------------------------------------------|
| <dl> <dt>**S\_OK**</dt> </dl>          | Memory allocated successfully.<br/>                                                        |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | There is something wrong with one or more of the parameters passed into the function.<br/> |
| <dl> <dt>**E\_POINTER**</dt> </dl>     | A parameter of pointer type was incorrect.<br/>                                            |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | Not enough free memory to satisfy request.<br/>                                            |



 

## Requirements



|                                     |                                                                                         |
|-------------------------------------|-----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP \[desktop apps only\]<br/>                                             |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                    |
| End of client support<br/>    | Windows XP<br/>                                                                   |
| End of server support<br/>    | Windows Server 2003<br/>                                                          |
| Header<br/>                   | <dl> <dt>Scarddat.h</dt> </dl>   |
| Type library<br/>             | <dl> <dt>Scarddat.tlb</dt> </dl> |
| DLL<br/>                      | <dl> <dt>Scardssp.dll</dt> </dl> |
| IID<br/>                      | IID\_ISCardTypeConv is defined as 53B6AA63-3F56-11D0-916B-00AA00C18068<br/>       |



## See also

<dl> <dt>

[**ISCardTypeConv**](iscardtypeconv.md)
</dt> <dt>

[Smart Card Return Values](authentication-return-values.md)
</dt> </dl>

 

 




