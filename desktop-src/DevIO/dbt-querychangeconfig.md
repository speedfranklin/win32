---
Description: The system broadcasts the DBT\_QUERYCHANGECONFIG device event to request permission to change the current configuration (dock or undock). Any application can deny this request and cancel the change.
ms.assetid: 2e452ea7-e2bf-4500-952a-ee7d891533a0
title: DBT_QUERYCHANGECONFIG event (Dbt.h)
ms.topic: reference
ms.date: 05/31/2018
---

# DBT\_QUERYCHANGECONFIG event

The system broadcasts the DBT\_QUERYCHANGECONFIG device event to request permission to change the current configuration (dock or undock). Any application can deny this request and cancel the change.

To broadcast this device event, the system uses the [**WM\_DEVICECHANGE**](wm-devicechange.md) message with *wParam* set to DBT\_QUERYCHANGECONFIG and *lParam* set to zero.


```C++
LRESULT CALLBACK WindowProc(
  HWND hwnd,       // handle to window
  UINT uMsg,       // WM_DEVICECHANGE
  WPARAM wParam,   // device-change event
  LPARAM lParam    // event-specific data
);
```



## Parameters

<dl> <dt>

*hwnd* 
</dt> <dd>

A handle to a window.

</dd> <dt>

*uMsg* 
</dt> <dd>

The [**WM\_DEVICECHANGE**](wm-devicechange.md) message identifier.

</dd> <dt>

*wParam* 
</dt> <dd>

Set to DBT\_QUERYCHANGECONFIG.

</dd> <dt>

*lParam* 
</dt> <dd>

Set to zero.

</dd> </dl>

## Return value

Return **TRUE** to grant permission to change the configuration.

Return BROADCAST\_QUERY\_DENY to deny permission to change the configuration.

## Requirements



| Requirement | Value |
|-------------------------------------|----------------------------------------------------------------------------------|
| Minimum supported client<br/> | Windows XP<br/>                                                            |
| Minimum supported server<br/> | Windows Server 2003<br/>                                                   |
| Header<br/>                   | <dl> <dt>Dbt.h</dt> </dl> |



## See also

<dl> <dt>

[Device Events](device-events.md)
</dt> <dt>

[Device Management Events](device-management-events.md)
</dt> <dt>

[**WM\_DEVICECHANGE**](wm-devicechange.md)
</dt> </dl>

 

 




