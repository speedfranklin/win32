---
Description: The InkEdit control provides an easy way to capture, recognize, and display ink.
ms.assetid: a1dfa254-cade-44c5-8fdd-74bb40849063
title: InkEdit Control
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# InkEdit Control

The [InkEdit](inkedit-control-reference.md) control provides an easy way to capture, recognize, and display ink.

This implementation of the [InkEdit](inkedit-control-reference.md) control is based on the [**RichEdit**](https://msdn.microsoft.com/library/windows/desktop/bb774306) control. The managed (.NET Framework) implementation of [InkEdit](frlrfMicrosoftInkInkEditClassTopic) is based on the [**RichTextBox**](T:System.Windows.Controls.RichTextBox) control.

The primary purpose of the [InkEdit](inkedit-control-reference.md) control is to collect ink, recognize it, and display it in text form. Additionally, it supports displaying ink as an embedded object with text formatting capabilities, such as bold and underline.

## Gestures and Correction

[InkEdit](inkedit-control-reference.md) supports the following gestures.



| Gesture                                                                    | Gesture Name              | Action               |
|----------------------------------------------------------------------------|---------------------------|----------------------|
| ![down-left gesture](images/d8b00c0a-f450-4f71-980f-3bca1b558e4c.gif)      | Down-left<br/>      | Enter<br/>     |
| ![down-left-long gesture](images/b8cb23b5-b947-477d-922f-2ffb42756804.gif) | Down-left-long<br/> | Enter<br/>     |
| ![up-right gesture](images/02c34d24-c2d7-404f-b99a-742ba6de7f0c.gif)       | Up-right<br/>       | Tab<br/>       |
| ![up-right-long gesture.](images/5e3522d3-2920-4a86-86ae-f29b01d93993.gif) | Up-right-long<br/>  | Tab<br/>       |
| ![right gesture](images/864cf4e1-2619-49cf-ac96-72994232e465.jpg)          | Right<br/>          | Space<br/>     |
| ![left gesture](images/ce60cc20-1769-428d-80de-7f47c86021fb.jpg)           | Left<br/>           | Backspace<br/> |



 

Gesture events that you can handle contain gesture, stroke, and cursor information you can use to send text to [InkEdit](inkedit-control-reference.md) or place data on the clipboard.

[InkEdit](inkedit-control-reference.md) also provides a correction user interface that enables users to view and select from alternates, use the on-screen keyboard, and character/letter/block recognizers.

## Other Details

[InkEdit](inkedit-control-reference.md) is designed to work well in a form scenario for single line as well as multiline text entry and editing. The primary intended use for InkEdit is to get text input from a user in the form of handwriting. By default, ink input is recognized and text is inserted in its place. The default user interface for InkEdit resembles that of the [**RichTextBox**](T:System.Windows.Controls.RichTextBox) control, except when the user is laying down ink. You can display original ink rather than text; however, the ink is scaled to the current input font size of the InkEdit control and is displayed inline with other text.

> [!Note]  
> For security reasons, you must use standard procedures to open or close a file, stream the input/output, and set the [**RTF**](/windows/win32/inked/?branch=master) or [**Text**](/windows/win32/inked/?branch=master) property.

 

The [InkEdit](inkedit-control-reference.md) control is set to recognize ink as text by default. To enable users to add ink as ink, set the [**InkInsertMode**](/windows/win32/inked/?branch=master) property to **InsertAsInk**.

For detailed reference information about the [InkEdit](inkedit-control-reference.md) control, see InkEdit.

> [!Note]  
> If you use the Win32 [InkEdit](inkedit-control-reference.md) control and place it inside a group box, make sure the box has a transparent style; otherwise, InkEdit is not able to collect ink.

 

> [!Note]  
> To ensure ink is displayed properly, call the [InkEdit](inkedit-control-reference.md) control [**Refresh**](/windows/win32/inked/?branch=master) method when it receives an [**HScroll**](frlrfSystemWindowsFormsRichTextBoxClassHScrollTopic) or [**VScroll**](frlrfSystemWindowsFormsRichTextBoxClassVScrollTopic) event.

 

The following sections detail the use of the [InkEdit](inkedit-control-reference.md) control:

-   [Instantiating InkEdit](instantiating-inkedit.md)
-   [Word vs. Character Recognition](word-vs--character-recognition.md)
-   [Displaying Ink as Ink](displaying-ink-as-ink.md)
-   [Using InkEdit on Earlier Versions of Windows](using-inkedit-on-earlier-versions-of-windows.md)
-   [Using an Application Dictionary with InkEdit](using-an-application-dictionary-with-inkedit.md)

 

 



