---
title: NM\_THEMECHANGED notification code
description: Notifies a control's parent window that the theme has changed. This notification code is sent in the form of a WM\_NOTIFY message.
ms.assetid: '5e6a039e-9c35-4476-8cf1-5aea8977ed2d'
keywords: ["NM_THEMECHANGED notification code Windows Controls"]
topic_type:
- apiref
api_name:
- NM_THEMECHANGED
api_location:
- Commctrl.h
api_type:
- HeaderDef
---

# NM\_THEMECHANGED notification code

Notifies a control's parent window that the theme has changed. This notification code is sent in the form of a [**WM\_NOTIFY**](wm-notify.md) message.


```C++
NM_THEMECHANGED

    lpnmhdr = (LPNMHDR) lParam;
```



## Parameters

<dl> <dt>

*lParam* 
</dt> <dd>

A pointer to an [**NMHDR**](nmhdr.md) structure that contains additional information about this notification.

</dd> </dl>

## Return value

The return value is ignored by the control.

## Requirements



|                                     |                                                                                       |
|-------------------------------------|---------------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows�Vista \[desktop apps only\]<br/>                                        |
| Minimum supported server<br/> | Windows Server�2008 \[desktop apps only\]<br/>                                  |
| Header<br/>                   | <dl> <dt>Commctrl.h</dt> </dl> |



�

�




