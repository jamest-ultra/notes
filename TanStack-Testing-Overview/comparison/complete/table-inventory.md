# Table Documentation: [Inventory for [Demo]]

## Page / Context
**Page:** [/standard#/report/manager/inventory]
**Status:** Phase 1
**Table Id:** [inventory-summary]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Vehicle Count |
| **Filtering**        | Global, Vehicle type, Funding and Currency |
| **Search**           | Yes |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Checklist |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label      | Document key            | Type    | Sortable | Filterable | Notes                                                         |
|-------------------|-------------------------|---------|----------|------------|---------------------------------------------------------------|
| Group             | tds_entity_name         | Text    | true     | true       | Links to group-specific fuel stats breakdown                  |
| Vehicle Count     | inventory_vehicle_count | Number  | true     | true       |                                                               |
| Avg. Age          |                         | Number  | true     | true       |                                                               |
| Renewals          | renewals_count          | Number  | true     | true       |                                                               |
| Rewrites          | rewrites_count          | Number  | true     | true       | Links to table of rewrites                                    |
| Overdue           | overdue_count           | Number  | true     | true       | Links to table of overdue                                     |
| Average Rental    | avg_funding_cost        | Currency| true     | true       |                                                               |

---

## Testing Checklist (Tan-stack Migration)

- [ ] All expected columns are present
- [ ] Column order and labels match legacy table
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

- Missing Avg Age column
- The table icon is different from current icon
