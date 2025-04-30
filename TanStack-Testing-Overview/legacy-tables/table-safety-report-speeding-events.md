# Table Documentation: [Speeding events]

## Page / Context
**Page:** [/standard#/report/manager/summary/safety]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Backend |
| **Pagination**       | Client-side (pagination present: 10 per page) |
| **Default Sorting**  | Yes — Events descending |
| **Filtering**        | None shown |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | Yes — Tooltip reads: “List of drivers’ speeding events from telematic data. Click on the name or event to see more information.” |
| **Icon Renders**     | Yes — Speeding Van |
| **Styling**          | Clean UI, fixed headers, pagination at bottom |

---

## Column Definitions

| Column Label     | Document key       | Type     | Sortable | Filterable | Notes                                                             |
|------------------|--------------------|----------|----------|------------|-------------------------------------------------------------------|
| DRIVER NAME      |                    | Text     | Yes      | No         | clickable down to driver details                                 |
| GROUP            |                    | Text     | Yes      | No         | Driver's assigned group                                         |
| EVENTS           |                    | Number   | Yes      | No         | Total number of speeding events recorded                          |
| PER 1,000 MILES  |                    | Number   | Yes      | No         | Normalized event count by mileage, useful for risk normalization  |

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
