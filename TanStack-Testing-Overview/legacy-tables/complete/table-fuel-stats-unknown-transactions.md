# Table Documentation: [Unknown transactions]

## Page / Context
**Page:** [/standard#/report/manager/fuel-stats]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Transactions, Decending |
| **Filtering**        | Global |
| **Search**           | Yes, For the VRN |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Checklist |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label           | Document key      | Type    | Sortable | Filterable | Notes                                                       |
|------------------------|-------------------|---------|----------|------------|-------------------------------------------------------------|
| Date                   | tn_dt             | Date    | true     | true       | Date of the transaction                                     |
| Licence Plate at Pump  | pump_vrn          | Text    | true     | true       | Entered or scanned licence plate at the pump                |
| Licence Plate on Card  | card_vrn          | Text    | true     | true       | Plate registered on the fuel card                           |
| Quantity               | tn_quantity       | Number  | true     | true       | Amount of fuel dispensed                                    |
| Brand                  | brand             | Text    | true     | true       | Fuel station brand (e.g., Shell, BP)                        |
| Location               | site_address      | Text    | true     | true       | Fuel station location                                       |
| Product                | tds_fuel_product  | Text    | true     | true       | Type of fuel (e.g., Diesel, Petrol, Electric)               |
| Provider               | tds_supplier_name | Text    | true     | true       | Fuel card provider or fuel vendor                           |
| Price @ Pump           | tn_net_unit_price | Number  | true     | true       | Price per litre/kWh at pump                                 |
| Cost                   | tn_net_cost       | Number  | true     | true       | Total cost of the transaction                               |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [x] Pagination works the same way
- [x] Global and column search matches behaviour
- [ ] Custom renders look/function correctly
- [x] Tool-tip text is correct
- [x] Styling and layout is consistent with legacy
- [x] Table is responsive and mobile-compatible
- [x] Loading, error, and empty states work properly
- [x] Accessibility (keyboard, ARIA roles) is preserved
- [x] Performance is acceptable for large datasets

---

## Notes / Known Issues

- The table icons is different
- When no data loaded there isn't a large piece of test saying "No data available"
