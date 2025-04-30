# Table Documentation: [Inventory for [Demo]]

## Page / Context
**Page:** [/standard#/report/manager/inventory]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | local state |
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

| Column Label      | Document key | Type    | Sortable | Filterable | Notes                                                         |
|-------------------|--------------|---------|----------|------------|---------------------------------------------------------------|
| Group             |              | Text    | true     | true       | Links to group-specific fuel stats breakdown                  |
| Vehicle Count     |              | Number  | true     | true       |                                                               |
| Avg. Age          |              | Number  | true     | true       |                                                               |
| Renewals          |              | Number  | true     | true       |                                                               |
| Rewrites          |              | Number  | true     | true       | Links to table of rewrites                                    |
| Overdue           |              | Number  | true     | true       | Links to table of overdue                                     |
| Average Rental    |              | Currency| true     | true       |                                                               |

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
