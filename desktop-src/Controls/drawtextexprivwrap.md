---
title: DrawTextExPrivWrap function
description: Draws formatted text in the specified rectangle. This function wraps a call to DrawTextEx.
ms.assetid: 3212282c-1adb-4f7e-b4d7-7d833b26ac60
keywords:
- DrawTextExPrivWrap function Windows Controls
topic_type:
- apiref
api_name:
- DrawTextExPrivWrap
api_location:
- Comctl32.dll
api_type:
- DllExport
ms.topic: article
ms.date: 05/31/2018
---

# DrawTextExPrivWrap function

\[**DrawTextExPrivWrap** is available through Windows XP with Service Pack 2 (SP2). It might be altered or unavailable in subsequent versions. It is recommended to use [**DrawTextEx**](https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-drawtextexa) directly instead.\]

Draws formatted text in the specified rectangle. This function wraps a call to [**DrawTextEx**](https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-drawtextexa).

## Syntax


```C++
int WINAPI DrawTextExPrivWrap(
  _In_    HDC              hdc,
  _Inout_ LPTSTR           lpchText,
  _In_    int              cchText,
  _Inout_ LPRECT           lprc,
  _In_    UINT             dwDTFormat,
  _In_    LPDRAWTEXTPARAMS lpDTParams
);
```



## Parameters

<dl> <dt>

*hdc* \[in\]
</dt> <dd>

Type: **[**HDC**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)**

A handle to the device context in which to draw.

</dd> <dt>

*lpchText* \[in, out\]
</dt> <dd>

Type: **[**LPTSTR**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)**

A pointer to a buffer that contains the text to draw. If the *cchText* parameter is -1, the string must be null-terminated.

If *dwDTFormat* includes DT\_MODIFYSTRING, the function might add up to four additional characters to this string. The buffer that contains the string should be large enough to accommodate these extra characters.

</dd> <dt>

*cchText* \[in\]
</dt> <dd>

Type: **int**

The length of the string pointed to by *lpchText*. If *cchText* is -1, then the *lpchText* parameter is assumed to be a pointer to a null-terminated string and [**DrawTextEx**](https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-drawtextexa) computes the character count automatically.

</dd> <dt>

*lprc* \[in, out\]
</dt> <dd>

Type: **LPRECT**

A pointer to a [**RECT**](https://docs.microsoft.com/previous-versions//dd162897(v=vs.85)) structure that contains the rectangle, in logical coordinates, in which the text is to be formatted.

</dd> <dt>

*dwDTFormat* \[in\]
</dt> <dd>

Type: **[**UINT**](https://docs.microsoft.com/windows/desktop/WinProg/windows-data-types)**

The formatting options. See the documentation for [**DrawTextEx**](https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-drawtextexa) for a complete list of options.

</dd> <dt>

*lpDTParams* \[in\]
</dt> <dd>

Type: **LPDRAWTEXTPARAMS**

A pointer to a [**DRAWTEXTPARAMS**](https://docs.microsoft.com/windows/win32/api/winuser/ns-winuser-drawtextparams) structure that specifies additional formatting options. This parameter can be **NULL**.

</dd> </dl>

## Return value

Type: **int**

If the function succeeds, the return value is the text height in logical units. If **DT\_VCENTER** or **DT\_BOTTOM** is specified, the return value is the offset from the **top** member of *lprc* to the bottom of the drawn text.

If the function fails, the return value is zero.

To get extended error information, call [**GetLastError**](https://docs.microsoft.com/windows/desktop/api/errhandlingapi/nf-errhandlingapi-getlasterror).

## Remarks

**DrawTextExPrivWrap** is not exported by name or declared in a public header file. To use it, you must use [**GetProcAddress**](https://docs.microsoft.com/windows/desktop/api/libloaderapi/nf-libloaderapi-getprocaddress) and request ordinal 416 from ComCtl32.dll to obtain a function pointer.

For additional remarks, please see [**DrawTextEx**](https://docs.microsoft.com/windows/desktop/api/winuser/nf-winuser-drawtextexa).

## Requirements



|                                     |                                                                                                                |
|-------------------------------------|----------------------------------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows Vista \[desktop apps only\]<br/>                                                                 |
| Minimum supported server<br/> | Windows Server 2003 \[desktop apps only\]<br/>                                                           |
| DLL<br/>                      | <dl> <dt>Comctl32.dll (version 6.0 or later)</dt> </dl> |



 

 





