---
title: Add Existing Item Command
description: Learn about the Add Existing Item command and how it adds an existing file to a current solution and opens it.
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- project.addexistingitem
helpviewer_keywords:
- File.AddExistingItem command
- Add Existing Item command
ms.assetid: 41f56131-d4c7-4f81-83b7-bdac713ea870
author: TerryGLee
ms.author: tglee
manager: jmartens
ms.technology: vs-ide-general
ms.workload:
- multiple
---
# Add Existing Item Command

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Adds an existing file to the current solution and opens it.

## Syntax

```cmd
File.AddExistingItem filename [/e:editorname]
```

## Arguments
`filename`\
Required. The full path and file name, with extension, of the item to add to the current solution. If the file path or file name contains spaces, enclose the entire path in quotation marks.

## Switches
/e: `editorname`\
Optional. Name of the editor in which the file will be opened. If the argument is specified but no editor name is supplied, the **Open With** dialog box appears.

The /e:`editorname` argument syntax uses the editor names as they appear in the **Open With Dialog Box**, enclosed in quotation marks. For example, to open a style sheet in the source code editor, you would enter the following for the /e:`editorname` argument.

```cmd
/e:"Source Code (text) Editor"
```

## Remarks
Autocompletion tries to locate the correct path and file name as you type.

## Example
This example adds the file, Form1.frm, to the current solution.

```cmd
>File.AddExistingItem "C:\public\solution files\Form1.frm"
```

## See also

- [Visual Studio Commands](../../ide/reference/visual-studio-commands.md)
- [Command Window](../../ide/reference/command-window.md)
- [Find/Command Box](../../ide/find-command-box.md)
- [Visual Studio Command Aliases](../../ide/reference/visual-studio-command-aliases.md)
