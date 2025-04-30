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

| Column Label        | Document key      | Type     | Sortable | Filterable | Notes                                         |
|---------------------|-------------------|----------|----------|------------|-----------------------------------------------|
| VRN                 |                   | Text     | Yes      | No         | Vehicle registration number                   |
| GROUP               |                   | Text     | Yes      | No         | Assigned region or team                       |
| DISTANCE (MILES)    |                   | Number   | Yes      | No         | Total mileage driven during tracked period    |
| TRIPS               |                   | Number   | Yes      | No         | Total trip count                              |
| DAYS UTILISED       |                   | Number   | Yes      | No         | Number of days vehicle was used               |
| DRIVING TIME (H)    |                   | Number   | Yes      | No         | Total driving hours                           |
| STANDSTILL TIME (H) |                   | Number   | Yes      | No         | All values shown as 0 in this dataset         |
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
