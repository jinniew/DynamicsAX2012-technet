﻿---
title: PricingDataManager.GetDiscountCodesByOfferId Method  (Microsoft.Dynamics.Commerce.Runtime.Data)
TOCTitle: GetDiscountCodesByOfferId Method
ms:assetid: M:Microsoft.Dynamics.Commerce.Runtime.Data.PricingDataManager.GetDiscountCodesByOfferId(System.Collections.Generic.IEnumerable{System.String},Microsoft.Dynamics.Commerce.Runtime.ColumnSet)
ms:mtpsurl: https://technet.microsoft.com/en-us/library/microsoft.dynamics.commerce.runtime.data.pricingdatamanager.getdiscountcodesbyofferid(v=AX.60)
ms:contentKeyID: 49851124
ms.date: 05/18/2015
mtps_version: v=AX.60
f1_keywords:
- Microsoft.Dynamics.Commerce.Runtime.Data.PricingDataManager.GetDiscountCodesByOfferId
dev_langs:
- CSharp
- C++
- VB
---

# GetDiscountCodesByOfferId Method

Get the discount codes (aka 'promo codes') associated with the given discount offer identifiers.

**Namespace:**  [Microsoft.Dynamics.Commerce.Runtime.Data](microsoft-dynamics-commerce-runtime-data-namespace.md)  
**Assembly:**  Microsoft.Dynamics.Commerce.Runtime.DataManagers (in Microsoft.Dynamics.Commerce.Runtime.DataManagers.dll)

## Syntax

``` vb
'Declaration
Public Function GetDiscountCodesByOfferId ( _
    offerIds As IEnumerable(Of String), _
    columns As ColumnSet _
) As ReadOnlyCollection(Of DiscountCode)
'Usage
Dim instance As PricingDataManager
Dim offerIds As IEnumerable(Of String)
Dim columns As ColumnSet
Dim returnValue As ReadOnlyCollection(Of DiscountCode)

returnValue = instance.GetDiscountCodesByOfferId(offerIds, _
    columns)
```

``` csharp
public ReadOnlyCollection<DiscountCode> GetDiscountCodesByOfferId(
    IEnumerable<string> offerIds,
    ColumnSet columns
)
```

``` c++
public:
virtual ReadOnlyCollection<DiscountCode^>^ GetDiscountCodesByOfferId(
    IEnumerable<String^>^ offerIds, 
    ColumnSet^ columns
) sealed
```

#### Parameters

  - offerIds  
    Type: [System.Collections.Generic.IEnumerable](https://technet.microsoft.com/en-us/library/9eekhta0\(v=ax.60\))\<[String](https://technet.microsoft.com/en-us/library/s1wwdcbf\(v=ax.60\))\>  

<!-- end list -->

  - columns  
    Type: [Microsoft.Dynamics.Commerce.Runtime.ColumnSet](columnset-class-microsoft-dynamics-commerce-runtime.md)  

#### Return Value

Type: [System.Collections.ObjectModel.ReadOnlyCollection](https://technet.microsoft.com/en-us/library/ms132474\(v=ax.60\))\<[DiscountCode](discountcode-class-microsoft-dynamics-commerce-runtime-datamodel.md)\>  
Discounts codes found for given offers. Empty if none found.  

#### Implements

[IPricingDataManager.GetDiscountCodesByOfferId(IEnumerable\<String\>, ColumnSet)](ipricingdatamanager-getdiscountcodesbyofferid-method-microsoft-dynamics-commerce-runtime-data.md)  

## See Also

#### Reference

[PricingDataManager Class](pricingdatamanager-class-microsoft-dynamics-commerce-runtime-data.md)

[Microsoft.Dynamics.Commerce.Runtime.Data Namespace](microsoft-dynamics-commerce-runtime-data-namespace.md)
