# Table Documentation: [Unknown transactions]

## Page / Context
**Page:** [/standard#/report/manager/fuel-stats]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | local state |
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

| Column Label           | Document key | Type    | Sortable | Filterable | Notes                                                       |
|------------------------|--------------|---------|----------|------------|-------------------------------------------------------------|
| Date                   |              | Date    | true     | true       | Date of the transaction                                     |
| Licence Plate at Pump  |              | Text    | true     | true       | Entered or scanned licence plate at the pump                |
| Licence Plate on Card  |              | Text    | true     | true       | Plate registered on the fuel card                           |
| Brand                  |              | Text    | true     | true       | Fuel station brand (e.g., Shell, BP)                        |
| Quantity               |              | Number  | true     | true       | Amount of fuel dispensed                                    |
| Location               |              | Text    | true     | true       | Fuel station location                                       |
| Product                |              | Text    | true     | true       | Type of fuel (e.g., Diesel, Petrol, Electric)               |
| Provider               |              | Text    | true     | true       | Fuel card provider or fuel vendor                           |
| Price @ Pump           |              | Number  | true     | true       | Price per litre/kWh at pump                                 |
| Cost                   |              | Number  | true     | true       | Total cost of the transaction                               |

---

## Testing Checklist (Tan-stack Migration)

- [ ] All expected columns are present
- [ ] Column order and labels match legacy table
- [ ] Sorting works as before
- [ ] Filtering behaves as before (types, logic)
- [ ] Pagination works the same way
- [ ] Global and column search matches behaviour
- [ ] Custom renders look/function correctly
- [ ] Tool-tip text is correct
- [ ] Styling and layout is consistent with legacy
- [ ] Table is responsive and mobile-compatible
- [ ] Loading, error, and empty states work properly
- [ ] Accessibility (keyboard, ARIA roles) is preserved
- [ ] Performance is acceptable for large datasets

---

## Notes / Known Issues

Add any relevant notes or known bugs here.
