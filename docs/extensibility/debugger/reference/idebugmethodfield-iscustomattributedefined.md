---
description: "Determines whether a specific custom attribute has been defined."
title: IDebugMethodField::IsCustomAttributeDefined
ms.date: 11/04/2016
ms.topic: reference
f1_keywords:
- IDebugMethodField::IsCustomAttributeDefined
helpviewer_keywords:
- IDebugMethodField::IsCustomAttributeDefined method
author: maiak
ms.author: maiak
manager: jmartens
ms.technology: vs-ide-debug
dev_langs:
- CPP
- CSharp
---
# IDebugMethodField::IsCustomAttributeDefined

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Determines whether a specific custom attribute has been defined.

## Syntax

### [C#](#tab/csharp)
```csharp
int IsCustomAttributeDefined(
   [In] string pszCustomAttributeName
);
```
### [C++](#tab/cpp)
```cpp
HRESULT IsCustomAttributeDefined( 
   LPCOLESTR pszCustomAttributeName
);
```
---

## Parameters
`pszCustomAttributeName`\
[in] A string containing the name of the custom attribute to find.

## Return Value
 Returns S_OK if the custom attribute is defined on this method, otherwise returns S_FALSE.

## See also
- [IDebugMethodField](../../../extensibility/debugger/reference/idebugmethodfield.md)
