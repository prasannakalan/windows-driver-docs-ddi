---
UID: NE:wdfdevice._WDF_POWER_POLICY_SX_WAKE_USER_CONTROL
title: "_WDF_POWER_POLICY_SX_WAKE_USER_CONTROL"
author: windows-driver-content
description: The WDF_POWER_POLICY_SX_WAKE_USER_CONTROL enumeration identifies whether a user can control a device's ability to wake the system from a low system power state.
old-location: wdf\wdf_power_policy_sx_wake_user_control.htm
old-project: wdf
ms.assetid: d5f4eb5f-28bb-4906-b9f5-3adae31cac80
ms.author: windowsdriverdev
ms.date: 2/26/2018
ms.keywords: DFDeviceObjectGeneralRef_1594c32d-63b6-4280-b5b3-dfcf508a88c6.xml, WDF_POWER_POLICY_SX_WAKE_USER_CONTROL, WDF_POWER_POLICY_SX_WAKE_USER_CONTROL enumeration, WakeAllowUserControl, WakeDoNotAllowUserControl, WakeUserControlInvalid, _WDF_POWER_POLICY_SX_WAKE_USER_CONTROL, kmdf.wdf_power_policy_sx_wake_user_control, wdf.wdf_power_policy_sx_wake_user_control, wdfdevice/WDF_POWER_POLICY_SX_WAKE_USER_CONTROL, wdfdevice/WakeAllowUserControl, wdfdevice/WakeDoNotAllowUserControl, wdfdevice/WakeUserControlInvalid, wudfddi_types/WDF_POWER_POLICY_SX_WAKE_USER_CONTROL, wudfddi_types/WakeAllowUserControl, wudfddi_types/WakeDoNotAllowUserControl, wudfddi_types/WakeUserControlInvalid
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: wdfdevice.h
req.include-header: Wdf.h
req.target-type: Windows
req.target-min-winverclnt: 
req.target-min-winversvr: 
req.kmdf-ver: 1.0
req.umdf-ver: 1.11
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
-	wdfdevice.h
-	wudfddi_types.h
api_name:
-	WDF_POWER_POLICY_SX_WAKE_USER_CONTROL
product:
- Windows
targetos: Windows
req.typenames: WDF_POWER_POLICY_SX_WAKE_USER_CONTROL
---

# _WDF_POWER_POLICY_SX_WAKE_USER_CONTROL enumeration


## -description


<p class="CCE_Message">[Applies to KMDF and UMDF]

The <b>WDF_POWER_POLICY_SX_WAKE_USER_CONTROL</b> enumeration identifies whether a user can control a device's ability to wake the system from a low system power state.


## -enum-fields




### -field WakeUserControlInvalid

For internal use only.


### -field WakeDoNotAllowUserControl

Users cannot control the device's ability to wake the system from a low system power state.


### -field WakeAllowUserControl

Users can control the device's ability to wake the system from a low system power state.


## -remarks



The <b>WDF_POWER_POLICY_SX_WAKE_USER_CONTROL</b> enumeration is used as a member type in the <a href="https://msdn.microsoft.com/library/windows/hardware/ff551277">WDF_DEVICE_POWER_POLICY_WAKE_SETTINGS</a> structure.

To control a device's ability to wake the system from a low system power state, users modify information on a <a href="https://docs.microsoft.com/en-us/windows-hardware/drivers/wdf/user-control-of-device-idle-and-wake-behavior">property sheet</a>. The framework creates the property sheet and Device Manager displays it.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff551277">WDF_DEVICE_POWER_POLICY_WAKE_SETTINGS</a>
 

 

