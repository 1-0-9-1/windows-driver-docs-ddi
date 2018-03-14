---
UID: NF:wiautil.wiauRegGetDwordA
title: wiauRegGetDwordA function
author: windows-driver-content
description: The wiauRegGetDword function gets a DWORD value from the DeviceData section of the registry.
old-location: image\wiaureggetdword.htm
old-project: image
ms.assetid: 936a3a49-ec36-421f-8554-c9ad37907a6d
ms.author: windowsdriverdev
ms.date: 2/27/2018
ms.keywords: image.wiaureggetdword, wiauFncs_a58ebb21-21ce-4815-9dd6-5a1906412a2f.xml, wiauRegGetDword, wiauRegGetDword function [Imaging Devices], wiauRegGetDwordA, wiauRegGetDwordW, wiautil/wiauRegGetDword
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: wiautil.h
req.include-header: Wiautil.h
req.target-type: Desktop
req.target-min-winverclnt: Available in Windows XP and later.
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
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	wiautil.h
api_name:
-	wiauRegGetDword
product: Windows
targetos: Windows
req.typenames: SKIP_AMOUNT
req.product: Windows 10 or later.
---

# wiauRegGetDwordA function


## -description


The <b>wiauRegGetDword</b> function gets a <b>DWORD</b> value from the <b>DeviceData</b> section of the registry.


## -syntax


````
HRESULT _stdcall wiauRegGetDword(
  _In_  HKEY   hkKey,
  _In_  PCTSTR pwszValueName,
  _Out_ DWORD  *pdwValue
);
````


## -parameters




### -param hkKey [in]

Specifies the registry key handle. This parameter should be set to the value pointed to by the <i>phkeyDeviceData </i>parameter when <a href="https://msdn.microsoft.com/library/windows/hardware/ff550179">wiauRegOpenData</a> returns.


### -param pszValueName

TBD


### -param pdwValue [out]

Pointer to a memory location that receives the returned DWORD value.


#### - pwszValueName [in]

Points to the first byte of a Unicode string containing the name of the registry entry.


## -returns



On success, the function returns S_OK. If the function fails, it returns a standard COM error.




## -see-also

<a href="https://msdn.microsoft.com/library/windows/hardware/ff550178">wiauRegGetStr</a>



<a href="https://msdn.microsoft.com/library/windows/hardware/ff550179">wiauRegOpenData</a>



 

 


