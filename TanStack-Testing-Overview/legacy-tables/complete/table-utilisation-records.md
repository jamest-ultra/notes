# Table Documentation: [Low Usage Vehicles]

## Page / Context
**Page:** [/standard#/report/manager/summary/utilisation]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (10 per page, pagination shown) |
| **Default Sorting**  | Yes — By VRN or Distance |
| **Filtering**        | Not shown (may be a filtered modal from a broader dataset) |
| **Search**           | No |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Yes — Fleet/vehicle icon in header |
| **Styling**          | Modal layout, fixed headers, consistent numeric formatting, clean pagination |
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
