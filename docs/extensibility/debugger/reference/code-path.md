---
description: "Describes a method or function call."
title: CODE_PATH
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- CODE_PATH
helpviewer_keywords:
- CODE_PATH structure
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# CODE_PATH

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Describes a method or function call.

## Syntax

### [C#](#tab/csharp)
```csharp
public struct CODE_PATH {
    public string            bstrName;
    public IDebugCodeContext pCode;
}
```
### [C++](#tab/cpp)
```cpp
typedef struct tagCODE_PATH { 
    BSTR                bstrName;
    IDebugCodeContext2* pCode;
} CODE_PATH;
```
---

## Members
`bstrName`\
The name of the code path.

`pCode`\
The [IDebugCodeContext2](../../../extensibility/debugger/reference/idebugcodecontext2.md) object that identifies where in the code to step into a function.

## Remarks
This structure is used to implement stepping into a function. [EnumCodePaths](../../../extensibility/debugger/reference/idebugprogram2-enumcodepaths.md) returns all the calls from the current location in the program being debugged. This structure represents one such call.

## Requirements
Header: msdbg.h

Namespace: Microsoft.VisualStudio.Debugger.Interop

Assembly: Microsoft.VisualStudio.Debugger.Interop.dll

## See also
- [Structures and Unions](../../../extensibility/debugger/reference/structures-and-unions.md)
- [IDebugCodeContext2](../../../extensibility/debugger/reference/idebugcodecontext2.md)
- [EnumCodePaths](../../../extensibility/debugger/reference/idebugprogram2-enumcodepaths.md)
