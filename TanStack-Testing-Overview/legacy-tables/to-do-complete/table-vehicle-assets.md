# Table Documentation: [Vehicles]

## Page / Context
**Page:** [/standard#/report/manager/summary/vehicle/tree]
**Status:** Phase 1
**Table Id:** [Id of the table]

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

| Column Label | Document key   | Type     | Sortable | Filterable | Notes                                              |
|--------------|----------------|----------|----------|------------|----------------------------------------------------|
| VRN          |                | Text     | Yes      | Yes        | Vehicle registration number                        |
| MAKE         |                | Text     | Yes      | Yes        | Manufacturer (e.g., Peugeot, Ford)                 |
| MODEL        |                | Text     | Yes      | Yes        | Vehicle model (e.g., Boxer, Proace)                |
| DRIVER       |                | Text     | Yes      | Yes        | Assigned driver (clickable, routes to driver page) |
| GROUP        |                | Text     | Yes      | Yes        | Assigned group or location                         |

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
