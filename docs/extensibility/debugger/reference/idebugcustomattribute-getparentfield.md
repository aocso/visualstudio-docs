---
title: "IDebugCustomAttribute::GetParentField | Microsoft Docs"
ms.custom: ""
ms.date: "11/04/2016"
ms.technology: 
  - "vs-ide-sdk"
ms.topic: "conceptual"
f1_keywords: 
  - "IDebugCustomAttribute::GetParentField"
helpviewer_keywords: 
  - "IDebugCustomAttribute::GetParentField"
ms.assetid: bcdfdf37-bfcf-4988-a7b8-4c731d0af1b0
author: "gregvanl"
ms.author: "gregvanl"
manager: douge
ms.workload: 
  - "vssdk"
---
# IDebugCustomAttribute::GetParentField
Gets the field to which the custom attribute is attached.  
  
## Syntax  
  
```cpp  
HRESULT GetParentField(   
   IDebugField** ppField  
);  
```  
  
```csharp  
int GetParentField(  
   out IDebugField ppField  
);  
```  
  
#### Parameters  
 `ppField`  
 [out] Returns the [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) object that represents the field to which the custom attribute is attached.  
  
## Return Value  
 If successful, returns S_OK; otherwise, returns an error code.  
  
## Remarks  
 Call the [GetKind](../../../extensibility/debugger/reference/idebugfield-getkind.md) method on the returned [IDebugField](../../../extensibility/debugger/reference/idebugfield.md) object to determine what kind of field the parent is.  
  
## See Also  
 [IDebugCustomAttribute](../../../extensibility/debugger/reference/idebugcustomattribute.md)   
 [IDebugField](../../../extensibility/debugger/reference/idebugfield.md)