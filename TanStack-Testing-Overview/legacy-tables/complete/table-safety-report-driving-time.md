# Table Documentation: [Driving time]

## Page / Context
**Page:** [/standard#/report/manager/summary/safety]
**Status:** Phase 1
**Table Id:** [reporting.table.title.driving-time7]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (pagination controls shown: 10 per page) |
| **Default Sorting**  | Yes — Driving Time descending |
| **Filtering**        | None |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | Yes — “Table to show total driving time of all your drivers.” |
| **Icon Renders**     | Yes — Clock icon |
| **Styling**          | Clean modal, fixed header, responsive layout, pagination |

---

## Column Definitions

| Column Label         | Document key         | Type     | Sortable | Filterable | Notes                                                                 |
|----------------------|----------------------|----------|----------|------------|-----------------------------------------------------------------------|
| DRIVER NAME          | tds_entity_name      | Text     | Yes      | No         | Clickable link likely routes to more detailed driver view             |
| GROUP                | tds_group_name       | Text     | Yes      | No         | Driver's assigned group                                  |
| DRIVING TIME (H)     | driving_time_seconds | Duration | Yes      | No         | Shown as days, hours, and minutes (e.g., 1d 22h 3m)                    |
| DISTANCE (MILES)     | distance_driven_     | Number   | Yes      | No         | Total distance driven in miles (with “mi” suffix) with update when changing to KM |
| ULTRA SCORE          | ultra_score          | Number   | Yes      | No         | Performance score with colored indicator (Green = high, Orange = med) |

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
