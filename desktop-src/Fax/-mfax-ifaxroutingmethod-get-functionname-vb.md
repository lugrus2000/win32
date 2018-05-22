﻿---
Description: 'The FunctionName property is a null-terminated string that contains the name of the function that executes a specific fax routing procedure.'
ms.assetid: '144023b3-bf12-4e81-856c-6745695d9c30'
title: 'FaxRoutingMethod.FunctionName property'
---

# FaxRoutingMethod.FunctionName property

The **FunctionName** property is a null-terminated string that contains the name of the function that executes a specific fax routing procedure.

This property is read-only.

## Syntax


```VB
Property FunctionName As String
```



## Property value

A **String** that receives the name of the function that executes the specified fax routing procedure. The fax routing extension DLL identified by the [**ImageName**](-mfax-ifaxroutingmethod-get-imagename-vb.md) property defines and exports the function.

## Remarks

A fax client application can use the [**Guid**](-mfax-ifaxroutingmethod-get-guid-vb.md) property to uniquely identify a fax routing method. It is possible for multiple routing methods to have the same user-friendly name and even the same function name. For more information, see [Fax Routing Methods](-mfax-fax-routing-methods.md).

**FunctionName** allocates the memory required for the buffer pointed to by the *pVal* parameter. The client application must call the [SysFreeString](8f230ee3-5f6e-4cb9-a910-9c90b754dcd3) function to deallocate the resources associated with this parameter. For more information, see [Freeing Fax Resources](-mfax-freeing-fax-resources.md).

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows 2000 Professional \[desktop apps only\]<br/>                            |
| Minimum supported server<br/> | Windows 2000 Server \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Faxcom.h</dt> </dl>   |
| DLL<br/>                      | <dl> <dt>Faxcom.dll</dt> </dl> |



## See also

<dl> <dt>

[**FaxRoutingMethod**](-mfax-faxroutingmethod-object-visual-basic-.md)
</dt> <dt>

[Fax Service Client API for Windows 2000](-mfax-fax-service-client-api-for-windows-2000.md)
</dt> <dt>

[Fax Service Client API Interfaces](-mfax-fax-service-client-api-interfaces.md)
</dt> <dt>

[**IFaxRoutingMethod**](-mfax-ifaxroutingmethod.md)
</dt> <dt>

[**IFaxRoutingMethods**](-mfax-ifaxroutingmethods.md)
</dt> <dt>

[**FriendlyName**](-mfax-ifaxroutingmethod-get-friendlyname-vb.md)
</dt> <dt>

[**FaxRouteMethod**](-mfax-faxroutemethod.md)
</dt> </dl>

 

 



