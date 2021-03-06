---
UID: NS:d3dkmddi._DXGK_CREATEPROCESSFLAGS
title: "_DXGK_CREATEPROCESSFLAGS"
author: windows-driver-content
description: DXGK_CREATEPROCESSFLAGS is used with DXGKARG_CREATEPROCESS and DxgkDdiCreateProcess to create a kernel mode driver object for a Microsoft DirectX graphics kernel process object.
old-location: display\dxgk_createprocessflags.htm
tech.root: display
ms.assetid: 43B8202C-6AC1-4596-BA85-FEB9FB0B5746
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: DXGK_CREATEPROCESSFLAGS, DXGK_CREATEPROCESSFLAGS structure [Display Devices], _DXGK_CREATEPROCESSFLAGS, d3dkmddi/DXGK_CREATEPROCESSFLAGS, display.dxgk_createprocessflags
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: struct
req.header: d3dkmddi.h
req.include-header: D3dkmddi.h
req.target-type: Windows
req.target-min-winverclnt: Windows 10
req.target-min-winversvr: Windows Server 2016
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
req.irql: PASSIVE_LEVEL
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	d3dkmddi.h
api_name:
-	DXGK_CREATEPROCESSFLAGS
product:
- Windows
targetos: Windows
req.typenames: DXGK_CREATEPROCESSFLAGS
---

# _DXGK_CREATEPROCESSFLAGS structure


## -description


<b>DXGK_CREATEPROCESSFLAGS</b> is used with <a href="https://msdn.microsoft.com/library/windows/hardware/dn914470">DXGKARG_CREATEPROCESS</a> and <a href="https://msdn.microsoft.com/E5AAEEB1-C29E-4AA7-9F8E-2C2DCFADED81">DxgkDdiCreateProcess</a> to create a kernel mode driver object for a Microsoft DirectX graphics kernel process object.


## -struct-fields




### -field SystemProcess

Indicates that a system process is being created.


### -field GdiProcess

Indicates that a GDI process is being created.


### -field VirtualMachineProcess

The virtual machine DXG process created during a call to DxgkDdiCreateProcess. Note that each virtual machine DXG process will belong to the same EPROCESS as the same virtual machine worker process.

### -field VirtualMachineWorkerProcess

The virtual machine worker process created during a call to DxgkDdiCreateProcess. Note that because no rendering or driver resource is created in this process context, the driver might skip allocating certain resources.

### -field Reserved

This member is reserved and should be set to zero.


### -field Value

The consolidated value of the bitfield members of the structure.


## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/dn914470">DXGKARG_CREATEPROCESS</a>



<a href="https://msdn.microsoft.com/E5AAEEB1-C29E-4AA7-9F8E-2C2DCFADED81">DxgkDdiCreateProcess</a>
 

 

