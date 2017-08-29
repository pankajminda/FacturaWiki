# Factura Release Notes


### 28-08-2017
* In Stk Jrnl printing can now configure the stock item name print format.
  In `TPP.ini` file add the following key : `StkJrnlPrintItemNameFormat = {ItemName}-{PartNumber}`
* In Purchase Invoice Edit Mode pressing `Ctrl+Alt+A`  toggles additional cost completed flag
* Additional cost can now be enetered in base currency when the purchase is in another currency.
  Select the checkbox `Expense in base currency`
* New report added `Purchase Item Analysis` in Smartlist. Shows the total additional cost linked to an invoice with effective rate.

## 23-08-2017
* In all master screens the selection dropdown now allows 'contains' filtering

## 16-08-2017
* Added Indian GST calculation support
