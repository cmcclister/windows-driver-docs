---
title: D3DKMT\_OUTPUTDUPL\_GET\_POINTER\_SHAPE\_DATA structure
description: Reserved for system use. Do not use in your driver.
ms.assetid: 31502888-88b0-49c2-8f03-63bb31886931
keywords: ["D3DKMT_OUTPUTDUPL_GET_POINTER_SHAPE_DATA structure Display Devices"]
topic_type:
- apiref
api_name:
- D3DKMT_OUTPUTDUPL_GET_POINTER_SHAPE_DATA
api_location:
- D3dkmthk.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 01/05/2018
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# D3DKMT\_OUTPUTDUPL\_GET\_POINTER\_SHAPE\_DATA structure


Reserved for system use. Do not use in your driver.

Syntax
------

```ManagedCPlusPlus
typedef struct _D3DKMT_OUTPUTDUPL_GET_POINTER_SHAPE_DATA {
  D3DKMT_HANDLE                     hAdapter;
  D3DDDI_VIDEO_PRESENT_SOURCE_ID    VidPnSourceId;
  UINT                              BufferSizeSupplied;
  PVOID                             pShapeBuffer;
  UINT                              BufferSizeRequired;
  D3DKMT_OUTDUPL_POINTER_SHAPE_INFO ShapeInfo;
} D3DKMT_OUTPUTDUPL_GET_POINTER_SHAPE_DATA;
```

Members
-------

**hAdapter**

**VidPnSourceId**

**BufferSizeSupplied**

**pShapeBuffer**

**BufferSizeRequired**

**ShapeInfo**

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
<td align="left"><p>Windows 8</p></td>
</tr>
<tr class="even">
<td align="left"><p>Minimum supported server</p></td>
<td align="left"><p>Windows Server 2012</p></td>
</tr>
<tr class="odd">
<td align="left"><p>Header</p></td>
<td align="left">D3dkmthk.h (include D3dkmthk.h)</td>
</tr>
</tbody>
</table>

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[display\display]:%20D3DKMT_OUTPUTDUPL_GET_POINTER_SHAPE_DATA%20structure%20%20RELEASE:%20%281/4/2018%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")




