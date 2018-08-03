---
UID: NE:portabledevice.tagWPD_STORAGE_TYPE_VALUES
title: tagWPD_STORAGE_TYPE_VALUES
author: windows-driver-content
description: The WPD_STORAGE_TYPE_VALUES enumeration type describes the different Windows Portable Devices storage types.
old-location: wpddk\wpd_storage_type_values.htm
tech.root: wpd_dk
ms.assetid: 709d8ead-5d10-4451-ac3a-09a38ebaa46f
ms.author: windowsdriverdev
ms.date: 2/15/2018
ms.keywords: WPD_STORAGE_TYPE_FIXED_RAM, WPD_STORAGE_TYPE_FIXED_ROM, WPD_STORAGE_TYPE_REMOVABLE_RAM, WPD_STORAGE_TYPE_REMOVABLE_ROM, WPD_STORAGE_TYPE_UNDEFINED, WPD_STORAGE_TYPE_VALUES, WPD_STORAGE_TYPE_VALUES enumeration, portabledevice/WPD_STORAGE_TYPE_FIXED_RAM, portabledevice/WPD_STORAGE_TYPE_FIXED_ROM, portabledevice/WPD_STORAGE_TYPE_REMOVABLE_RAM, portabledevice/WPD_STORAGE_TYPE_REMOVABLE_ROM, portabledevice/WPD_STORAGE_TYPE_UNDEFINED, portabledevice/WPD_STORAGE_TYPE_VALUES, tagWPD_STORAGE_TYPE_VALUES, wpddk.wpd_storage_type_values
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: enum
req.header: portabledevice.h
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
topic_type:
-	APIRef
-	kbSyntax
api_type:
-	HeaderDef
api_location:
-	PortableDevice.h
api_name:
-	WPD_STORAGE_TYPE_VALUES
product: Windows
targetos: Windows
req.typenames: WPD_STORAGE_TYPE_VALUES
---

# tagWPD_STORAGE_TYPE_VALUES enumeration


## -description



The <b>WPD_STORAGE_TYPE_VALUES</b> enumeration type describes the different Windows Portable Devices storage types.




## -enum-fields




### -field WPD_STORAGE_TYPE_UNDEFINED

The storage is of an undefined type.


### -field WPD_STORAGE_TYPE_FIXED_ROM

The storage is non-removable and read-only.


### -field WPD_STORAGE_TYPE_REMOVABLE_ROM

The storage is removable and is read-only.


### -field WPD_STORAGE_TYPE_FIXED_RAM

The storage is non-removable and is read/write capable.


### -field WPD_STORAGE_TYPE_REMOVABLE_RAM

The storage is removable and is read/write capable.


## -remarks



None.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/ff597672">Structures and Enumeration Types</a>
 

 
