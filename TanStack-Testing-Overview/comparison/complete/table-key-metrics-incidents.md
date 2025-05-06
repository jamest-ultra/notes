# Table Documentation: [Key metrics]

## Page / Context
**Page:** [/standard#/report/manager/summary/breakdown]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property              | Description / Value                                                |
|-----------------------|--------------------------------------------------------------------|
| **Data Source**       | Rest API                                                      |
| **Pagination**        | Client-side (visible page selector and row limit dropdown)         |
| **Default Sorting**   | Yes — sorted by **Date** (descending)                              |
| **Filtering**         | No visible global or per-column filtering                          |
| **Search**            | Not present in this view                                           |
| **Column Visibility** | No — all columns are always shown                                  |
| **Table Actions**     | Download button visible in top-right corner                        |
| **Tool-tip Text**     | No                                                                 |
| **Icon Renders**      | Yes, Car crash icon                                                |
| **Styling**           | Fixed header, row hover highlighting, no zebra striping            |

---

## Column Definitions

| Column Label    | Document key       | Type     | Sortable | Filterable | Notes                                                  |
|-----------------|--------------------|----------|----------|------------|--------------------------------------------------------|
| Claim Reference | claim_reference_no | Text     | true     | false      | UUID-style identifier for the claim                    |
| Name            | driver_name        | Text     | true     | false      | Driver's full name                                     |
| Date            | position.datetime  | Date     | true     | false      | Date of the incident                                   |
| VRN             | vehicle_vrn        | Text     | true     | false      | Vehicle registration number                            |
| Fault Type      | fault_type         | Text     | true     | false      | e.g. Driver, Third Party                               |
| Cost            | total_net_cost     | Currency | true     | false      | Cost of the incident if known, displayed in £ GBP      |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [x] Pagination works the same way
- [x] Global and column search matches behaviour
- [x] Custom renders look/function correctly
- [x] Tool-tip text is correct
- [x] Styling and layout is consistent with legacy
- [x] Table is responsive and mobile-compatible
- [x] Loading, error, and empty states work properly
- [x] Accessibility (keyboard, ARIA roles) is preserved
- [x] Performance is acceptable for large datasets

---

## Notes / Known Issues

-
