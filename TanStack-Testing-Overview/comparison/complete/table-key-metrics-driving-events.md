# Table Documentation: [Driving Events]

## Page / Context
**Page:** [/standard#/report/manager/summary/breakdown/driver/summary/driving/events]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property              | Description / Value                                                  |
|-----------------------|----------------------------------------------------------------------|
| **Data Source**       | Rest API                                                        |
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

| Column Label | Document key      | Type       | Sortable | Filterable | Notes                                          |
|--------------|-------------------|------------|----------|------------|------------------------------------------------|
| Date         | position.datetime | DateTime   | true     | false      | Timestamp of the event                         |
| Location     | position.location | Text       | true     | false      | Not populated here — placeholder in table      |
| Event Type   | tds_event_type    | Text       | true     | false      | e.g., Braking, CorneringLeft                   |
| G-Force      | gforce_max        | Number     | true     | false      | Force measured in g; indicates event severity  |
| Speed        | speed_mph         | Number     | true     | false      | Speed in mph during the event                  |
| Severity     | severity          | Number     | true     | false      | Numeric value quantifying event intensity      |

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

- Table looks good but theres two tables renderd
