# Table Documentation: [Driver Tree]

## Page / Context
**Page:** [/standard#/report/manager/summary/driver/tree]
**Status:** Phase 1
**Table ID:** []

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | local state |
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

| Column Label | Document key | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|--------------|--------------|----------------------------|----------|------------|-------|
|Names         |              |Text                        |true      |true        |       |
|VRN           |              |Text                        |true      |true        |       |
|EMPLOYEE ID   |              |Number                      |true      |true        |       |
|FOB           |              |Number                      |true      |false       |       |
|GROUP         |              |Text                        |true      |true        |       |

---

## Testing Checklist (TanStack Migration)

- [ ] All expected columns are present
- [ ] Column order and labels match legacy table
- [ ] Sorting works as before
- [ ] Filtering behaves as before (types, logic)
- [ ] Pagination works the same way
- [ ] Global and column search matches behavior
- [ ] Row and bulk actions behave identically
- [ ] Custom renderers look/function correctly
- [ ] Styling and layout is consistent with legacy
- [ ] Table is responsive and mobile-compatible
- [ ] Loading, error, and empty states work properly
- [ ] Accessibility (keyboard, ARIA roles) is preserved
- [ ] Performance is acceptable for large datasets

---

## Notes / Known Issues

Add any relevant notes, quirks, limitations, or known bugs here.
