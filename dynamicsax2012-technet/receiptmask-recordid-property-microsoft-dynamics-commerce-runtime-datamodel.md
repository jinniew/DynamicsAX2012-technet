﻿---
title: ReceiptMask.RecordId Property  (Microsoft.Dynamics.Commerce.Runtime.DataModel)
TOCTitle: RecordId Property
ms:assetid: P:Microsoft.Dynamics.Commerce.Runtime.DataModel.ReceiptMask.RecordId
ms:mtpsurl: https://technet.microsoft.com/en-us/library/microsoft.dynamics.commerce.runtime.datamodel.receiptmask.recordid(v=AX.60)
ms:contentKeyID: 62214639
ms.date: 05/18/2015
mtps_version: v=AX.60
f1_keywords:
- Microsoft.Dynamics.Commerce.Runtime.DataModel.ReceiptMask.RecordId
dev_langs:
- CSharp
- C++
- VB
---

# RecordId Property

Gets the record identifier.

**Namespace:**  [Microsoft.Dynamics.Commerce.Runtime.DataModel](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)  
**Assembly:**  Microsoft.Dynamics.Commerce.Runtime.Entities (in Microsoft.Dynamics.Commerce.Runtime.Entities.dll)

## Syntax

``` vb
'Declaration
<DataMemberAttribute> _
<ColumnAttribute("RECID")> _
Public Property RecordId As Long
    Get
    Friend Set
'Usage
Dim instance As ReceiptMask
Dim value As Long

value = instance.RecordId
```

``` csharp
[DataMemberAttribute]
[ColumnAttribute("RECID")]
public long RecordId { get; internal set; }
```

``` c++
[DataMemberAttribute]
[ColumnAttribute(L"RECID")]
public:
property long long RecordId {
    long long get ();
    internal: void set (long long value);
}
```

#### Property Value

Type: [System.Int64](https://technet.microsoft.com/en-us/library/6yy583ek\(v=ax.60\))  
Returns [Int64](https://technet.microsoft.com/en-us/library/6yy583ek\(v=ax.60\)).  

## See Also

#### Reference

[ReceiptMask Class](receiptmask-class-microsoft-dynamics-commerce-runtime-datamodel.md)

[Microsoft.Dynamics.Commerce.Runtime.DataModel Namespace](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)
