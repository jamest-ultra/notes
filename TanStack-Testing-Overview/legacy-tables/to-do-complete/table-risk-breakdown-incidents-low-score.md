# Table Documentation: [Incidents - Low Score]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side |
| **Default Sorting**  | No |
| **Filtering**        | None visible |
| **Search**           | No global search |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Yes, Car crash icon |
| **Styling**          | Clean modal layout, fixed headers, centered empty-state graphic and text |

---

## Column Definitions

| Column Label    | Document key     | Type     | Sortable | Filterable | Notes                                   |
|-----------------|------------------|----------|----------|------------|-----------------------------------------|
| DRIVER NAME     |                  | Text     | Yes      | No         | Clickable to driver details             |
| GROUP           |                  | Text     | Yes      | No         | User’s assigned group                   |
| INCIDENT SCORE  |                  | Number   | Yes      | No         | Represents a severity score  |

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
