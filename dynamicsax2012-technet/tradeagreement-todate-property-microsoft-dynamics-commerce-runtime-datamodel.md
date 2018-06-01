﻿---
title: TradeAgreement.ToDate Property  (Microsoft.Dynamics.Commerce.Runtime.DataModel)
TOCTitle: ToDate Property
ms:assetid: P:Microsoft.Dynamics.Commerce.Runtime.DataModel.TradeAgreement.ToDate
ms:mtpsurl: https://technet.microsoft.com/en-us/library/microsoft.dynamics.commerce.runtime.datamodel.tradeagreement.todate(v=AX.60)
ms:contentKeyID: 49834801
ms.date: 05/18/2015
mtps_version: v=AX.60
f1_keywords:
- Microsoft.Dynamics.Commerce.Runtime.DataModel.TradeAgreement.ToDate
dev_langs:
- CSharp
- C++
- VB
---

# ToDate Property

Gets the ending date when this rule becomes inactive.

**Namespace:**  [Microsoft.Dynamics.Commerce.Runtime.DataModel](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)  
**Assembly:**  Microsoft.Dynamics.Commerce.Runtime.Entities (in Microsoft.Dynamics.Commerce.Runtime.Entities.dll)

## Syntax

``` vb
'Declaration
<DataMemberAttribute> _
<ColumnAttribute("TODATE")> _
Public Property ToDate As DateTimeOffset
    Get
    Friend Set
'Usage
Dim instance As TradeAgreement
Dim value As DateTimeOffset

value = instance.ToDate
```

``` csharp
[DataMemberAttribute]
[ColumnAttribute("TODATE")]
public DateTimeOffset ToDate { get; internal set; }
```

``` c++
[DataMemberAttribute]
[ColumnAttribute(L"TODATE")]
public:
property DateTimeOffset ToDate {
    DateTimeOffset get ();
    internal: void set (DateTimeOffset value);
}
```

#### Property Value

Type: [System.DateTimeOffset](https://technet.microsoft.com/en-us/library/bb341783\(v=ax.60\))  
Returns [DateTime](https://technet.microsoft.com/en-us/library/03ybds8y\(v=ax.60\)).  

## See Also

#### Reference

[TradeAgreement Class](tradeagreement-class-microsoft-dynamics-commerce-runtime-datamodel.md)

[Microsoft.Dynamics.Commerce.Runtime.DataModel Namespace](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)
