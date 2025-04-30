# Table Documentation: [Fleet costs for Demo]

## Page / Context
**Page:** [/standard#/report/manager/fleet-cost]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | local state |
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

| Column Label  | Document key       | Type      | Sortable | Filterable | Notes                              |
|---------------|--------------------|-----------|----------|------------|------------------------------------|
| Group         |                    | Text      | true     | false      | Links to group-level drilldown     |
| Fleet Costs   |                    | Number    | true     | false      |                                    |
| Invoices      |                    | Number    | true     | false      |                                    |
| Suppliers     |                    | Number    | true     | false      |                                    |
| Parts         |                    | Number    | true     | false      |                                    |
| Windscreen    |                    | Number    | true     | false      |                                    |
| Labour        |                    | Number    | true     | false      |                                    |
| Paint & Body  |                    | Number    | true     | false      |                                    |
| Misc          |                    | Number    | true     | false      |                                    |
| Avg. Cost     |                    | Number    | true     | false      |                                    |
| Max Cost      |                    | Number    | true     | false      |                                    |
| Total Cost    |                    | Number    | true     | false      |                                    |
| Total Cost    |                    | Number    | true     | false      |                                    |

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
