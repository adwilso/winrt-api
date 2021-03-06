---
-api-id: M:Windows.UI.Notifications.BadgeUpdater.Clear
-api-type: winrt method
---

<!-- Method syntax
public void Clear()
-->

# Windows.UI.Notifications.BadgeUpdater.Clear

## -description
Removes the badge from the tile that the updater is bound to.

## -remarks
The badge can also be cleared by setting the badge value to "0" or "none".

> [!NOTE]
> If your badge is using periodic updates, you must also call [StopPeriodicUpdate](badgeupdater_stopperiodicupdate.md) or the badge will reappear at the next polling interval.

## -examples

## -see-also
[App tiles and badges sample](http://go.microsoft.com/fwlink/p/?linkid=231469), [Guidelines and checklist for tiles and badges](http://msdn.microsoft.com/library/e825f754-97dd-41c2-aff4-4dfb60eda677), [How to clear a badge](XREF:TODO:m_ui_tiles.howto_clear_a_badge), [How to send a glyph or numeric badge in a local notification](XREF:TODO:m_ui_tiles.howto_send_local_badge_notifications), [How to set up periodic notifications for badges](XREF:TODO:m_ui_tiles.howto_setup_badge_polling), [How to update a badge through push notifications](XREF:TODO:m_ui_tiles.howto_update_badges_push), [Badge XML schema](XREF:TODO:badge.Schema_Root), [Badge overview](http://msdn.microsoft.com/library/a64c58bb-d9c9-4c09-a685-4df94fa7dfdd)