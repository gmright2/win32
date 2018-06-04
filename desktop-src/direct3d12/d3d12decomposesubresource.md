---
title: D3D12DecomposeSubresource function
description: Outputs the mip slice, array slice, and plane slice that correspond to the specified subresource index.
ms.assetid: 89FAD7C5-E732-4E74-AC2F-DEECD6ADDA7D
keywords:
- D3D12DecomposeSubresource function
topic_type:
- apiref
api_name:
- D3D12DecomposeSubresource
api_location:
- D3D12.dll
api_type:
- DllExport
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# D3D12DecomposeSubresource function

Outputs the mip slice, array slice, and plane slice that correspond to the specified subresource index.

## Syntax


```C++
void inline D3D12DecomposeSubresource(
        UINT Subresource,
        UINT MipLevels,
        UINT ArraySize,
  _Out_ T    &amp;MipSlice,
  _Out_ U    &amp;ArraySlice,
  _Out_ V    &amp;PlaneSlice
);
```



## Parameters

<dl> <dt>

*Subresource* 
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/library/windows/desktop/aa383751)**

The index of the subresource.

</dd> <dt>

*MipLevels* 
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/library/windows/desktop/aa383751)**

The maximum number of mipmap levels in the subresource.

</dd> <dt>

*ArraySize* 
</dt> <dd>

Type: **[**UINT**](https://msdn.microsoft.com/library/windows/desktop/aa383751)**

The number of elements in the array.

</dd> <dt>

*MipSlice* \[out, ref\]
</dt> <dd>

Type: **T**

Outputs the mip slice that corresponds to the given subresource index.

</dd> <dt>

*ArraySlice* \[out, ref\]
</dt> <dd>

Type: **U**

Outputs the array slice that corresponds to the given subresource index.

</dd> <dt>

*PlaneSlice* \[out, ref\]
</dt> <dd>

Type: **V**

Outputs the plane slice that corresponds to the given subresource index.

</dd> </dl>

## Return value

This method does not return a value.

## Remarks

This function determines which mip slice, array slice, and plane slice correspond to a given subresource index. This is a useful utility, though it is C++ specific.

This function is declared as follows, with C++ templatized parameters for types **T**, **U**, and **V**:


```
template &amp;lt;typename T, typename U, typename V&amp;gt;
inline void D3D12DecomposeSubresource( UINT Subresource, UINT MipLevels, UINT ArraySize, _Out_ T&amp;amp; MipSlice, _Out_ U&amp;amp; ArraySlice, _Out_ V&amp;amp; PlaneSlice )
{
    MipSlice = static_cast&amp;lt;T&amp;gt;(Subresource % MipLevels);
    ArraySlice = static_cast&amp;lt;U&amp;gt;((Subresource / MipLevels) % ArraySize);
    PlaneSlice = static_cast&amp;lt;V&amp;gt;(Subresource / (MipLevels * ArraySize));
}
```



## Requirements



|                    |                                                                                      |
|--------------------|--------------------------------------------------------------------------------------|
| Header<br/>  | <dl> <dt>D3dx12.h</dt> </dl>  |
| Library<br/> | <dl> <dt>D3D12.lib</dt> </dl> |
| DLL<br/>     | <dl> <dt>D3D12.dll</dt> </dl> |



## See also

<dl> <dt>

[Helper Functions for D3D12](helper-functions-for-d3d12.md)
</dt> <dt>

[Subresources](subresources.md)
</dt> </dl>

 

 




