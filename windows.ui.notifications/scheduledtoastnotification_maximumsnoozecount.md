---
-api-id: P:Windows.UI.Notifications.ScheduledToastNotification.MaximumSnoozeCount
-api-type: winrt property
---

<!-- Property syntax
public uint MaximumSnoozeCount { get; }
-->

# Windows.UI.Notifications.ScheduledToastNotification.MaximumSnoozeCount

## -description
Gets the maximum number of times to display this notification.

## -property-value
The maximum number of times to display this notification. This will be a value between 1 and 5, inclusive.

## -remarks
Note that this is the number of repeat showings specified when the [ScheduledToastNotification](scheduledtoastnotification.md) is created. It is not the number of showings remaining if the toast has already been shown. There is no method to directly retrieve that information.

## -examples

## -see-also
[Scheduled notifications sample](http://go.microsoft.com/fwlink/p/?linkid=241614), [Toast schema](XREF:TODO:toast.Schema_Root), [Guidelines and checklist for scheduled notifications](XREF:TODO:m_ui_tiles.guidelines_for_scheduled_notifications)