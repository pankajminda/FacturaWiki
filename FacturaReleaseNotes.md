# Factura Release Notes

### 22-04-2019
-in stk jrnl/mfg jrnl if alt-c create project then both combos do not refresh

* Fixed : `Receipt & Payments` report removed multi currency calculation
* Fixed : `Receipt & Payments` report drill down to `Ledger Monthly Summary` and `Daybook` will exclude forex calculation

### 21-04-2019
* Fixed : Effective date is now used in voucher for calculating due date in billwise window
* Fixed : Forex calculation in (BS, P&L, TB, Daybook, Forex Gain Loss)
* Fixed : `Item Monthly Summary` report Opening is now show separatly
* Fixed : `Stock Summary` report in mid period closing and opening was not shown correct. Fixed (New Adjust Quantities, Logic of Stock Summary, P&L, BS, Item Monthly Summary)
* Fixed : `Receipt & Payments` report speed issue
* Added : `Statistics` report date customize option
* Fixed : `SmartList`>`Negative Stock` report split qty and unit in separate columns
* Added : `Smartlist`>`Stock Item` show costing method
* Fixed : `SmartList`>`Audit Trail` Modified Date column not showing data

### 22-01-2019
* Fixed : `Physical Stock Worksheet` was not opening in single user company
* Fixed : Negative stock error message now displayed in web edition from Item Allocation window

### 23-01-2019
* Added : In Ledger Vouchers Report customize window added option `Show Line Balance`

### 04-12-2018
* Fixed : In party details window if order no. was entered manually then next time when tab was press from order no. field date would change to voucher date

### 23-11-2018
* Added : New keyword in `Cheque` printing `[DATE_DAY]`,`[DATE_MONTH]`,`[DATE_YEAR]`

### 13-11-2018
* Added : New keyword in `Sales Invoice` printing `[INVOICE_DUE_DATE]`, will display the Credit Period (1st Billwise due date)
* Added : Plugins for Workflow Engine can be written
* Fixed : Barcode printing in both Laser and thermal has been tested and working fine

### 30-07-2018
* Fixed : In `Godown` Master, for `Main Location` `Allow storage of materials` option could not be unchecked
* Added : In `Sales/Purchase Bill Pending` report added option to sort by party name

### 30-06-2018
* Fixed : UDF entry screen size increased to avoid labels wrapping

### 27-06-2018
* Fixed : In reports for `Forex Unadjusted Gain/Loss` calculation `Contra` vouchers were not being considered
* Fixed : Voucher printing for Jrnl/Ctra/Reversing_Journal/Memorandum was not showing currency excange rate in case of forex transaction
* Fixed : In voucher printing for Pymt/Rcpt where there were multiple Cr in Pymt or Dr in Rcpt and PaymentModeTop/RcptModeTop was true, the ledgers were not shown

### 24-06-2018
* Fixed : Voucher Class does not show in voucher edit mode.
* Added : Voucher Type `Import Purchase Vat` is now excluded in VAT Reports for UAE
* Added : In `Quick Payment/Receipt` now filters text by contains
* Fixed : In `Ledger` master when address is added, now gets linked to Billing/Shipping/Statement automatically

### 12-06-2018
* Fixed : `Forex/Gain Loss` report should show only those ledgers whose currency is not set as base currency.

### 08-06-2018
* Added : `Purchase Vouchers` report in `SmartList`

### 07-06-2018
* Added : in `Ledger Address` multi edit screen, now can add new address for existing ledgers

### 18-05-2018
* Added : in `Budget` master added `Import from Excel` option
* Fixed : in `Budget` master exported excel file did not have extension
* Added : in `Price List` master added `Import from Excel` option

### 09-05-2018
* Added : in `Stock Summary - Pivot` report added new view `Company` to see multiple companies data in same report

### 22-04-2018
* Added : New Multi-Address editing screen in Masters Gallery
* Added : In Multi-Edit mode added option to Export data and Group by columns
* Fixed : In Purchase preview the VAT no. was shown wrong in the footer

### 07-04-2018
* Added : User can select exported file path when exporting Reports to Excel
* Fixed : `rowheight` attribute on `tr` element in voucher printing template can be used for setting the height of rows

