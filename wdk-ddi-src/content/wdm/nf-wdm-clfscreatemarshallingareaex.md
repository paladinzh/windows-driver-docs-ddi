---
UID: NF:wdm.ClfsCreateMarshallingAreaEx
title: ClfsCreateMarshallingAreaEx function
author: windows-driver-content
description: Initalizes a marshalling area for a physical or client log file stream.
ms.assetid: 00a9624d-0cc9-4429-8050-74934176bbdd
ms.author: windowsdriverdev
ms.date: 
ms.topic: function
ms.keywords: ClfsCreateMarshallingAreaEx
req.header: wdm.h
req.include-header:
req.target-type:
req.target-min-winverclnt: Windows 10, version 1803
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib: NtosKrnl.lib
req.dll: NtosKrnl.exe
req.irql: 
req.ddi-compliance:
req.unicode-ansi:
req.idl:
req.max-support:
req.namespace:
req.assembly:
req.type-library: 
topictype: 
-	apiref
apitype: 
-	DllExport
apilocation: 
-	NtosKrnl.exe
apiname: 
-	ClfsCreateMarshallingAreaEx
product:
-	Windows
targetos: Windows

---

# ClfsCreateMarshallingAreaEx function


## -description

Initalizes a marshalling area for a physical or client log file stream.

## -parameters

### -param plfoLog
The handle associated with new marshalling area.

### -param ePoolType
Paged or non-paged pool buffers.

### -param pfnAllocBuffer
Optional. A pointer to the block allocation callback function.

### -param pfnFreeBuffer
Optional. A pointer to the block deallocation callback function.

### -param cbMarshallingBuffer
The size of marshalling buffers.

### -param cMaxWriteBuffers
The maximum number of allocated write buffers.

### -param cMaxReadBuffers
The maximum number of allocated read buffers.

### -param cAlignmentSize
The alignment size of mashalling buffers.

### -param fFlags
buffer management flag

### -param ppvMarshalContext
marshalling context

## -returns
This function returns CLFSUSER_API NTSTATUS.
## -remarks

## -see-also