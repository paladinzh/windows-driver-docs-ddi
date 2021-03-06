---
UID: NE:d3d10umddi.D3D10_DDI_MAP_FLAG
title: D3D10_DDI_MAP_FLAG
author: windows-driver-content
description: The D3D10_DDI_MAP_FLAG enumeration type contains flags that identify how to map to a subresource in a call to the driver's ResourceMap function.
old-location: display\d3d10_ddi_map_flag.htm
tech.root: display
ms.assetid: e17ca347-6514-47df-9373-5d33fc7f8e5c
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: D3D10_DDI_MAP_FLAG, D3D10_DDI_MAP_FLAG enumeration [Display Devices], D3D10_DDI_MAP_FLAG_DONOTWAIT, D3D10_DDI_MAP_FLAG_MASK, UMDisplayDriver_Dx10param_Structs_ff1e6692-48bb-4381-831a-3d090bbb6f3f.xml, d3d10umddi/D3D10_DDI_MAP_FLAG, d3d10umddi/D3D10_DDI_MAP_FLAG_DONOTWAIT, d3d10umddi/D3D10_DDI_MAP_FLAG_MASK, display.d3d10_ddi_map_flag
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: d3d10umddi.h
req.include-header: D3d10umddi.h
req.target-type: Windows
req.target-min-winverclnt: Available in Windows Vista and later versions of the Windows operating systems.
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
-	d3d10umddi.h
api_name:
-	D3D10_DDI_MAP_FLAG
product:
- Windows
targetos: Windows
req.typenames: D3D10_DDI_MAP_FLAG
---

# D3D10_DDI_MAP_FLAG enumeration


## -description


The D3D10_DDI_MAP_FLAG enumeration type contains flags that identify how to map to a subresource in a call to the driver's <a href="https://msdn.microsoft.com/1310a3f8-02dd-4d35-98ad-4016e57d1eb2">ResourceMap</a> function.


## -enum-fields




### -field D3D10_DDI_MAP_FLAG_DONOTWAIT

The driver can call the <a href="https://msdn.microsoft.com/968b04a7-8869-410c-a6fc-83d57726858f">pfnSetErrorCb</a> function to set the ERR_WASSTILLDRAWING error code if contention exists between an application and hardware when the driver receives the call to <a href="https://msdn.microsoft.com/1310a3f8-02dd-4d35-98ad-4016e57d1eb2">ResourceMap</a>.


### -field D3D10_DDI_MAP_FLAG_MASK

A mask value that indicates the valid bitfields in a bitwise OR combination of the values from this enumeration. 


## -see-also




<a href="https://msdn.microsoft.com/1310a3f8-02dd-4d35-98ad-4016e57d1eb2">ResourceMap</a>



<a href="https://msdn.microsoft.com/968b04a7-8869-410c-a6fc-83d57726858f">pfnSetErrorCb</a>
 

 

