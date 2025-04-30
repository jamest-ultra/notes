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

| Column Label    | Document key | Type     | Sortable | Filterable | Notes                                                  |
|-----------------|--------------|----------|----------|------------|--------------------------------------------------------|
| Claim Reference |              | Text     | true     | false      | UUID-style identifier for the claim                    |
| Name            |              | Text     | true     | false      | Driver's full name                                     |
| Date            |              | Date     | true     | false      | Date of the incident                                   |
| VRN             |              | Text     | true     | false      | Vehicle registration number                            |
| Fault Type      |              | Text     | true     | false      | e.g. Driver, Third Party                               |
| Cost            |              | Currency | true     | false      | Cost of the incident if known, displayed in £ GBP      |

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
