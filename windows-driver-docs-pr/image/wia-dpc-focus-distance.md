---
title: WIA\_DPC\_FOCUS\_DISTANCE
description: The WIA\_DPC\_FOCUS\_DISTANCE property contains the distance, in millimeters, between the image-capturing plane of a digital camera and the point of focus.
ms.assetid: 0f12fbdf-2c40-4b8b-9a22-ee35aa8cbc3f
keywords: ["WIA_DPC_FOCUS_DISTANCE Imaging Devices"]
topic_type:
- apiref
api_name:
- WIA_DPC_FOCUS_DISTANCE
api_location:
- Wiadef.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# WIA\_DPC\_FOCUS\_DISTANCE


The WIA\_DPC\_FOCUS\_DISTANCE property contains the distance, in millimeters, between the image-capturing plane of a digital camera and the point of focus.

## <span id="ddk_wia_dpc_focus_distance_si"></span><span id="DDK_WIA_DPC_FOCUS_DISTANCE_SI"></span>


Property Type: VT\_I4

Valid Values: WIA\_PROP\_RANGE or WIA\_PROP\_LIST

Access Rights: Read/write

Remarks
-------

A value of 0xFFFF for the WIA\_DPC\_FOCUS\_DISTANCE property corresponds to a setting that is greater than 655 meters.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Version</p></td>
<td><p>Obsolete in Windows Vista and later operating systems and should no longer be used. However, this property is still defined in Windows Vista for compatibility with applications and devices designed for Windows Server 2003, Windows XP, and previous versions of Windows.</p></td>
</tr>
<tr class="even">
<td><p>Header</p></td>
<td>Wiadef.h (include Wiadef.h)</td>
</tr>
</tbody>
</table>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20%5Bimage\image%5D:%20WIA_DPC_FOCUS_DISTANCE%20%20RELEASE:%20%2811/13/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




