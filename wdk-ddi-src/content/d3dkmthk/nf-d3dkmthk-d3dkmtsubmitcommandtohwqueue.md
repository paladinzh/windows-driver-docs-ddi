---
UID: NF:d3dkmthk.D3DKMTSubmitCommandToHwQueue
title: D3DKMTSubmitCommandToHwQueue function
author: windows-driver-content
description: Used to submit a command to the hardware queue.
old-location: display\d3dkmtsubmitcommandtohwqueue.htm
tech.root: display
ms.assetid: E4E6B637-BFAF-4ACD-86C2-109704B8D33D
ms.author: windowsdriverdev
ms.date: 5/10/2018
ms.keywords: D3DKMTSubmitCommandToHwQueue, D3DKMTSubmitCommandToHwQueue function [Display Devices], d3dkmthk/D3DKMTSubmitCommandToHwQueue, display.d3dkmtsubmitcommandtohwqueue
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: function
req.header: d3dkmthk.h
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
req.lib: Gdi32.lib 
req.dll: Gdi32.dll 
req.irql: 
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	DllExport
api_location:
-	Gdi32.dll
api_name:
-	D3DKMTSubmitCommandToHwQueue
product:
- Windows
targetos: Windows
req.typenames: 
---

# D3DKMTSubmitCommandToHwQueue function


## -description


Used to submit a command to the hardware queue.


## -parameters




### -param D3DKMT_SUBMITCOMMANDTOHWQUEUE






#### - submitCommandToHwQueue [in]

A structure holding the information needed to submit a command to the hardware queue.


## -returns



Returns STATUS_SUCCESS if called successfully. 



