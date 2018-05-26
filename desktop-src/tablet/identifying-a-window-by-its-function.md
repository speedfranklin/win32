---
Description: Description of identifying a window by its function for the Tablet PC.
ms.assetid: 513e0c9d-4c9e-4e7c-8314-bd7603489e89
title: Identifying a Window by Its Function
ms.date: 05/31/2018
ms.topic: article
ms.author: windowssdkdev
ms.prod: windows
ms.technology: desktop
---

# Identifying a Window by Its Function

Identify each type of window by assigning it a unique window class. Avoid having a single window class that is used for a wide variety of functions.

Accessibility aids must have this identification in order to handle different windows within the same application. There may be separate instructions for handling these windows, such as announcing specific areas when the content changes.

If you cannot use separate window classes, you can expose the differences through Microsoft&lt;entity type="reg"/&gt; Active Accessibility&lt;entity type="reg"/&gt;, or if necessary, by a private window message that you document on your website.

For more information about exposing window classes by using Active Accessibility, see the [Accessibility](https://msdn.microsoft.com/library/windows/desktop/ee663255) section.

 

 


