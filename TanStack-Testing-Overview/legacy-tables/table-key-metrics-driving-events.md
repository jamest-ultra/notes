# Table Documentation: [Driving Events]

## Page / Context
**Page:** [/standard#/report/manager/summary/breakdown/driver/summary/driving/events]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property              | Description / Value                                                  |
|-----------------------|----------------------------------------------------------------------|
| **Data Source**       | Local Storage                                                        |
| **Pagination**        | Client-side (10 rows per page, paginator at bottom)                  |
| **Default Sorting**   | Yes — sorted by Date (descending)                                    |
| **Filtering**         | No                                                                   |
| **Search**            | No                                                                   |
| **Column Visibility** | No                                                                   |
| **Table Actions**     | No Download                                                          |
| **Tool-tip Text**     | No                                                                   |
| **Icon Renders**      | Yes - Car with a tilt icon                                           |
| **Styling**           | Fixed header, row hover state, no zebra striping                     |

---

## Column Definitions

| Column Label | Document key | Type       | Sortable | Filterable | Notes                                          |
|--------------|--------------|------------|----------|------------|------------------------------------------------|
| Date         |              | DateTime   | true     | false      | Timestamp of the event                         |
| Location     |              | Text       | true     | false      | Not populated here — placeholder in table      |
| Event Type   |              | Text       | true     | false      | e.g., Braking, CorneringLeft                   |
| G-Force      |              | Number     | true     | false      | Force measured in g; indicates event severity  |
| Speed        |              | Number     | true     | false      | Speed in mph during the event                  |
| Severity     |              | Number     | true     | false      | Numeric value quantifying event intensity      |

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
