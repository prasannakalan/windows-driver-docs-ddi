---
UID : NN:printerextension.IPrinterQueueView
title : IPrinterQueueView
author : windows-driver-content
description : Provides a way to change the range of print jobs being monitored.
old-location : print\iprinterqueueview.htm
old-project : print
ms.assetid : 81B3D4A3-7176-4656-B23D-04F0F84D9000
ms.author : windowsdriverdev
ms.date : 1/8/2018
ms.keywords : IPrintSchemaTicket2, IPrintSchemaTicket2::GetParameterInitializer, GetParameterInitializer
ms.prod : windows-hardware
ms.technology : windows-devices
ms.topic : interface
req.header : printerextension.h
req.include-header : 
req.target-type : Windows
req.target-min-winverclnt : Windows 8.1
req.target-min-winversvr : Windows Server 2012 R2
req.kmdf-ver : 
req.umdf-ver : 
req.alt-api : IPrinterQueueView
req.alt-loc : Printerextension.h
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
req.typenames : PrintSchemaSelectionType
req.product : Windows 10 or later.
---

# IPrinterQueueView interface

Provides a way to change the range of print jobs being monitored.

## Methods

<p>The <b>IPrinterQueueView</b> interface has these methods.</p>

| Method | Description |
| ---- |:---- |
| [printerextension.IPrinterQueueView.SetViewRange](nf-printerextension-iprinterqueueview-setviewrange.md) | Sets the range of print jobs being monitored. |

## Remarks

An event is raised whenever the status of the print queue changes. So when a client uses <a href="https://msdn.microsoft.com/library/windows/hardware/dn265395">SetViewRange</a> to specify the range of print jobs (the view) to be monitored, the <a href="https://msdn.microsoft.com/D964A0C4-041A-47BD-87AB-4AF523939DF0">IPrinterQueueViewEvent::OnChanged</a> event method fires, and the live queue is returned in response.

And also, note that job enumeration starts when the first event handler is added and stops when the last event handler is removed.

<b>IPrinterQueueView</b> also helps to make it possible to perform job management from a UWP  device app or from a printer extension. For more information, see <a href="https://msdn.microsoft.com/D1236DD2-D4AD-4615-9036-7EC75D6CADCE">Job Management</a>.

## Requirements
| &nbsp; | &nbsp; |
| ---- |:---- |
| **Windows Driver kit version** |  |
| **Target platform** | Windows |
| **Minimum UMDF version** |  |
| **Header** | printerextension.h |
| **DLL** |  |

    ## See Also

        <dl>
<dt>
<a href="https://msdn.microsoft.com/D964A0C4-041A-47BD-87AB-4AF523939DF0">IPrinterQueueViewEvent::OnChanged</a>
</dt>
<dt>
<a href="https://msdn.microsoft.com/D1236DD2-D4AD-4615-9036-7EC75D6CADCE">Job Management</a>
</dt>
</dl>
 

 

<a href="mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback [print\print]:%20IPrinterQueueView interface%20 RELEASE:%20(1/8/2018)&amp;body=%0A%0APRIVACY STATEMENT%0A%0AWe use your feedback to improve the documentation. We don't use your email address for any other purpose, and we'll remove your email address from our system after the issue that you're reporting is fixed. While we're working to fix this issue, we might send you an email message to ask for more info. Later, we might also send you an email message to let you know that we've addressed your feedback.%0A%0AFor more info about Microsoft's privacy policy, see http://privacy.microsoft.com/en-us/default.aspx." title="Send comments about this topic to Microsoft">Send comments about this topic to Microsoft</a>