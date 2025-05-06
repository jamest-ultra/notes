# Table Documentation: [TCO]

## Page / Context
**Page:** [/standard#/report/manager/tco]
**Status:** Phase 1
**Table Id:** [tco-summary]

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

| Column Label | Document key         | Type     | Sortable | Filterable | Notes                                            |
|--------------|----------------------|----------|----------|------------|--------------------------------------------------|
| GROUP        | tds_entity_name      | Text     | Yes      | Yes (via dropdown filter) | Location or department name                     |
| VEHICLES     | active_vehicle_count | Number   | Yes      | No         | Total number of vehicles in the group            |
| AVG. COST    | avg_cost_per_vehicle | Currency | Yes      | No         | Shown in GBP (£); Depending on currency selected |
| TOTAL COST   | total_cost           | Currency | Yes      | No         | Group-wide total for selected period |

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
