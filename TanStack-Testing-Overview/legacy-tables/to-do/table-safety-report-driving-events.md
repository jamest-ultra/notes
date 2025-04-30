# Table Documentation: [Driving events]

## Page / Context
**Page:** [/standard#/report/manager/summary/safety]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (pagination visible at bottom: 10 per page) |
| **Default Sorting**  | Yes — Driving Events descending |
| **Filtering**        | None |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | Yes — Tooltip reads: “List of drivers' speeding events from telematic data. Click on the name or event to see more information.” |
| **Icon Renders**     | Yes — Tilt Car |
| **Styling**          | Fixed headers, responsive layout, clean modal styling with pagination controls |

---

## Column Definitions

| Column Label     | Document key       | Type     | Sortable | Filterable | Notes                                                            |
|------------------|--------------------|----------|----------|------------|------------------------------------------------------------------|
| DRIVER NAME      |                    | Text     | Yes      | No         | Clickable link to drill down into driver detail or event         |
| GROUP            |                    | Text     | Yes      | No         | Driver's assigned group                                       |
| DRIVING EVENTS   |                    | Number   | Yes      | No         | Total count of relevant driving events |
| PER 1,000 MILES  |                    | Number   | Yes      | No         | Normalized events count by distance                             |
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
