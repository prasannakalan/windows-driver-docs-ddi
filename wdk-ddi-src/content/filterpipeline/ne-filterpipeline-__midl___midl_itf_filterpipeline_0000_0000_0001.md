---
UID : NE:filterpipeline.__MIDL___MIDL_itf_filterpipeline_0000_0000_0001
title : __MIDL___MIDL_itf_filterpipeline_0000_0000_0001
author : windows-driver-content
description : The ExpsCompressionOptions enumeration describes compression options for an XPS part.
old-location : print\expscompressionoptions.htm
old-project : print
ms.assetid : 7df53803-4e01-4d00-b7a4-2f2d1dde5ad8
ms.author : windowsdriverdev
ms.date : 1/8/2018
ms.keywords : __MIDL___MIDL_itf_filterpipeline_0000_0000_0001, EXpsCompressionOptions
ms.prod : windows-hardware
ms.technology : windows-devices
ms.topic : enum
req.header : filterpipeline.h
req.include-header : Filterpipeline.h
req.target-type : Windows
req.target-min-winverclnt : 
req.target-min-winversvr : 
req.kmdf-ver : 
req.umdf-ver : 
req.alt-api : EXpsCompressionOptions
req.alt-loc : filterpipeline.h
req.ddi-compliance : 
req.unicode-ansi : 
req.idl : Filterpipeline.idl
req.max-support : 
req.namespace : 
req.assembly : 
req.type-library : 
req.lib : 
req.dll : 
req.irql : <= APC_LEVEL
req.typenames : EXpsCompressionOptions
---

# __MIDL___MIDL_itf_filterpipeline_0000_0000_0001 Enumeration
The ExpsCompressionOptions enumeration describes compression options for an XPS part.

## Syntax
````
typedef enum  { 
  Compression_NotCompressed,
  Compression_Normal,
  Compression_Small,
  Compression_Fast
} EXpsCompressionOptions;
````

## Constants

<table>

<tr>
<td>Compression_Fast</td>
<td>The compression for the part is optimized for speed.</td>
</tr>

<tr>
<td>Compression_Normal</td>
<td>The part is compressed normally.</td>
</tr>

<tr>
<td>Compression_NotCompressed</td>
<td>The part is not compressed.</td>
</tr>

<tr>
<td>Compression_Small</td>
<td>The compression for the part is optimized for size.</td>
</tr>
</table>


## Requirements
| &nbsp; | &nbsp; |
| ---- |:---- |
| **Windows Driver kit version** |  |
| **Minimum KMDF version** |  |
| **Minimum UMDF version** |  |
| **Header** | filterpipeline.h (include Filterpipeline.h) |