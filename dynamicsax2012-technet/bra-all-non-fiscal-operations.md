﻿---
title: (BRA) All non fiscal operations
TOCTitle: (BRA) All non fiscal operations
ms:assetid: 8ce32ee3-fe3c-4faf-b6a3-dd13443cd507
ms:mtpsurl: https://technet.microsoft.com/en-us/library/Dn600278(v=AX.60)
ms:contentKeyID: 62200242
ms.date: 05/02/2014
mtps_version: v=AX.60
f1_keywords:
- non fiscal
- forms.FBNonFiscalOperation_BR
- SPED EFD
---

# (BRA) All non fiscal operations 


_**Applies To:** Microsoft Dynamics AX 2012 R3_

This topic explains how to create non fiscal document transactions to be included in the Sistema Publico de Escrituração Digital Escrituracao Fiscal Digital (SPED EFD) text file.

The SPED EFD contributions text files are generated by legal entities that already have the obligation to issue Accounting and Fiscal SPED. The text files provide information about transactions that represent the Programa de Integração Social (PIS) and Contribuição para o Financiamento da Seguridade Social (COFINS) taxable and non-taxable revenue, and the cost or expenses with credit of PIS and COFINS. Operations that are not related to fiscal documents, such as rent, or revenue or expenses that are related to operations, must be included in record F100 of the text file.

## Set up a sales tax code to calculate PIS and COFINS tax amounts

You must set up sales tax codes to calculate PIS and COFINS tax amounts to be included in record F100.

To set up the sales tax codes, follow these steps:

1.  Click **General ledger** \> **Setup** \> **Sales tax** \> **Sales tax codes**.

2.  Click **New** to create a sales tax code. For more information, see [Set up and use sales tax codes](set-up-and-use-sales-tax-codes.md).

3.  In the **Settlement period** field, select a settlement period for PIS.

4.  On the **Calculation** FastTab, in the **Origin** field, select **Percentage of net amount**.

5.  In the **Tax type** field, select **PIS**.

6.  Click **Values** to open the **Values** form. In the **Value** field, enter the tax value.

7.  Click **Close**.

8.  Repeat steps 2 through 7 for COFINS.

## Set up a sales tax group

Sales tax groups are groups of sales tax codes that are attached to customers and vendors. They are also attached to ledger accounts for transactions that are not posted to a particular vendor or customer. You must set up a sales tax group to calculate PIS and COFINS tax amounts in general ledger transactions.

To set up sales tax groups for PIS and COFINS tax, follow these steps:

1.  Click **General ledger** \> **Setup** \> **Sales tax** \> **Sales tax groups**.

2.  Click **New** to create a sales tax group for PIS and COFINS tax.

