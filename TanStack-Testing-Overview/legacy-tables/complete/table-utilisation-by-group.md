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

| Column Label         | Document key         | Type     | Sortable | Filterable | Notes                                                  |
|----------------------|----------------------|----------|----------|------------|--------------------------------------------------------|
| NAME                 | tds_entity_name      | Text     | Yes      | No         | Group or depot name                                   |
| VEHICLES             | active_vehicle_count | Number   | Yes      | No         | Total number of vehicles                              |
| DISTANCE (MILES)     | distance_driven_     | Number   | Yes      | No         | Total and per-vehicle mileage                         |
| TRIPS                | trip_count           | Number   | Yes      | No         | Trip count, with per-vehicle average                  |
| DAYS UTILISED        | days_utilised        | Number   | Yes      | No         | How many days the fleet was active                    |
| DRIVING TIME (H)     | driving_time_seconds | Duration | Yes      | No         | Driving hours total and per vehicle                   |
| STANDSTILL TIME (H)  | driving_time_seconds | Duration | Yes      | No         | Logged idle/standstill time, total and per vehicle    |

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
