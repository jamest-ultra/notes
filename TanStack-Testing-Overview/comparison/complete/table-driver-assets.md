# Table Documentation: [Driver Tree]

## Page / Context
**Page:** [/standard#/report/manager/summary/driver/tree]
**Status:** Phase 1
**Table Id:** [asset-list-drivers]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Name |
| **Filtering**        | Per column |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download  |
| **Tool-tip Text**    | "You can seach for individual drivers here" |
| **Icon Renders**     | Steering wheel |
| **Styling**          | Fixed headers |
---

## Column Definitions

| Column Label | Document key         | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|--------------|----------------------|----------------------------|----------|------------|-------|
|Names         | FirstName + LastName |Text                        |true      |true        |       |
|VRN           | currentVehicle.vrn   |Text                        |true      |true        |       |
|EMPLOYEE ID   | employeeId           |Number                      |true      |true        |       |
|FOB           | FobUID               |Number                      |true      |false       |       |
|GROUP         | currentGroup.name    |Text                        |true      |true        |       |

---

## Testing Checklist (TanStack Migration)

- [ ] All expected columns are present
- [x] Column order and labels match legacy table
- [ ] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [x] Pagination works the same way
- [x] Global and column search matches behavior
- [ ] Custom renderers look/function correctly
- [ ] Styling and layout is consistent with legacy
- [x] Table is responsive and mobile-compatible
- [x] Loading, error, and empty states work properly
- [x] Performance is acceptable for large datasets

---

## Notes / Known Issues

- Missing Fob Column
- Missing sort function on driver.
- Tooltip is missing from driver tree