3.  Enter the identifier and a description of the sales tax group. For more information, see [Sales tax codes (form)](https://technet.microsoft.com/en-us/library/aa553257\(v=ax.60\)).

4.  On the **Setup** FastTab, in the **Sales tax code** field, select the sales tax code that represents PIS tax.

5.  Repeat steps 2 through 4 for COFINS tax.

## Set up an item sales tax group

You must set up item sales tax groups to calculate PIS and COFINS tax amounts in general ledger transactions.

To set up item sales tax groups for PIS and COFINS tax, follow these steps:

1.  Click **General ledger** \> **Setup** \> **Sales tax** \> **Item sales tax groups**.

2.  Click **New** to create an item withholding tax group for PIS tax in revenue transactions.

3.  In the **Item sales tax group** field, enter a unique identifier for the item sales tax group. For more information, see [Create item sales tax groups](create-item-sales-tax-groups.md).

4.  On the **Setup** FastTab, in the **Sales tax code** field, select a PIS sales tax code.

5.  In the **Taxation code** field, enter a tax value to use for revenue transactions.

6.  Repeat steps 2 through 5 for the COFINS tax.

7.  Repeat steps 2 through 6 to create an item tax group for expense transactions.

## Create and post non fiscal document revenue transactions

You can create general journal transactions to register specific revenues that include PIS and COFINS tax amounts.

To create and post transactions for non fiscal document revenues, follow these steps:

1.  Click **General ledger** \> **Journals** \> **General journal**.

2.  Click **New** to create a line.

3.  In the **Name** field, select a journal name.

4.  Click **Lines** to open the **Journal voucher** form. Some fields might display default values from the **Journal** form.

5.  In the **Account type** field, select **Ledger**.

6.  Select the main account and the fiscal establishment of revenue.

7.  Enter a description and the credit amount.

8.  In the **Sales tax group** field, select the sales tax group for PIS or COFINS.

9.  In the **Item sales tax group** field, select the item sales tax group for PIS or COFINS.
    
    Click **Sales tax** to verify that PIS or COFINS tax is included in the sales tax calculation, and that the **Taxation code** values are correct. Click **Close**.

10. Click **New** to create a second line.

11. In the **Account type** field, select **Customer**.

12. In the **Account** field, select the customer account.

13. Enter a description and a debit amount.

14. Click **Validate**.

15. Click **Post**.

## Create and post non fiscal document expense transactions

You can create general journal transaction to register specific expenses that include PIS and COFINS tax amounts.

To create and post transactions for non fiscal document expenses, follow these steps:

1.  Click **General ledger** \> **Journals** \> **General journal**.

2.  Click **New** to create a line.

3.  In the **Name** field, select a journal name.

4.  Click **Lines** to open the **Journal voucher** form. Some fields might display default values from the **Journal** form.

5.  In the **Account type** field, select **Ledger**.

6.  Select the main account and the fiscal establishment of expense.

7.  Enter a description and the debit amount.

8.  In the **Sales tax group** field, select the sales tax group for PIS or COFINS.

9.  In the **Item sales tax group** field, select the item sales tax group for PIS or COFINS.
    
    Click **Sales tax** to verify that PIS or COFINS tax is included in the sales tax calculation, and that the **Taxation code** values are correct.

10. Click **New** to create a second line.

11. In the **Account type** field, select **Vendor**.

12. In the **Account** field, select the vendor account.

13. Enter a description and a credit amount.

14. Click **Validate**.

15. Click **Post**.

## Register non fiscal document operations

To register non fiscal document operations, follow these steps:

1.  Click **Fiscal books** \> **Common** \> **All non fiscal operations**.

2.  Click **New** to create a non fiscal document operation for transactions that are posted to the general ledger but that do not have tax specified.
    
    You can also see the non fiscal operations that were created manually or by using the **General journal** form.

3.  On the **Details** FastTab, in the **Fiscal establishment ID** field, select a fiscal establishment.

4.  Enter a posting date.

5.  In the **Account type** field, select **Vendor**.

6.  In the **Account** field, select the vendor account.

7.  Enter a description and an amount.

8.  In the **Offset account** field, select the expense account.

9.  In the **Cost center** field, select the related cost center.

10. Select the credit source code.

11. On the **Tax transactions** FastTab, click **Add line** to create PIS and COFINS lines.

12. In the **Tax type** field, select either **PIS** or **COFINS**.

13. In the **Taxation code** field, enter a value between 50 and 99.

14. In the **Sales tax rate** field, enter a value between 1.65 and 7.65.

15. Close the form.

16. To create record F100 in the SPED EFD contribution file, the booking period must be synced. Click **Fiscal books** \> **Common** \> **Booking period**.

17. Click **Sync**, and then click **OK.** This synchronizes all fiscal and non fiscal documents.

18. On the **Booking period** list page, click **Non fiscal operations** to confirm that all non fiscal document transactions were created for the specified booking period and fiscal establishment.

## See also

[(BRA) Generate the SPED fiscal export file for a month](bra-generate-the-sped-fiscal-export-file-for-a-month.md)

  
**Announcements:** To see known issues and recent fixes, use [Issue search](http://go.microsoft.com/fwlink/?linkid=389258) in [Microsoft Dynamics Lifecycle Services](http://go.microsoft.com/fwlink/?linkid=306505) (LCS).
