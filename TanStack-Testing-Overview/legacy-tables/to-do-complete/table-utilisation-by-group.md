# Table Documentation: [Utilisation by Group]

## Page / Context
**Page:** [/standard#/report/manager/summary/utilisation]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (all 4 groups shown) |
| **Default Sorting**  | Yes — Group name ascending |
| **Filtering**        | Not visible here; may be global page filters (e.g. by period) |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | Not shown in this view |
| **Icon Renders**     | Yes — Header icon representing fleet/utilisation theme |
| **Styling**          | Fixed headers, nested data (values + “per vehicle” line), clean grid layout |

---

## Column Definitions

| Column Label         | Document key        | Type     | Sortable | Filterable | Notes                                                  |
|----------------------|---------------------|----------|----------|------------|--------------------------------------------------------|
| NAME                 |                     | Text     | Yes      | No         | Group or depot name                                   |
| VEHICLES             |                     | Number   | Yes      | No         | Total number of vehicles                              |
| DISTANCE (MILES)     |                     | Number   | Yes      | No         | Total and per-vehicle mileage                         |
| TRIPS                |                     | Number   | Yes      | No         | Trip count, with per-vehicle average                  |
| DAYS UTILISED        |                     | Number   | Yes      | No         | How many days the fleet was active                    |
| DRIVING TIME (H)     |                     | Duration | Yes      | No         | Driving hours total and per vehicle                   |
| STANDSTILL TIME (H)  |                     | Duration | Yes      | No         | Logged idle/standstill time, total and per vehicle    |

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
