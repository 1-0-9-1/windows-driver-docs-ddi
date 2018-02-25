---
UID: NI:usbioctl.IOCTL_INTERNAL_USB_RECORD_FAILURE
title: IOCTL_INTERNAL_USB_RECORD_FAILURE
author: windows-driver-content
description: The IOCTL_INTERNAL_USB_RECORD_FAILURE IOCTL is used by the USB hub driver. Do not use.
old-location: buses\ioctl_internal_usb_record_failure.htm
old-project: UsbRef
ms.assetid: b0b2f80c-38d3-47c7-b57b-d49fb5b6edd7
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: IOCTL_INTERNAL_USB_RECORD_FAILURE, IOCTL_INTERNAL_USB_RECORD_FAILURE control code [Buses], buses.ioctl_internal_usb_record_failure, usbioctl/IOCTL_INTERNAL_USB_RECORD_FAILURE
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: usbioctl.h
req.include-header: 
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
-	Usbioctl.h
apiname:
-	IOCTL_INTERNAL_USB_RECORD_FAILURE
product: Windows
targetos: Windows
req.typenames: USB_HUB_TYPE
req.product: Windows 10 or later.
---

# IOCTL_INTERNAL_USB_RECORD_FAILURE IOCTL


##  Major Code: 


[IRP_MJ_DEVICE_CONTROL](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/irp-mj-device-control)

## -description


 The <b>IOCTL_INTERNAL_USB_RECORD_FAILURE</b> IOCTL is used by the USB hub driver. Do not use.


## -ioctlparameters




### -input-buffer



<text></text>




### -input-buffer-length



<text></text>




### -output-buffer



<text></text>




### -output-buffer-length



<text></text>




### -in-out-buffer



<text></text>




### -inout-buffer-length



<text></text>




### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [XREF-LINK:NTSTATUS Values].



