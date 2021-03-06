---
UID: NI:winbio_ioctl.IOCTL_BIOMETRIC_GET_SENSOR_STATUS
title: IOCTL_BIOMETRIC_GET_SENSOR_STATUS
author: windows-driver-content
description: The IOCTL_BIOMETRIC_GET_SENSOR_STATUS IOCTL tells the driver to perform any necessary steps to collect the current operating status of the device. Vendor-supplied WBDI drivers must support this IOCTL.
old-location: biometric\ioctl_biometric_get_sensor_status.htm
tech.root: biometric
ms.assetid: 88a2a73b-4fce-4f7a-b73b-ab66e136320d
ms.author: windowsdriverdev
ms.date: 2/20/2018
ms.keywords: IOCTL_BIOMETRIC_GET_SENSOR_STATUS, IOCTL_BIOMETRIC_GET_SENSOR_STATUS control, IOCTL_BIOMETRIC_GET_SENSOR_STATUS control code [Biometric Devices], biometric.ioctl_biometric_get_sensor_status, biometric_ref_74620630-37ce-4473-bb28-2fef40f885ad.xml, winbio_ioctl/IOCTL_BIOMETRIC_GET_SENSOR_STATUS
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: ioctl
req.header: winbio_ioctl.h
req.include-header: 
req.target-type: Windows
req.target-min-winverclnt: Available in Windows 7 and later versions of Windows.
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
-	Winbio_ioctl.h
api_name:
-	IOCTL_BIOMETRIC_GET_SENSOR_STATUS
product:
- Windows
targetos: Windows
req.typenames: 
---

# IOCTL_BIOMETRIC_GET_SENSOR_STATUS IOCTL


## -description


The IOCTL_BIOMETRIC_GET_SENSOR_STATUS IOCTL tells the driver to perform any necessary steps to collect the current operating status of the device. Vendor-supplied WBDI drivers must support this IOCTL.


## -ioctlparameters




### -input-buffer

None.


### -input-buffer-length

None.


### -output-buffer

The <b>AssociatedIrp</b>.<b>SystemBuffer</b> member points to a buffer that contains a <a href="https://msdn.microsoft.com/library/windows/hardware/ff536470">WINBIO_DIAGNOSTICS</a> structure.


### -output-buffer-length

The length of a <a href="https://msdn.microsoft.com/library/windows/hardware/ff536470">WINBIO_DIAGNOSTICS</a> structure.

The vendor-supplied driver can optionally return a DWORD-sized buffer that specifies the buffer size necessary for the requested operation.


### -in-out-buffer








### -inout-buffer-length








### -status-block

Indicates whether the DeviceIoControl call to the driver completed and the OUT payload is valid.

The <b>Status</b> member is set to one of the values in the following table.

<table>
<tr>
<th>Status value</th>
<th>Description</th>
</tr>
<tr>
<td>
S_OK, STATUS_SUCCESS

</td>
<td>
The operation completed successfully.  If the size of data returned is DWORD, the payload contains the size of the buffer necessary for the call.  Otherwise, the payload contains the full output buffer.

</td>
</tr>
<tr>
<td>
E_INVALIDARG

</td>
<td>
The parameters were not specified correctly.

</td>
</tr>
<tr>
<td>
E_UNKNOWN

</td>
<td>
Any other failure that prevents the payload from being filled in.

</td>
</tr>
<tr>
<td>
E_UNEXPECTED

</td>
<td>
Any other failure that prevents the payload from being filled in.

</td>
</tr>
<tr>
<td>
E_FAIL

</td>
<td>
Any other failure that prevents the payload from being filled in.

</td>
</tr>
</table>
 


## -remarks



If the vendor-supplied driver passes back the entire payload, it should fill in the <b>WinBioHresult</b> member of WINBIO_DIAGNOSTICS with the status of the Biometric operation. 



