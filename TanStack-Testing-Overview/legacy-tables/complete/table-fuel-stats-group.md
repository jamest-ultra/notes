# Table Documentation: [Fuel stats - Group]

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

| Column Label    | Document key     | Type     | Sortable | Filterable | Notes                                        |
|-----------------|------------------|----------|----------|------------|----------------------------------------------|
| LICENCE PLATE   | tds_entity_name  | Text     | Yes      | No         | Vehicle registration number                  |
| TRANSACTIONS    | fuel_tn_count    | Number   | Yes      | No         | Able to drip into the transactions           |
| LITRES          | ice_litres       | Number   | Yes      | No         | Fuel dispensed (L)                           |
| KWH             | kwh              | Number   | Yes      | No         | Energy equivalent (if EV hybrid)             |
| KG              | hydrogen_kg      | Number   | Yes      | No         | Likely CO₂ equivalent weight                 |
| COST            | tn_net_cost      | Currency | Yes      | No         | Monetary cost — shown as “-”                 |

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

- The Licence Plate column is called Group
- The table icons is different
