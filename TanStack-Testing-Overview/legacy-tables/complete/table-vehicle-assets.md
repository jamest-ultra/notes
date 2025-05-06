# Table Documentation: [Vehicles]

## Page / Context
**Page:** [/standard#/report/manager/summary/vehicle/tree]
**Status:** Phase 1
**Table Id:** [reporting.title.vehicle-tree]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (pagination shown: 10 per page out of 21 total) |
| **Default Sorting**  | Yes — By VRN (Vehicle Reg Number) ascending |
| **Filtering**        | Yes — Per-column filters (VRN, Make, Model, First Name, Last Name, Group) |
| **Search**           | Yes — Inline search fields under each column heading |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | Yes — “You can search for vehicles here” |
| **Icon Renders**     | Yes — Vehicle icon in header |
| **Styling**          | Fixed headers, zebra striping, paginated, intuitive filter row with clear inputs |

---

## Column Definitions

| Column Label | Document key                 | Type     | Sortable | Filterable | Notes                                              |
|--------------|------------------------------|----------|----------|------------|----------------------------------------------------|
| VRN          | tds_vehicle_vrn              | Text     | Yes      | Yes        | Vehicle registration number                        |
| MAKE         | make                         | Text     | Yes      | Yes        | Manufacturer (e.g., Peugeot, Ford)                 |
| MODEL        | model                        | Text     | Yes      | Yes        | Vehicle model (e.g., Boxer, Proace)                |
| DRIVER       | currentDriverFromAllocations | Text     | Yes      | Yes        | Assigned driver (clickable, routes to driver page) |
| GROUP        | group                        | Text     | Yes      | Yes        | Assigned group or location                         |

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

- Missing sort function on model.
- Tooltip is missing from vehicle tree
