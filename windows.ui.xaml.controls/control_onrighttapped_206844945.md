---
-api-id: M:Windows.UI.Xaml.Controls.Control.OnRightTapped(Windows.UI.Xaml.Input.RightTappedRoutedEventArgs)
-api-type: winrt method
---

<!-- Method syntax
virtual protected void OnRightTapped(Windows.UI.Xaml.Input.RightTappedRoutedEventArgs e)
-->

# Windows.UI.Xaml.Controls.Control.OnRightTapped

## -description
Called before the [RightTapped](../windows.ui.xaml/uielement_righttapped.md) event occurs.

## -parameters
### -param e
Event data for the event.

## -remarks
<!--The following remark is relevant for Windows 8 > 8.1 migration. See WBB 458128-->
### Windows 8 behavior

Windows 8 had an issue with the data for the [RightTapped](../windows.ui.xaml/uielement_righttapped.md) event, where the **X** and **Y** values for the point you'd get from [RightTappedRoutedEventArgs.GetPosition](../windows.ui.xaml.input/righttappedroutedeventargs_getposition.md) were reversed (**X** was really **Y**; **Y** was really **X**). This issue has been fixed starting with Windows 8.1. But if you're retargeting a Windows 8 app for Windows 8.1, you might have had code that worked around this issue by swapping the **X** and **Y** back. If so, remove that code when you retarget because the issue is now fixed.

Apps that were compiled for Windows 8 but running on Windows 8.1 continue to use the Windows 8 behavior.


<!--The following remark is relevant for Windows 8 > 8.1 migration. See WBB 458260-->
Also, Windows 8 didn't include default key handling for Shift+F10 that would fire this event and then display context menus. Shift+F10 is typically a secondary key combination for the VK_APP virtual key value (the Properties key), and thus Shift+F10 might be expected to fire [RightTapped](../windows.ui.xaml/uielement_righttapped.md) too. This issue has been fixed starting with Windows 8.1; Shift+F10 now fires [RightTapped](../windows.ui.xaml/uielement_righttapped.md). You can see this change as default event handling on some controls that have default context menus for text, such as [TextBox](textbox.md), or when invoking custom menus and flyouts.

Apps that were compiled for Windows 8 but running on Windows 8.1 do not use this Windows 8 behavior, they use the corrected Windows 8.1 behavior.

## -examples

## -see-also
[UIElement.RightTapped](../windows.ui.xaml/uielement_righttapped.md), [RightTappedRoutedEventArgs](../windows.ui.xaml.input/righttappedroutedeventargs.md), [Events and routed events overview](http://msdn.microsoft.com/library/34c219e8-3efb-45bc-8bbd-6fd937698832), [Custom user interactions](http://msdn.microsoft.com/library/9403c46c-60da-4c13-a381-6fbd069dd9ce), [Handle pointer input](http://msdn.microsoft.com/library/bdbc9e33-4037-4671-9596-471dcf855c82)