---
UID : NN:bidispl.IBidiRequestContainer
title : IBidiRequestContainer
author : windows-driver-content
description : The IBidiRequestContainer interface allows an application or other objects to compose and retrieve a list of bidi requests.
old-location : print\ibidirequestcontainer.htm
old-project : print
ms.assetid : 21dfcbe8-2fc1-4495-af54-5d4c83b8bb79
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
req.alt-api : IBidiRequestContainer
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

# IBidiRequestContainer interface

The <b>IBidiRequestContainer</b> interface allows an application or other objects to compose and retrieve a list of bidi requests.

## Methods

<p>The <b>IBidiRequestContainer</b> interface has these methods.</p>

| Method | Description |
| ---- |:---- |
| [bidispl.IBidiRequestContainer.AddRequest](nf-bidispl-ibidirequestcontainer-addrequest.md) | The IBidiRequestContainer::AddRequest method adds a request to the request list. |
| [bidispl.IBidiRequestContainer.GetEnumObject](nf-bidispl-ibidirequestcontainer-getenumobject.md) | The IBidiRequestContainer::GetEnumObject method enumerates the bidi requests in a list. |
| [bidispl.IBidiRequestContainer.GetRequestCount](nf-bidispl-ibidirequestcontainer-getrequestcount.md) | The IBidiRequestContainer::GetRequestCount method gets the number of requests in the request list. |

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
 

 

<a href="mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback [print\print]:%20IBidiRequestContainer interface%20 RELEASE:%20(1/8/2018)&amp;body=%0A%0APRIVACY STATEMENT%0A%0AWe use your feedback to improve the documentation. We don't use your email address for any other purpose, and we'll remove your email address from our system after the issue that you're reporting is fixed. While we're working to fix this issue, we might send you an email message to ask for more info. Later, we might also send you an email message to let you know that we've addressed your feedback.%0A%0AFor more info about Microsoft's privacy policy, see http://privacy.microsoft.com/en-us/default.aspx." title="Send comments about this topic to Microsoft">Send comments about this topic to Microsoft</a>