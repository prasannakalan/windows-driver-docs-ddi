---
UID: NF:ndischimney.NdisTerminateOffload
title: NdisTerminateOffload function
author: windows-driver-content
description: A protocol driver or intermediate driver calls the NdisTerminateOffload function to terminate the offload of one or more state objects
old-location: netvista\ndisterminateoffload.htm
old-project: netvista
ms.assetid: 13eb4c17-2cb5-4773-b2e3-e8e624473c97
ms.author: windowsdriverdev
ms.date: 4/25/2018
ms.keywords: NdisTerminateOffload, NdisTerminateOffload function [Network Drivers Starting with Windows Vista], ndischimney/NdisTerminateOffload, netvista.ndisterminateoffload, tcp_chim_ndis_func_44201f08-cbfc-4796-b2a9-78bbc5c348c4.xml
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: ndischimney.h
req.include-header: Ndischimney.h
req.target-type: Universal
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: 
req.max-support: 
req.namespace: 
req.assembly: 
req.type-library: 
req.lib: Ndis.lib
req.dll: 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	LibDef
api_location:
-	ndis.lib
-	ndis.dll
api_name:
-	NdisTerminateOffload
product:
- Windows
targetos: Windows
req.typenames: 
---

# NdisTerminateOffload function


## -description


<p class="CCE_Message">[The TCP chimney offload feature is deprecated and should not be used.]

A protocol driver or intermediate driver calls the 
  <b>NdisTerminateOffload</b> function to terminate the offload of one or more state objects


## -parameters




### -param NdisBindingHandle [in]

The handle that NDIS provided at the 
     <i>NdisBindingHandle</i> parameter of 
     <a href="https://msdn.microsoft.com/library/windows/hardware/ff563715">NdisOpenAdapterEx</a>. This handle
     identifies the binding between the caller and the underlying intermediate driver or offload
     target.


### -param OffloadBlockList [in, out]

A pointer to an 
     <a href="https://msdn.microsoft.com/64febd55-1ab8-4e2e-b738-340167866333">
     NDIS_PROTOCOL_OFFLOAD_BLOCK_LIST</a> structure that can be a stand-alone structure or the root of a
     linked list of such structures. These structures identify the offloaded state objects that are being
     terminated.


## -returns



None




## -remarks



An intermediate driver calls the 
    <b>NdisTerminateOffload</b> function to propagate a terminate offload operation that was initiated by the
    host stack. For more information, see 
    <a href="https://msdn.microsoft.com/en-us/library/windows/hardware/ff563771">Propagating
    State-Manipulation Operations</a>.

From the 
    <a href="https://msdn.microsoft.com/ebc98e65-5d11-4c3d-aea1-dfad1434c093">
    NDIS_MINIPORT_OFFLOAD_BLOCK_LIST</a> structure that was passed to its 
    <i>MiniportTerminateOffload</i> function, the intermediate driver constructs an
    NDIS_PROTOCOL_OFFLOAD_BLOCK_LIST structure. For more information, see 
    <a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/network/reusing-an-ndis-miniport-offload-block-list-structure">Reusing an
    NDIS_MINIPORT_OFFLOAD_BLOCK_LIST Structure</a>. The intermediate driver passes a pointer (the 
    <i>OffloadBlockList</i> parameter) to this NDIS_PROTOCOL_OFFLOAD_BLOCK_LIST structure when calling the 
    <b>NdisTerminateOffload</b> function.




## -see-also




<a href="https://msdn.microsoft.com/1b808e3c-2d64-44c9-88d3-0a0311e1dc99">MiniportTerminateOffload</a>



<a href="https://msdn.microsoft.com/ebc98e65-5d11-4c3d-aea1-dfad1434c093">
   NDIS_MINIPORT_OFFLOAD_BLOCK_LIST</a>



<a href="https://msdn.microsoft.com/64febd55-1ab8-4e2e-b738-340167866333">
   NDIS_PROTOCOL_OFFLOAD_BLOCK_LIST</a>



<a href="https://msdn.microsoft.com/d444eae5-2e7c-41f2-9fb2-55e172505cf6">
   NdisMTerminateOffloadComplete</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff563715">NdisOpenAdapterEx</a>



<a href="https://msdn.microsoft.com/614d36e8-38ac-49a7-8711-7a6c6646309c">
   ProtocolTerminateOffloadComplete</a>
 

 

