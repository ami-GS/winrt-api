---
-api-id: T:Windows.UI.Input.PointerPoint
-api-type: winrt class
---

<!-- Class syntax.
public class PointerPoint : Windows.UI.Input.IPointerPoint
-->

# Windows.UI.Input.PointerPoint

## -description

Provides basic properties for the input pointer associated with a single mouse, pen/stylus, or touch contact.

## -remarks

The PointerPoint class implements IPointerPoint.

See [PointerPointProperties](pointerpointproperties.md) for extended properties accessible through [Properties](pointerpoint_properties.md).

In most cases, we recommend that you get pointer info through the event argument of the pointer event handlers in your chosen language framework.

If the event argument doesn't intrinsically expose the pointer details required by your app, you can get access to extended pointer data through the [GetCurrentPoint](../windows.ui.xaml.input/pointerroutedeventargs_getcurrentpoint_1761708789.md) and [GetIntermediatePoints](../windows.ui.xaml.input/pointerroutedeventargs_getintermediatepoints_1716242609.md) methods of [PointerRoutedEventArgs](../windows.ui.xaml.input/pointerroutedeventargs.md). Use these methods to specify the context of the pointer data.

The static PointerPoint methods, [GetCurrentPoint](pointerpoint_getcurrentpoint_131721878.md) and [GetIntermediatePoints](pointerpoint_getintermediatepoints_143894736.md), always use the app context.

<!-- confirmed -->
> [!NOTE]
> This class is not agile, which means that you need to consider its threading model and marshaling behavior. For more info, see [Threading and Marshaling (C++/CX)](/cpp/cppcx/threading-and-marshaling-c-cx) and [Using Windows Runtime objects in a multithreaded environment (.NET)](/windows/uwp/threading-async/using-windows-runtime-objects-in-a-multithreaded-environment).

## -examples

In the following example, we query various pointer properties using a PointerPoint object.

[!code-csharp[QueryPointer](../windows.ui.input.inking/code/PointerInput/csharp/MainPage.xaml.cs#SnippetQueryPointer)]

[!code-csharp[QueryPointer](../windows.ui.input.inking/code/PointerInput_UWP/csharp/MainPage.xaml.cs#SnippetQueryPointer)]

## -see-also

[Windows.UI.Input Classes](windows_ui_input_classes.md), [Windows.Devices.Input](../windows.devices.input/windows_devices_input.md), [Windows.UI.Core](../windows.ui.core/windows_ui_core.md), [Windows.UI.Input](windows_ui_input.md), [Windows.UI.Input.Inking](../windows.ui.input.inking/windows_ui_input_inking.md), [Windows.UI.Xaml.Input](../windows.ui.xaml.input/windows_ui_xaml_input.md), [TypedEventHandler](../windows.foundation/typedeventhandler_2.md), [Custom user interactions](/windows/uwp/design/layout/index), [UX guidelines for custom user interactions](/windows/uwp/design/layout/index), [Touch design guidelines](/windows/uwp/input-and-devices/guidelines-for-user-interaction), [User interaction mode sample](https://github.com/Microsoft/Windows-universal-samples/tree/master/Samples/UserInteractionMode), [Focus visuals sample](https://go.microsoft.com/fwlink/p/?LinkID=619895), [Input: Device capabilities sample](/samples/browse/), [Input: Ink sample](/samples/browse/), [Input: Manipulations and gestures (JavaScript) sample](/samples/browse/), [Input: Simplified ink  sample](/samples/browse/), [Input: Windows 8 gestures sample](/samples/browse/), [Input: XAML user input events sample](/samples/browse/), [XAML scrolling, panning, and zooming sample](/samples/browse/), [DirectX touch input sample](/samples/browse/), [Input: Manipulations and gestures (C++) sample](/samples/browse/), [Input: Touch hit testing sample](/samples/browse/), [Input source identification sample](/samples/browse/), [Touch injection sample](/samples/browse/), [Win32 touch hit-testing sample](/samples/browse/), [Basic input sample (Windows 10)](https://go.microsoft.com/fwlink/p/?LinkId=620514)