### 05-04-2018
* Added : New keywords in `Sales` `Invoice` printing `[PARTY_CURRENT_BALANCE_IN_WORDS]`,`[PARTY_BALANCE_PREV_DAY_IN_WORDS]` and `[ADVANCE_PENDING_AMOUNT_IN_WORDS]`

### 02-04-2018
* Added : New keywords in `Invoice` printing for `GST` for Ledger row `[GST_TAXABLE_AMOUNT]`
  
### 27-03-2018
* Added : New keywords in `Sales` `Invoice` printing for feature "Advance Received against Invoice" `[ADVANCE_RCVD_AMOUNT]` and `[ADVANCE_PENDING_AMOUNT]`

### 25-03-2018
* Added : In `Vat Classification` report `City` column added for UAE

### 19-03-2018
* Added : New keyword `[SUPPLIER_ITEM_NAME]` added to item row for invoice printing
* Fixed : On exporting Smartlist to Excel, $ sign was being displayed
* Fixed : Document Expiry Plugin will get activated only when Expiry Date is set for the attachment
* Fixed : `Project` Master in single user edition was not saving
* Fixed : Multiuser - Ledger Name can now be entered in non-english characters
* Fixed : Multiuser - Stock Item Name, Part Number, Remarks, Description, Supplier Item Name can now be entered in non-english characters

### 17-03-2018
* Added : In `Stock Item` master Project wise opening stock can be entered. Also included in stock item master xml export and import. **Note: Godown or Batch must be `On` for the item for Project allocation.**

### 05-03-2018
* Fixed : In `Daybook` report Currency symbol can be entered in customize dialog to view report in any currency of choice

### 21-02-2018
* Added : In `Invoice` data entry screen Party combo now shows `Credit Limit` in tooltip after pressing tab
* Fixed : In `Columnar Register` Customize window was not showing controls
* Fixed : In `Project` Master `Project Value` field was limited to maximum length of 4

### 07-02-2018
* Added : New column `Stock Group Name` and `Date` in `Smartlist`->`Sales by Customer` report

### 31-01-2018
* Fixed : Page Up/Down in `Additional Cost of Purchase` will loop through all `Additional Cost of Purchase` entries now.
* Added : New column `Entry Type` in `Smartlist`->`Vouchers` report, will help find all `Additional Cost of Purchase` entries
* Added : Drilldown from `Smartlist`->`Vouchers` report for `Additional Cost of Purchase` entries will now open the `Additional Cost of Purchase` screen
* Added : Now can delete `Additional Cost of Purchase` entries and automatically reversing its costing effect.
* Fixed : All Reports->Customize window now show the list of Ledgers/Stock Items much faster, earlier used to take time in opening
* Added : New field `Project Value` in Project master
* Added : In `Project Analysis`report `Project Value` is displayed next to date in header

### 20-01-2018
* Fixed : Fix for negative stock calculation when multiple years in a single company
* Fixed : In continuous numbering method when voucher was modified sometimes the voucher no. changed
* Fixed : Password in the database are now encrypted

### 30-12-2017
* Fixed : Restore Deleted Data : Only Admin can Clear/Restore any Masters/Vocuhers (Web/Desktop)

### 21-12-2017
* Added : New keywords in `Invoice` printing for `GST`
  [AMOUNT_WITH_GST]
* Fixed : Track user login attempts from desktop/web along with ipaddress
* Fixed : Track failed login attempts with ipaddress
* Fixed : Continuous Voucher Numbering, in some case was repeating

### 18-12-2017
* Added : Enabled VAT for UAE
* Fixed : Report `One Account` Opening balance date was wrongly displayed when mentod of balancing was set to `Daily`
* Added : Report `Bills Receivables` option to sort by `Party`, `Ref. No.`, `Date`
* Fixed : Report `Bills Receivables` option to set aging period 

### 29-11-2017
* Added : In Body only printing templates now can print image in header/footer. eg.
```
<tr name="header">
    <td valign="middle" colspan="5" align="center">[IMAGE'maxside|145|E:\logo.png']</td>
</tr>
```
* Updated : Reorder Status Report was causing OutOfMemory in Suruchi data in homepage, now uses the StockSummary for closing calculation.
* Fixed : Journal vouchers unable to preview.

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
