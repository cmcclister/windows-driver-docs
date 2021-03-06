---
title: KSPROPERTY\_AUDIOENGINE\_LOOPBACK\_PROTECTION
description: The KSPROPERTY\_AUDIOENGINE\_LOOPBACK\_PROTECTION property request allows the audio driver to set the loopback protection status of the audio engine node.
ms.assetid: E798582C-7662-413C-B25C-6A129FDEEE38
keywords: ["KSPROPERTY_AUDIOENGINE_LOOPBACK_PROTECTION Audio Devices"]
topic_type:
- apiref
api_name:
- KSPROPERTY_AUDIOENGINE_LOOPBACK_PROTECTION
api_location:
- Ksmedia.h
api_type:
- HeaderDef
ms.author: windowsdriverdev
ms.date: 11/28/2017
ms.topic: article
ms.prod: windows-hardware
ms.technology: windows-devices
---

# KSPROPERTY\_AUDIOENGINE\_LOOPBACK\_PROTECTION


The **KSPROPERTY\_AUDIOENGINE\_LOOPBACK\_PROTECTION** property request allows the audio driver to set the loopback protection status of the audio engine node.

### <span id="Usage_Summary_Table"></span><span id="usage_summary_table"></span><span id="USAGE_SUMMARY_TABLE"></span>Usage Summary Table

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">Get</th>
<th align="left">Set</th>
<th align="left">Target</th>
<th align="left">Property descriptor type</th>
<th align="left">Property value type</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p>No</p></td>
<td align="left"><p>Yes</p></td>
<td align="left"><p>Node via Pin instance</p></td>
<td align="left"><p>KSP_NODE</p></td>
<td align="left"><p>ULONG</p></td>
</tr>
</tbody>
</table>

 

### <span id="Return_Value"></span><span id="return_value"></span><span id="RETURN_VALUE"></span>Return Value

The KSPROPERTY\_AUDIOENGINE\_LOOPBACK\_PROTECTION property request returns STATUS\_SUCCESS to indicate that it has completed successfully. Otherwise, the request returns an appropriate error status code.

Remarks
-------

The input buffer that is associated with this property call is populated with an enumeration value of type CONSTRICTOR\_OPTION. So the input buffer is either set to CONSTRICTOR\_OPTION\_DISABLE or CONSTRICTOR\_OPTION\_MUTE.

If there are any active streams with CONSTRICTOR\_OPTION\_MUTE in effect, then the KS loopback tap for this audio output will emit silence. If all the active streams have CONSTRICTOR\_OPTION\_DISABLE in effect (which is the default state), then and only then does the loopback tap contain meaningful data.

Requirements
------------

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<tbody>
<tr class="odd">
<td align="left"><p>Version</p></td>
<td align="left"><p>Windows 8</p></td>
</tr>
<tr class="even">
<td align="left"><p>Header</p></td>
<td align="left">Ksmedia.h</td>
</tr>
</tbody>
</table>

## <span id="see_also"></span>See also


[**KSPROPERTY\_AUDIOENGINE**](ksproperty-audioengine.md)

 

 

[Send comments about this topic to Microsoft](mailto:wsddocfb@microsoft.com?subject=Documentation%20feedback%20[audio\audio]:%20KSPROPERTY_AUDIOENGINE_LOOPBACK_PROTECTION%20%20RELEASE:%20%2811/22/2017%29&body=%0A%0APRIVACY%20STATEMENT%0A%0AWe%20use%20your%20feedback%20to%20improve%20the%20documentation.%20We%20don't%20use%20your%20email%20address%20for%20any%20other%20purpose,%20and%20we'll%20remove%20your%20email%20address%20from%20our%20system%20after%20the%20issue%20that%20you're%20reporting%20is%20fixed.%20While%20we're%20working%20to%20fix%20this%20issue,%20we%20might%20send%20you%20an%20email%20message%20to%20ask%20for%20more%20info.%20Later,%20we%20might%20also%20send%20you%20an%20email%20message%20to%20let%20you%20know%20that%20we've%20addressed%20your%20feedback.%0A%0AFor%20more%20info%20about%20Microsoft's%20privacy%20policy,%20see%20http://privacy.microsoft.com/default.aspx. "Send comments about this topic to Microsoft")





