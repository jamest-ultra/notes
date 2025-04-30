# Table Documentation: [TCO]

## Page / Context
**Page:** [/standard#/report/manager/tco]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes — Group Name ascending |
| **Filtering**        | Yes — Filters for Period, Vehicle Types, Funding, Currency (GBP) |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right of table |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Yes — Checklist icon |
| **Styling**          | Fixed headers, clean layout, integrated with interactive chart above |

---

## Column Definitions

| Column Label | Document key   | Type     | Sortable | Filterable | Notes                                            |
|--------------|----------------|----------|----------|------------|--------------------------------------------------|
| GROUP        |                | Text     | Yes      | Yes (via dropdown filter) | Location or department name                     |
| VEHICLES     |                | Number   | Yes      | No         | Total number of vehicles in the group            |
| AVG. COST    |                | Currency | Yes      | No         | Shown in GBP (£); Depending on currency selected |
| TOTAL COST   |                | Currency | Yes      | No         | Group-wide total for selected period |

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
