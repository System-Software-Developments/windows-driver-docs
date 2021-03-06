---
title: DEVPKEY_Device_FriendlyName
description: DEVPKEY_Device_FriendlyName
ms.assetid: 0acea25e-5068-441b-be6b-fa863d1bdba2
keywords: ["DEVPKEY_Device_FriendlyName Device and Driver Installation"]
topic_type:
- apiref
api_name:
- DEVPKEY_Device_FriendlyName
api_location:
- Devpkey.h
api_type:
- HeaderDef
ms.localizationpriority: medium
ms.date: 10/17/2018
---

# DEVPKEY_Device_FriendlyName


The DEVPKEY_Device_FriendlyName device property represents the friendly name of a device instance.

<table>
<colgroup>
<col width="50%" />
<col width="50%" />
</colgroup>
<thead>
<tr>
<th>Attribute</th>
<th>Value</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left"><p><strong>Property key</strong></p></td>
<td align="left"><p>DEVPKEY_Device_FriendlyName</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Property-data-type identifier</strong></p></td>
<td align="left"><p><a href="devprop-type-string.md" data-raw-source="[&lt;strong&gt;DEVPROP_TYPE_STRING&lt;/strong&gt;](devprop-type-string.md)"><strong>DEVPROP_TYPE_STRING</strong></a></p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Property access</strong></p></td>
<td align="left"><p>Read and write access by installation applications and installers</p></td>
</tr>
<tr class="even">
<td align="left"><p><strong>Corresponding SPDRP_</strong><em>Xxx</em> <strong>identifier</strong></p></td>
<td align="left"><p>SPDRP_FRIENDLYNAME</p></td>
</tr>
<tr class="odd">
<td align="left"><p><strong>Localized?</strong></p></td>
<td align="left"><p>No</p></td>
</tr>
</tbody>
</table>

 

Remarks
-------

You can use the [**DEVPKEY_NAME**](devpkey-name--device-instance-.md) device property instead of DEVPKEY_Device_FriendlyName to display the name that identifies a device instance in a user interface display.

You can set the value of DEVPKEY_Device_FriendlyName by using an [**INF AddReg directive**](https://docs.microsoft.com/windows-hardware/drivers/install/inf-addreg-directive) that is included in the [**INF *DDInstall*.HW section**](https://docs.microsoft.com/windows-hardware/drivers/install/inf-ddinstall-hw-section) in the INF file that installs a device.

You can retrieve the value of DEVPKEY_Device_FriendlyName by calling [**SetupDiGetDeviceProperty**](https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdigetdevicepropertyw) or you can set this property by calling [**SetupDiSetDeviceProperty**](https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdisetdevicepropertyw).

Windows Server 2003, Windows XP, and Windows 2000 support this property, but do not support the DEVPKEY_Device_FriendlyName property key. Instead, you can use the corresponding SPDRP_FRIENDLYNAME identifier to access the value of the property on these earlier versions of Windows. For information about how to access this property value on these earlier versions of Windows, see [Accessing Device Instance SPDRP_Xxx Properties](https://docs.microsoft.com/windows-hardware/drivers/install/accessing-device-instance-spdrp-xxx-properties).

Requirements
------------

**Version**: Windows Vista and later versions of Windows
**Header**: Devpkey.h (include Devpkey.h)


## See also


[**DEVPKEY_NAME (Device Instance)**](devpkey-name--device-instance-.md)

[**INF AddReg Directive**](https://docs.microsoft.com/windows-hardware/drivers/install/inf-addreg-directive)

[**INF *DDInstall*.HW Section**](https://docs.microsoft.com/windows-hardware/drivers/install/inf-ddinstall-hw-section)

[**SetupDiGetDeviceProperty**](https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdigetdevicepropertyw)

[**SetupDiSetDeviceProperty**](https://docs.microsoft.com/windows/desktop/api/setupapi/nf-setupapi-setupdisetdevicepropertyw)

 

 






