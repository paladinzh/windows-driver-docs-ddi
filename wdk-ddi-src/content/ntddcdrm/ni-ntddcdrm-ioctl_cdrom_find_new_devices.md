---
UID: NI:ntddcdrm.IOCTL_CDROM_FIND_NEW_DEVICES
title: IOCTL_CDROM_FIND_NEW_DEVICES
author: windows-driver-content
description: In Microsoft Windows 2000 and later operating systems, this IOCTL is replaced by IOCTL_STORAGE_FIND_NEW_DEVICES. The only difference between the two IOCTLs is the base value.
old-location: storage\ioctl_cdrom_find_new_devices.htm
tech.root: storage
ms.assetid: edaf2b57-ca1a-478f-85b9-2a1e86df98ed
ms.author: windowsdriverdev
ms.date: 3/29/2018
ms.keywords: IOCTL_CDROM_FIND_NEW_DEVICES, IOCTL_CDROM_FIND_NEW_DEVICES control, IOCTL_CDROM_FIND_NEW_DEVICES control code [Storage Devices], k307_80deb95c-40d4-4e22-969e-da0df49599a4.xml, ntddcdrm/IOCTL_CDROM_FIND_NEW_DEVICES, storage.ioctl_cdrom_find_new_devices
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: ntddcdrm.h
req.include-header: TBD
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
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	ntddcdrm.h
api_name:
-	IOCTL_CDROM_FIND_NEW_DEVICES
product:
- Windows
targetos: Windows
req.typenames: 
---

# IOCTL_CDROM_FIND_NEW_DEVICES IOCTL


## -description


In Microsoft Windows 2000 and later operating systems, this IOCTL is replaced by <a href="https://msdn.microsoft.com/library/windows/hardware/ff560546">IOCTL_STORAGE_FIND_NEW_DEVICES</a>. The only difference between the two IOCTLs is the base value.


## -ioctlparameters




### -input-buffer








### -input-buffer-length








### -output-buffer








### -output-buffer-length








### -in-out-buffer








### -inout-buffer-length








### -status-block



Irp->IoStatus.Status is set to STATUS_SUCCESS if the request is successful.

Otherwise, Status to the appropriate error condition as a NTSTATUS code. 

For more information, see [NTSTATUS Values](https://docs.microsoft.com/en-us/windows-hardware/drivers/kernel/ntstatus-values).



