---
UID: NS:usbscan._DEVICE_DESCRIPTOR
title: "_DEVICE_DESCRIPTOR"
author: windows-driver-content
description: The DEVICE_DESCRIPTOR structure is used as a parameter to DeviceIoControl, when the specified I/O control code is IOCTL_GET_DEVICE_DESCRIPTOR.
old-location: image\device_descriptor.htm
old-project: image
ms.assetid: 15ad337a-0b33-48ba-98cf-6aff2698e2ba
ms.author: windowsdriverdev
ms.date: 2/23/2018
ms.keywords: ",  , *, *PDEVICE_DESCRIPTOR, ,, C, D, DEVICE_DESCRIPTOR, DEVICE_DESCRIPTOR structure [Imaging Devices], E, I, O, P, PDEVICE_DESCRIPTOR, PDEVICE_DESCRIPTOR structure pointer [Imaging Devices], R, S, T, V, _, _DEVICE_DESCRIPTOR, image.device_descriptor, stifnc_1b07d50b-5530-47d4-a212-54305a0fef7a.xml, usbscan/DEVICE_DESCRIPTOR, usbscan/PDEVICE_DESCRIPTOR"
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: usbscan.h
req.include-header: Usbscan.h
req.target-type: Windows
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
req.lib: 
req.dll: 
req.irql: 
topictype:
-	APIRef
-	kbSyntax
apitype:
-	HeaderDef
apilocation:
-	usbscan.h
apiname:
-	DEVICE_DESCRIPTOR
product: Windows
targetos: Windows
req.typenames: DEVICE_DESCRIPTOR, *PDEVICE_DESCRIPTOR
req.product: Windows 10 or later.
---

# _DEVICE_DESCRIPTOR structure


## -description


The DEVICE_DESCRIPTOR structure is used as a parameter to <a href="https://msdn.microsoft.com/1d35c087-6672-4fc6-baa1-a886dd9d3878">DeviceIoControl</a>, when the specified I/O control code is <a href="..\usbscan\ni-usbscan-ioctl_get_device_descriptor.md">IOCTL_GET_DEVICE_DESCRIPTOR</a>.


## -syntax


````
typedef struct _DEVICE_DESCRIPTOR {
  USHORT usVendorId;
  USHORT usProductId;
  USHORT usBcdDevice;
  USHORT usLanguageId;
} DEVICE_DESCRIPTOR, *PDEVICE_DESCRIPTOR;
````


## -struct-fields




### -field usVendorId

Vendor identifier.


### -field usProductId

Device product identifier.


### -field usBcdDevice

BCD-encoded device version number.


### -field usLanguageId

<i>Not used</i>.

