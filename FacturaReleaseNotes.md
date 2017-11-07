# Factura Release Notes

### 07-11-2017
* Updated : Plugin : Report `SmartList`->`Custom`->`Negative Stock`. Date column now in `dd-MMM-yyyy` format.
* Updated : Plugin : Report `SmartList`->`Custom`->`Negative Stock`. Drilldown to Stock Vouchers report for quick details view.
* Fixed : `Export to Excel` option in `Price List` was not working.
* Fixed : Stock Valuation opening calculation time reduced upto 1/3rd when start date of report is greater than Financial Period.

### 31-10-2017
* Added : Plugin : Report `SmartList`->`Stock Item Project Budget`. Budget can be compared with `Inward Qty` or `Inward Amount` fields.

### 28-10-2017
* Added : Plugin : Report `SmartList`->`Custom`->`Negative Stock`. This report will show all items which have gone negative on any date within the financial period.

### 12-10-2017
* Added : AutoRestore.exe to allow automatic restore of database from Dropbox. For 1 way sync where internet is slow for syncronization.

### 11-10-2017
* Fixed : Auto Column in P&L was producing columns with wrong date ranges

### 04-10-2017
* Added : New keywords in `Invoice` printing for `GST`
  [IGST]
  [SGST]
  [CGST]
  [IGST_AMOUNT]
  [SGST_AMOUNT]
  [CGST_AMOUNT]

### 17-09-2017
* Fixed : `StockItem` was not saving
* Fixed : `GST` tab in `StockItem` will now show only if GST is enabled in TPP.ini file
* Fixed : In double entry voucher mode attachment were not saving in edit mode

### 16-09-2017
* Added : New fields in `Ledger` master for `Attachment`: `DocumentName`, `DocumentNo`, `ExpiryDate`
* Ctrl + Y in party selection drowdown will open Ledger History report
* Ctrl + N in party selection drowdown will show Ledger Notes
* Ctrl + T in party selection drowdown will show Ledger Attachments

### 12-09-2017
* Added : New Report Smartlist->`Stock Summary by HSN Code`
* Added : New field in Ledger Master : GSTRegistrationType
* Added : New `Reference No.` field in `Additional Cost of Purchase`
* Changed : For `RR Busduct` in `Additional Cost of Purchase` billwise will always post `Agst Ref`
* Fixed : In Group Master and others, auto filter did not work in dropdown fields
* Fixed : In `Additional Cost of Purchase`, auto filter did not work in ledger fields
* Added : In `Columnar Register` added column `Registration Type`
* Fixed : Drilldown from `Stock item with Image` report

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
