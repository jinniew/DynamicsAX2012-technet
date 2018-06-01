﻿---
title: PaymentCardBase.CardTypes Property  (Microsoft.Dynamics.Commerce.Runtime.DataModel)
TOCTitle: CardTypes Property
ms:assetid: P:Microsoft.Dynamics.Commerce.Runtime.DataModel.PaymentCardBase.CardTypes
ms:mtpsurl: https://technet.microsoft.com/en-us/library/microsoft.dynamics.commerce.runtime.datamodel.paymentcardbase.cardtypes(v=AX.60)
ms:contentKeyID: 65316221
ms.date: 05/18/2015
mtps_version: v=AX.60
f1_keywords:
- Microsoft.Dynamics.Commerce.Runtime.DataModel.PaymentCardBase.CardTypes
dev_langs:
- CSharp
- C++
- VB
---

# CardTypes Property

Gets or sets the value for CardTypes.

**Namespace:**  [Microsoft.Dynamics.Commerce.Runtime.DataModel](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)  
**Assembly:**  Microsoft.Dynamics.Commerce.Runtime.Entities (in Microsoft.Dynamics.Commerce.Runtime.Entities.dll)

## Syntax

``` vb
'Declaration
<IgnoreDataMemberAttribute> _
Public Property CardTypes As String
    Get
    Set
'Usage
Dim instance As PaymentCardBase
Dim value As String

value = instance.CardTypes

instance.CardTypes = value
```

``` csharp
[IgnoreDataMemberAttribute]
public string CardTypes { get; set; }
```

``` c++
[IgnoreDataMemberAttribute]
public:
property String^ CardTypes {
    String^ get ();
    void set (String^ value);
}
```

#### Property Value

Type: [System.String](https://technet.microsoft.com/en-us/library/s1wwdcbf\(v=ax.60\))  
The card types.  

## See Also

#### Reference

[PaymentCardBase Class](paymentcardbase-class-microsoft-dynamics-commerce-runtime-datamodel.md)

[Microsoft.Dynamics.Commerce.Runtime.DataModel Namespace](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)
