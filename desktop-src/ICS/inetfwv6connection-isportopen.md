---
title: INetFwV6Connection IsPortOpen method
description: The IsPortOpen method checks if inbound connection attempts are allowed for the specified port and protocol pair.
ms.assetid: 28dad0f2-3126-4577-9fdf-e6f6e9ee3110
keywords:
- IsPortOpen method ICS/ICF
- IsPortOpen method ICS/ICF , INetFwV6Connection interface
- INetFwV6Connection interface ICS/ICF , IsPortOpen method
topic_type:
- apiref
api_name:
- INetFwV6Connection.IsPortOpen
api_location:
- Netfwv6.dll
api_type:
- COM
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# INetFwV6Connection::IsPortOpen method

\[The IPv6 Internet Connection Firewall is available for use in the operating systems specified in the Requirements section. Instead, use the [Windows Firewall API](windows-firewall-start-page.md).\]

The **IsPortOpen** method checks if inbound connection attempts are allowed for the specified port and protocol pair.

## Syntax


```C++
HRESULT IsPortOpen(
  [in]  USHORT        usPort,
  [in]  PORT_PROTOCOL Protocol,
  [out] VARIANT_BOOL  pvbPortIsOpen
);
```



## Parameters

<dl> <dt>

*usPort* \[in\]
</dt> <dd>

Specified in host byte order, and must be in the range 1   65535.

</dd> <dt>

*Protocol* \[in\]
</dt> <dd>

Specifies a value defined in the [**PORT\_PROTOCOL**](port-protocol.md) enumeration.

</dd> <dt>

*pvbPortIsOpen* \[out\]
</dt> <dd>

Receives the port open status.

</dd> </dl>

## Return value

If the method succeeds the return value is S\_OK.

If the method fails, the return value is one of the following error codes.



| Return code                                                                                   | Description                                                   |
|-----------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| <dl> <dt>**E\_ABORT**</dt> </dl>       | The operation was aborted.<br/>                         |
| <dl> <dt>**E\_FAIL**</dt> </dl>        | An unspecified error occurred.<br/>                     |
| <dl> <dt>**E\_INVALIDARG**</dt> </dl>  | One of the parameters is invalid.<br/>                  |
| <dl> <dt>**E\_NOINTERFACE**</dt> </dl> | A specified interface is not supported.<br/>            |
| <dl> <dt>**E\_NOTIMPL**</dt> </dl>     | A specified method is not implemented.<br/>             |
| <dl> <dt>**E\_OUTOFMEMORY**</dt> </dl> | The method was unable to allocate required memory.<br/> |
| <dl> <dt>**E\_POINTER**</dt> </dl>     | A pointer passed as a parameter is not valid.<br/>      |
| <dl> <dt>**E\_UNEXPECTED**</dt> </dl>  | The method failed for unknown reasons.<br/>             |



 

## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP with SP1 \[desktop apps only\]<br/>                                   |
| Minimum supported server<br/> | None supported<br/>                                                              |
| End of client support<br/>    | Windows XP with SP1<br/>                                                         |
| Redistributable<br/>          | Advanced Networking Pack for Windows XP<br/>                                     |
| Header<br/>                   | <dl> <dt>Netfwv6.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Netfwv6.dll</dt> </dl> |



## See also

<dl> <dt>

[**INetFwV6Connection**](inetfwv6connection.md)
</dt> </dl>

 

 




