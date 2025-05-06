# Table Documentation: [Speeding events]

## Page / Context
**Page:** [/standard#/report/manager/summary/safety]
**Status:** Phase 1
**Table Id:** [reporting.table.title.events-speeding]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
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

| Column Label     | Document key         | Type     | Sortable | Filterable | Notes                                                             |
|------------------|----------------------|----------|----------|------------|-------------------------------------------------------------------|
| DRIVER NAME      | tds_entity_name      | Text     | Yes      | No         | clickable down to driver details                                 |
| GROUP            | tds_group_name       | Text     | Yes      | No         | Driver's assigned group                                         |
| EVENTS           | speeding_events      | Number   | Yes      | No         | Total number of speeding events recorded                          |
| PER 1,000 MILES  | speeding_eventsper1k | Number   | Yes      | No         | Normalized event count by mileage, useful for risk normalization  |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [ ] Pagination works the same way
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

Add any relevant notes or known bugs here.
