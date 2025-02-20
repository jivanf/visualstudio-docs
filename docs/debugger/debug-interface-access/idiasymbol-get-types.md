---
description: "Retrieves an array of compiler-specific types for this symbol."
title: "IDiaSymbol::get_types"
ms.date: "11/04/2016"
ms.topic: "reference"
dev_langs:
  - "C++"
helpviewer_keywords:
  - "IDiaSymbol::get_types method"
author: "mikejo5000"
ms.author: "mikejo"
manager: jmartens
ms.technology: vs-ide-debug
---
# IDiaSymbol::get_types

 [!INCLUDE [Visual Studio](~/includes/applies-to-version/vs-windows-only.md)]
Retrieves an array of compiler-specific types for this symbol.

## Syntax

```C++
HRESULT get_types ( 
   DWORD       cTypes,
   DWORD*      pcTypes,
   IDiaSymbol* types[]
);
```

#### Parameters
 `cTypes`

[in] Size of the buffer to hold the data.

 `pcTypes`

[out] Returns the number of types written, or, if the `types` parameter is `NULL`, then the total number of types available.

 `types[]`

[out] An array that is to be filled in with the [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md) objects that represent all the types for this symbol.

## Return Value
 If successful, returns `S_OK`; otherwise, returns `S_FALSE` or an error code.

> [!NOTE]
> A return value of `S_FALSE` means the property is not available for the symbol.

## See also
- [IDiaSymbol](../../debugger/debug-interface-access/idiasymbol.md)
