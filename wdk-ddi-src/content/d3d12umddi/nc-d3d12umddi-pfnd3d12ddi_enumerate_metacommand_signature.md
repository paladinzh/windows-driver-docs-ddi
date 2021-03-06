---
UID: NC:d3d12umddi.PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE
title: PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE
author: windows-driver-content
description:
ms.assetid: 9ab6bbb3-6641-4576-b86d-f90dd2975cb0
ms.author: windowsdriverdev
ms.date:
ms.topic: callback
ms.prod: windows-hardware
ms.technology: windows-devices
req.header: d3d12umddi.h
req.include-header:
req.target-type:
req.target-min-winverclnt:
req.target-min-winversvr:
req.kmdf-ver:
req.umdf-ver:
req.lib:
req.dll:
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
-	UserDefined
apilocation:
-	d3d12umddi.h
apiname:
-	PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE
product: 
- Windows
targetos: Windows
---

# PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE callback function

## -description

Implemented by the client driver to enumerate meta-command signatures.

## -prototype

```
//Declaration

PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE Pfnd3d12ddiEnumerateMetacommandSignature;

// Definition

HRESULT Pfnd3d12ddiEnumerateMetacommandSignature
(
	 D3D12DDI_HDEVICE
	GUID CommandId
	UINT SignatureId
	UINT *pParameterCount
	D3D12DDIARG_METACOMMAND_PARAMETER_DESC *pParameterDescs
)
{...}

PFND3D12DDI_ENUMERATE_METACOMMAND_SIGNATURE


```

## -parameters

### -param D3D12DDI_HDEVICE

A handle to the display device (graphics context).

### -param CommandId

The command identifier.

### -param SignatureId

The command signature id.

### -param *pParameterCount

The count of meta-commands.

### -param *pParameterDescs:

The description of meta-commands.

## -returns

Returns STATUS_SUCCESS if completed successfully.
