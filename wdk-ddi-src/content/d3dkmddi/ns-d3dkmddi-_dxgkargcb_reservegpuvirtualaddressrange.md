---
UID: NS:d3dkmddi._DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE
title: "_DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE"
author: windows-driver-content
description: DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE is used with the DxgkCbReserveGpuVirtualAddressRangedevice driver interface (DDI) to allow the kernel mode driver to reserve a graphics processing unit (GPU) virtual address range during creation of a process.
old-location: display\dxgkargcb_reservegpuvirtualaddressrange.htm
tech.root: display
ms.assetid: D555E595-4319-4FCC-84A7-52FA3F278FFD
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: "*INOUT_PDXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE, DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE, DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE structure [Display Devices], _DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE, d3dkmddi/DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE, display.dxgkargcb_reservegpuvirtualaddressrange"
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
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	d3dkmddi.h
api_name:
-	DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE
product:
- Windows
targetos: Windows
req.typenames: DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE
---

# _DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE structure


## -description


<b>DXGKARGCB_RESERVEGPUVIRTUALADDRESSRANGE</b> is used with the <a href="https://msdn.microsoft.com/26A827F1-1094-4A7D-9C63-758925EE6273">DxgkCbReserveGpuVirtualAddressRange</a>device driver interface (DDI) to allow the kernel mode driver to reserve a graphics processing unit (GPU) virtual address range during creation of a process. 


## -struct-fields




### -field hDxgkProcess

The handle that was passed to <a href="https://msdn.microsoft.com/E5AAEEB1-C29E-4AA7-9F8E-2C2DCFADED81">DxgkDdiCreateProcess</a>.


### -field SizeInBytes

The size of the address range in bytes, this must be set to an integral multiple of the address space covered by a single page table entry.


### -field Alignment

The number of bytes to align the start address to. Must be a multiple of the address space covered by a single page table entry and a power of 2.


### -field StartVirtualAddress

The starting location of the reserved address range.


### -field BaseAddress

The base virtual address of the virtual address range in bytes. It must be aligned to the size of the address space, covered by a single page table entry.


### -field AllowUserModeMapping

Allow the user mode driver to map allocations to the range.


### -field Flags

A single value containing the flags set in the structure.


## -see-also




<a href="https://msdn.microsoft.com/26A827F1-1094-4A7D-9C63-758925EE6273">DxgkCbReserveGpuVirtualAddressRange</a>



<a href="https://msdn.microsoft.com/E5AAEEB1-C29E-4AA7-9F8E-2C2DCFADED81">DxgkDdiCreateProcess</a>
 

 

