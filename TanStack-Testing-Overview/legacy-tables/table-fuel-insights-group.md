# Table Documentation: [Insights for [Company]]

## Page / Context
**Page:** [/standard#/report/manager/fuel-insights]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Group Column, Ascending |
| **Filtering**        | No |
| **Search**           | Yes, Period, Vehicle Types, Currency |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Check List Icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label         | Document key | Type   | Sortable | Filterable | Notes                                               |
|----------------------|--------------|--------|----------|------------|-----------------------------------------------------|
| Group                |              | Text   | true     | false      | Links to group-specific insights or drilldown       |
| Weekend              |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Small                |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Tank Size            |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Premium              |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Card       |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Vehicle    |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Fuel       |              | Number | true     | false      | Links to a modal of those fuel transactions         |
| Non Fuel             |              | Number | true     | false      | Links to a modal of those fuel transactions         |
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
