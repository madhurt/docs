---
title: "ICorDebugEval2::NewStringWithLength Method | Microsoft Docs"
ms.custom: ""
ms.date: "03/30/2017"
ms.prod: ".net-framework-4.6"
ms.reviewer: ""
ms.suite: ""
ms.technology: 
  - "dotnet-clr"
ms.tgt_pltfrm: ""
ms.topic: "reference"
apiname: 
  - "ICorDebugEval2.NewStringWithLength"
apilocation: 
  - "mscordbi.dll"
apitype: "COM"
f1_keywords: 
  - "ICorDebugEval2::NewStringWithLength"
dev_langs: 
  - "C++"
helpviewer_keywords: 
  - "NewStringWithLength method [.NET Framework debugging]"
  - "ICorDebugEval2::NewStringWithLength method [.NET Framework debugging]"
ms.assetid: d5f54a34-6335-4708-b407-a756ec70fab4
caps.latest.revision: 11
author: "rpetrusha"
ms.author: "ronpet"
manager: "wpickett"
---
# ICorDebugEval2::NewStringWithLength Method
Creates a string of the specified length, with the specified contents.  
  
## Syntax  
  
```  
HRESULT NewStringWithLength (  
    [in] LPCWSTR               string,  
    [in] UINT                  uiLength  
);  
```  
  
#### Parameters  
 `string`  
 [in] A pointer to the string value.  
  
 `uiLength`  
 [in] Length of the string.  
  
## Remarks  
 If the string's trailing null character is expected to be in the managed string, the caller of the `NewStringWithLength` method must ensure that the string length includes the trailing null character.  
  
 The string is always created in the application domain in which the thread is currently executing.  
  
## Requirements  
 **Platforms:** See [System Requirements](../../../../docs/framework/get-started/system-requirements.md).  
  
 **Header:** CorDebug.idl, CorDebug.h  
  
 **Library:** CorGuids.lib  
  
 **.NET Framework Versions:** [!INCLUDE[net_current_v20plus](../../../../includes/net-current-v20plus-md.md)]