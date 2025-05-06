# Table Documentation: [Risk Summary]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes — Speeding Offences Score ascending |
| **Filtering**        | None visible |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Truck Going Fast |
| **Styling**          | Modal view, fixed header, centered empty-state graphic and message |

---

## Column Definitions

| Column Label             | Document key                          | Type     | Sortable | Filterable | Notes                                        |
|--------------------------|---------------------------------------|----------|----------|------------|----------------------------------------------|
| DRIVER NAME              | tds_entity_name                       | Text     | Yes      | No         | Clickable to driver details                  |
| GROUP                    | tds_group_name                        | Text     | Yes      | No         | Driver's assigned Group                      |
| POINTS                   | licence_penalty_points_speeding_count | Number   | Yes      | No         |                                              |
| SPEEDING OFFENCES SCORE  | licence_penalty_points_speeding_score | Number   | Yes      | No         |                                              |
| DATE LAST CHECKED        | licence_last_check_dt                 | Date     | Yes      | No         | Last time data was reviewed or updated       |

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

Add any relevant notes or known bugs here.
