---
UID: NF:wdtfsimulatedbatterysystemaction.IWDTFSimulatedBatterySystemAction.SetSimulatedBatteryToAC
title: IWDTFSimulatedBatterySystemAction::SetSimulatedBatteryToAC
author: windows-driver-content
description: Sets the simulated battery status to AC power.
old-location: dtf\iwdtfsimulatedbatterysystemaction_setsimulatedbatterytoac.htm
tech.root: dtf
ms.assetid: ddfd38d9-a78e-4573-9bf3-24f2f69b5949
ms.author: windowsdriverdev
ms.date: 4/4/2018
ms.keywords: IWDTFSimulatedBatterySystemAction interface [Windows Device Testing Framework],SetSimulatedBatteryToAC method, IWDTFSimulatedBatterySystemAction.SetSimulatedBatteryToAC, IWDTFSimulatedBatterySystemAction::SetSimulatedBatteryToAC, SetSimulatedBatteryToAC, SetSimulatedBatteryToAC method [Windows Device Testing Framework], SetSimulatedBatteryToAC method [Windows Device Testing Framework],IWDTFSimulatedBatterySystemAction interface, dtf.iwdtfsimulatedbatterysystemaction_setsimulatedbatterytoac, wdtfsimulatedbatterysystemaction/IWDTFSimulatedBatterySystemAction::SetSimulatedBatteryToAC
ms.prod: windows-hardware
ms.technology: windows-devices
ms.topic: method
req.header: wdtfsimulatedbatterysystemaction.h
req.include-header: 
req.target-type: Desktop
req.target-min-winverclnt: Windows 8.1
req.target-min-winversvr: Windows Server 2012 R2
req.kmdf-ver: 
req.umdf-ver: 
req.ddi-compliance: 
req.unicode-ansi: 
req.idl: WDTFSimulatedBatterySystemAction.idl
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
-	COM
api_location:
-	wdtfsimulatedbatterysystemaction.h
api_name:
-	IWDTFSimulatedBatterySystemAction.SetSimulatedBatteryToAC
product:
- Windows
targetos: Windows
req.typenames: 
---

# IWDTFSimulatedBatterySystemAction::SetSimulatedBatteryToAC


## -description



Sets the simulated battery status to AC power.



Use this method to set the simulated battery status to AC power.  If
    real batteries in the system are disabled, this sets the OS status and 
    policy to AC power.  This is useful for testing software behavior that
    changes depending on the AC/DC state.


## -parameters




### -param pbSuccess [out, retval]


## -returns



If this method succeeds, it returns <b xmlns:loc="http://microsoft.com/wdcml/l10n">S_OK</b>. Otherwise, it returns an <b xmlns:loc="http://microsoft.com/wdcml/l10n">HRESULT</b> error code.




## -see-also




<a href="https://msdn.microsoft.com/library/windows/hardware/dn265160">IWDTFSimulatedBatterySystemAction</a>
 

 

