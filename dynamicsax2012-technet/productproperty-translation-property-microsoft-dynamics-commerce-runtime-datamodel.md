﻿---
title: ProductProperty.Translation Property  (Microsoft.Dynamics.Commerce.Runtime.DataModel)
TOCTitle: Translation Property
ms:assetid: P:Microsoft.Dynamics.Commerce.Runtime.DataModel.ProductProperty.Translation
ms:mtpsurl: https://technet.microsoft.com/en-us/library/microsoft.dynamics.commerce.runtime.datamodel.productproperty.translation(v=AX.60)
ms:contentKeyID: 62209686
ms.date: 05/18/2015
mtps_version: v=AX.60
f1_keywords:
- Microsoft.Dynamics.Commerce.Runtime.DataModel.ProductProperty.Translation
dev_langs:
- CSharp
- C++
- VB
---

# Translation Property

Gets the language of this property's value, if text.

**Namespace:**  [Microsoft.Dynamics.Commerce.Runtime.DataModel](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)  
**Assembly:**  Microsoft.Dynamics.Commerce.Runtime.Entities (in Microsoft.Dynamics.Commerce.Runtime.Entities.dll)

## Syntax

``` vb
'Declaration
<DataMemberAttribute> _
<ColumnAttribute("TRANSLATION")> _
Public Property Translation As String
    Get
    Friend Set
'Usage
Dim instance As ProductProperty
Dim value As String

value = instance.Translation
```

``` csharp
[DataMemberAttribute]
[ColumnAttribute("TRANSLATION")]
public string Translation { get; internal set; }
```

``` c++
[DataMemberAttribute]
[ColumnAttribute(L"TRANSLATION")]
public:
property String^ Translation {
    String^ get ();
    internal: void set (String^ value);
}
```

#### Property Value

Type: [System.String](https://technet.microsoft.com/en-us/library/s1wwdcbf\(v=ax.60\))  
Returns [String](https://technet.microsoft.com/en-us/library/s1wwdcbf\(v=ax.60\)).  

## See Also

#### Reference

[ProductProperty Class](productproperty-class-microsoft-dynamics-commerce-runtime-datamodel.md)

[Microsoft.Dynamics.Commerce.Runtime.DataModel Namespace](microsoft-dynamics-commerce-runtime-datamodel-namespace.md)
