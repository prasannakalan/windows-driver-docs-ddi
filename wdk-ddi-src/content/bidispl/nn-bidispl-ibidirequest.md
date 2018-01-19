---
UID : NN:bidispl.IBidiRequest
title : IBidiRequest
author : windows-driver-content
description : The IBidiRequest interface allows an application or other objects to compose a bidi request.
old-location : print\ibidirequest.htm
old-project : print
ms.assetid : e7b16853-7f1d-45e4-af5e-4ae9cbb9b191
ms.author : windowsdriverdev
ms.date : 1/8/2018
ms.keywords : IBidiSpl2, IBidiSpl2::UnbindDevice, UnbindDevice
ms.prod : windows-hardware
ms.technology : windows-devices
ms.topic : interface
req.header : bidispl.h
req.include-header : 
req.target-type : Windows
req.target-min-winverclnt : Windows XP
req.target-min-winversvr : Windows Server 2003
req.kmdf-ver : 
req.umdf-ver : 
req.alt-api : IBidiRequest
req.alt-loc : Bidispl.h
req.ddi-compliance : 
req.unicode-ansi : 
req.idl : 
req.max-support : 
req.namespace : 
req.assembly : 
req.type-library : 
req.lib : 
req.dll : Bidispl.dll
req.irql : 
req.typenames : MPEG2_TRANSPORT_STRIDE, *PMPEG2_TRANSPORT_STRIDE
---

# IBidiRequest interface

The <b>IBidiRequest</b> interface allows an application or other objects to compose a bidi request.

## Methods

<p>The <b>IBidiRequest</b> interface has these methods.</p>

| Method | Description |
| ---- |:---- |
| [bidispl.IBidiRequest.GetEnumCount](nf-bidispl-ibidirequest-getenumcount.md) | The IBidiRequest::GetEnumCount method gets the number of output results from the bidi request. |
| [bidispl.IBidiRequest.GetOutputData](nf-bidispl-ibidirequest-getoutputdata.md) | The IBidiRequest::GetOutputData method gets the specified output data coming back from the printer. |
| [bidispl.IBidiRequest.GetResult](nf-bidispl-ibidirequest-getresult.md) | The IBidiRequest::GetResult method tells whether the bidi request was successful. |
| [bidispl.IBidiRequest.SetInputData](nf-bidispl-ibidirequest-setinputdata.md) | The IBidiRequest::SetInputData method sets the data to send to the printer. |
| [bidispl.IBidiRequest.SetSchema](nf-bidispl-ibidirequest-setschema.md) | The IBidiRequest::SetSchema method sets the bidi schema string. |

## Remarks



## Requirements
| &nbsp; | &nbsp; |
| ---- |:---- |
| **Windows Driver kit version** |  |
| **Target platform** | Windows |
| **Minimum UMDF version** |  |
| **Header** | bidispl.h |
| **DLL** | Bidispl.dll |

    ## See Also

        <dl>
<dt>
<a href="https://msdn.microsoft.com/library/windows/hardware/ff545163">Bidirectional Communication Interfaces</a>
</dt>
<dt>
<a href="https://msdn.microsoft.com/b15b1aff-623e-4159-ab0f-ce386a1377eb">Bidirectional Communication Schema</a>
</dt>
<dt>
<a href="https://msdn.microsoft.com/42b5e6cf-b434-4734-86f3-b3b9d15ea468">Print Spooler Components</a>
</dt>
</dl>
 

 

<a href="mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback [print\print]:%20IBidiRequest interface%20 RELEASE:%20(1/8/2018)&amp;body=%0A%0APRIVACY STATEMENT%0A%0AWe use your feedback to improve the documentation. We don't use your email address for any other purpose, and we'll remove your email address from our system after the issue that you're reporting is fixed. While we're working to fix this issue, we might send you an email message to ask for more info. Later, we might also send you an email message to let you know that we've addressed your feedback.%0A%0AFor more info about Microsoft's privacy policy, see http://privacy.microsoft.com/en-us/default.aspx." title="Send comments about this topic to Microsoft">Send comments about this topic to Microsoft</a>