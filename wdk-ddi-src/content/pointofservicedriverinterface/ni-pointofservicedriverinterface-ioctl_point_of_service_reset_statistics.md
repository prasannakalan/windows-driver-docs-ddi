---
UID : NI:pointofservicedriverinterface.IOCTL_POINT_OF_SERVICE_RESET_STATISTICS
title : IOCTL_POINT_OF_SERVICE_RESET_STATISTICS
author : windows-driver-content
description : This I/O control function resets the specified statistic's value to zero.
old-location : pos\ioctl_point_of_service_reset_statistics.htm
old-project : pos
ms.assetid : dfa6a460-ea80-4aa4-9948-2fd290f6616b
ms.author : windowsdriverdev
ms.date : 1/10/2018
ms.keywords : _PosPropertyId, PosPropertyId
ms.prod : windows-hardware
ms.technology : windows-devices
ms.topic : ioctl
req.header : pointofservicedriverinterface.h
req.include-header : Pointofservicedriverinterface.h
req.target-type : Windows
req.target-min-winverclnt : 
req.target-min-winversvr : 
req.kmdf-ver : 
req.umdf-ver : 
req.alt-api : IOCTL_POINT_OF_SERVICE_RESET_STATISTICS
req.alt-loc : pointofservicedriverinterface.h
req.ddi-compliance : 
req.unicode-ansi : 
req.idl : 
req.max-support : 
req.namespace : 
req.assembly : 
req.type-library : 
req.lib : 
req.dll : 
req.irql : 
req.typenames : PosPropertyId
---

# IOCTL_POINT_OF_SERVICE_RESET_STATISTICS IOCTL
This I/O control function resets the specified statistic's value to zero.

### Major Code
[IRP_MJ_DEVICE_CONTROL](xref:"https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/irp-mj-device-control")

### Input Buffer
<a href="..\pointofservicedriverinterface\ns-pointofservicedriverinterface-_posstringtype.md">PosStringType</a> that names the statistic to reset to zero.

### Input Buffer Length
Size of the string passed in <i>lpInBuffer</i>. Set to sizeof(<i>PosStringType</i>) + the size of the string in bytes.

### Output Buffer
Not used with this operation; set to <b>NULL</b>.

### Output Buffer Length
Not used with this operation; set to <b>0</b> (zero).

### Input / Output Buffer
<text></text>

### Input / Output Buffer Length
<text></text>

### Status Block
I/O Status block
Returns <b>TRUE</b> if successful; otherwise, returns <b>FALSE</b>.

To get extended error information, call <a href="http://go.microsoft.com/fwlink/p/?LinkId=316871">GetLastError</a>. The following list shows common error values: 



Statistic updating or reporting is not supported.


## Requirements
| &nbsp; | &nbsp; |
| ---- |:---- |
| **Windows Driver kit version** |  |
| **Header** | pointofservicedriverinterface.h (include Pointofservicedriverinterface.h) |
| **IRQL** |  |