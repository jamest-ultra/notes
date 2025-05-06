# Table Documentation: [Fleet costs for Demo]

## Page / Context
**Page:** [/standard#/report/manager/fleet-cost]
**Status:** Phase 1
**Table Id:** [table-fleetcost-group]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | No |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Check List Icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label  | Document key        | Type      | Sortable | Filterable | Notes                              |
|---------------|---------------------|-----------|----------|------------|------------------------------------|
| Group         | tds_entity_name     | Text      | true     | false      | Links to group-level drilldown     |
| Fleet Costs   | tn_count            | Number    | true     | false      |                                    |
| Invoices      | invoice_count       | Number    | true     | false      |                                    |
| Suppliers     | supplier_count      | Number    | true     | false      |                                    |
| Parts         | parts_tn_count      | Number    | true     | false      |                                    |
| Windscreen    | windscreen_tn_count | Number    | true     | false      |                                    |
| Labour        | windscreen_tn_count | Number    | true     | false      |                                    |
| Paint & Body  | paint_body_tn_count | Number    | true     | false      |                                    |
| Misc          | misc_tn_count       | Number    | true     | false      |                                    |
| Avg. Cost     | avg_tn_net_cost     | Number    | true     | false      |                                    |
| Max Cost      | max_tn_net_cost     | Number    | true     | false      |                                    |
| Total Cost    | tn_net_cost         | Number    | true     | false      |                                    |

---

## Testing Checklist (Tan-stack Migration)

- [X] All expected columns are present
- [X] Column order and labels match legacy table
- [X] Sorting works as before
- [X] Filtering behaves as before (types, logic)
- [X] Pagination works the same way
- [X] Global and column search matches behaviour
- [ ] Custom renders look/function correctly
- [X] Tool-tip text is correct
- [X] Styling and layout is consistent with legacy
- [X] Table is responsive and mobile-compatible
- [X] Loading, error, and empty states work properly
- [X] Accessibility (keyboard, ARIA roles) is preserved
- [X] Performance is acceptable for large datasets

---

## Notes / Known Issues

The table icon isn't correct
