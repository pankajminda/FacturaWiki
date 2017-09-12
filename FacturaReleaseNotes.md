# Factura Release Notes

### 12-09-2017
* Added : New Report Smartlist->`Stock Summary by HSN Code`
* Added : New field in Ledger Master : GSTRegistrationType
* Added : New `Reference No.` field in `Additional Cost of Purchase`
* Changed : For `RR Busduct` in `Additional Cost of Purchase` billwise will always post `Agst Ref`
* Fixed : In Group Master, auto filter did not work in sub group field
* Fixed : In `Additional Cost of Purchase`, auto filter did not work in ledger fields
* Added : In `Columnar Register` added column `Registration Type`

### 11-09-2017
* Fixed : Additional Cost entries could not be deleted
* Fixed : In Additional Cost entries when expense was enetered in base currency and invoice in diff. currency then total amount was shown in wrong currency

### 08-09-2017
* Fixed : When transactions were going for WF, there balances would reflect in Trial Balance even though they are optional

### 07-09-2017
* Fixed : In StockSummary report alternate units display
* Added : `[CURRENCY_SYMBOL]` and `[CURRENCY_FORMALNAME]` keywords for invoice header/footer printing

### 06-09-2017
* Added default Billwise allocaton for Additional Cost journals

### 28-08-2017
* In Stk Jrnl printing can now configure the stock item name print format.
  In `TPP.ini` file add the following key : `StkJrnlPrintItemNameFormat = {ItemName}-{PartNumber}`
* In Purchase Invoice Edit Mode pressing `Ctrl+Alt+A`  toggles additional cost completed flag
* Additional cost can now be entered in base currency when the purchase is in another currency.
  Select the checkbox `Expense in base currency`
* Added : New report added `Purchase Item Analysis` in Smartlist. Shows the total additional cost linked to an invoice with effective rate.

### 23-08-2017
* In all master screens the selection dropdown now allows `contains` filtering

### 16-08-2017
* Added: Indian GST calculation support
