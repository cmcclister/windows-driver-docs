---
title: DXGK\_POWER\_P\_STATE structure
description: Reserved for system use. Do not use it in your driver.
ms.assetid: F4612284-36C8-49C4-914D-43C32489EABD
keywords: ["DXGK_POWER_P_STATE structure Display Devices", "PDXGK_POWER_P_STATE structure pointer Display Devices"]
topic_type:
- apiref
api_name:
- DXGK_POWER_P_STATE
api_location:
- D3dkmddi.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 01/05/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# DXGK\_POWER\_P\_STATE structure


Reserved for system use. Do not use it in your driver.

Syntax
------

```ManagedCPlusPlus
typedef struct _DXGK_POWER_P_STATE {
  ULONG     NominalPower;
  ULONG     OperatingFrequency;
  ULONGLONG TransitionLatencies[DXGK_MAX_P_STATES];
  ULONGLONG ResidencyRequirement;
} DXGK_POWER_P_STATE, *PDXGK_POWER_P_STATE;
```

Members
-------

**NominalPower**

**OperatingFrequency**

**TransitionLatencies**

**ResidencyRequirement**

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Minimum supported client</p></td>
<td align="left"><p>Windows 8.1</p></td>
</tr>
<tr class="even">
<td align="left"><p>Minimum supported server</p></td>
<td align="left"><p>Windows Server 2012 R2</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Header</p></td>
<td align="left">D3dkmddi.h (include D3dkmddi.h)</td>
</tr>
</tbody>
</table>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20DXGK_POWER_P_STATE%20structure%20%20RELEASE:%20%281/4/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




