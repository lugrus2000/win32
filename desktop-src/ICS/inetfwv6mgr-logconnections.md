---
title: INetFwV6Mgr LogConnections property
description: Specifies whether the firewall logs information about connections to the file location at LogfilePath.
ms.assetid: '87362401-7686-4cb5-bbd2-e2c3e13ef9ab'
keywords: ["LogConnections property ICS/ICF", "LogConnections property ICS/ICF , INetFwV6Mgr interface", "INetFwV6Mgr interface ICS/ICF , LogConnections property"]
topic_type:
- apiref
api_name:
- INetFwV6Mgr.LogConnections
- INetFwV6Mgr.get_LogConnections
- INetFwV6Mgr.put_LogConnections
api_location:
- Netfwv6.dll
api_type:
- COM
---

# INetFwV6Mgr::LogConnections property

\[The IPv6 Internet Connection Firewall is available for use in the operating systems specified in the Requirements section. Instead, use the [Windows Firewall API](windows-firewall-start-page.md).\]

Specifies whether the firewall logs information about connections to the file location at [**LogfilePath**](inetfwv6mgr-logfilepath.md).

This property is read/write.

## Syntax


```C++
HRESULT put_LogConnections(
  [in]��VARIANT_BOOL bvLogConnections
);

HRESULT get_LogConnections(
  [out]�VARIANT_BOOL *pbvLogConnections
);
```



## Property value

Specifies the value to set.

## Error codes

If the method succeeds, the return value is S\_OK.

If the method fails, the return value is one of the following error codes.



| Name                                                                                      | Meaning                                                       |
|-------------------------------------------------------------------------------------------|---------------------------------------------------------------|
| <dl> <dt>E\_ABORT</dt> </dl>       | The operation was aborted.<br/>                         |
| <dl> <dt>E\_FAIL</dt> </dl>        | An unspecified error occurred.<br/>                     |
| <dl> <dt>E\_INVALIDARG</dt> </dl>  | One of the parameters is invalid.<br/>                  |
| <dl> <dt>E\_NOINTERFACE</dt> </dl> | A specified interface is not supported.<br/>            |
| <dl> <dt>E\_NOTIMPL</dt> </dl>     | A specified method is not implemented.<br/>             |
| <dl> <dt>E\_OUTOFMEMORY</dt> </dl> | The method was unable to allocate required memory.<br/> |
| <dl> <dt>E\_POINTER</dt> </dl>     | A pointer passed as a parameter is not valid.<br/>      |
| <dl> <dt>E\_UNEXPECTED</dt> </dl>  | The method failed for unknown reasons.<br/>             |



## Requirements



|                                     |                                                                                        |
|-------------------------------------|----------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�XP with SP1 \[desktop apps only\]<br/>                                   |
| Minimum supported server<br/> | None supported<br/>                                                              |
| End of client support<br/>    | Windows�XP with SP1<br/>                                                         |
| Redistributable<br/>          | Advanced Networking Pack for Windows�XP<br/>                                     |
| Header<br/>                   | <dl> <dt>Netfwv6.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Netfwv6.dll</dt> </dl> |



## See also

<dl> <dt>

[INetFwV6Mgr](https://msdn.microsoft.com/library/windows/desktop/aa365874)
</dt> <dt>


</dt> <dt>

[**INetFwV6Mgr**](inetfwv6mgr.md)
</dt> </dl>

�

�




