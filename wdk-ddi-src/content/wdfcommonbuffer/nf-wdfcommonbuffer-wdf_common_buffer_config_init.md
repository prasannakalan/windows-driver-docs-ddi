---
UID: NF:wdfcommonbuffer.WDF_COMMON_BUFFER_CONFIG_INIT
title: WDF_COMMON_BUFFER_CONFIG_INIT function
author: windows-driver-content
description: The WDF_COMMON_BUFFER_CONFIG_INIT function initializes a WDF_COMMON_BUFFER_CONFIG structure.
old-location: wdf\wdf_common_buffer_config_init.htm
old-project: wdf
ms.assetid: a678516a-159f-42bc-b135-489677452472
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: DFCommonBufferObjectRef_23c5b41e-89ce-448c-86fa-3ae4e688b378.xml, WDF_COMMON_BUFFER_CONFIG_INIT, WDF_COMMON_BUFFER_CONFIG_INIT function, kmdf.wdf_common_buffer_config_init, wdf.wdf_common_buffer_config_init, wdfcommonbuffer/WDF_COMMON_BUFFER_CONFIG_INIT
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: wdfcommonbuffer.h
req.include-header: WdfCommonBuffer.h
req.target-type: Universal
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 1.0
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: 
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	wdfcommonbuffer.h
api_name:
-	WDF_COMMON_BUFFER_CONFIG_INIT
product:
- Windows
targetos: Windows
req.typenames: 
---

# WDF_COMMON_BUFFER_CONFIG_INIT function


## -description


<p class="CCE_Message">[Applies to KMDF only]

The <b>WDF_COMMON_BUFFER_CONFIG_INIT</b> function initializes a <a href="https://msdn.microsoft.com/library/windows/hardware/ff551244">WDF_COMMON_BUFFER_CONFIG</a> structure.


## -parameters




### -param Config [out]

A pointer to a <a href="https://msdn.microsoft.com/library/windows/hardware/ff551244">WDF_COMMON_BUFFER_CONFIG</a> structure.


### -param AlignmentRequirement [in]

A value for the <b>AlignmentRequirement</b> member of the <a href="https://msdn.microsoft.com/library/windows/hardware/ff551244">WDF_COMMON_BUFFER_CONFIG</a> structure. This value specifies the alignment requirement for the common buffer that the structure describes.


## -returns



None




## -remarks



The <b>WDF_COMMON_BUFFER_CONFIG_INIT</b> function zeros the specified <a href="https://msdn.microsoft.com/library/windows/hardware/ff551244">WDF_COMMON_BUFFER_CONFIG</a> structure and sets the structure's <b>AlignmentRequirement</b> member to the specified value.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff551244">WDF_COMMON_BUFFER_CONFIG</a>
 

 

