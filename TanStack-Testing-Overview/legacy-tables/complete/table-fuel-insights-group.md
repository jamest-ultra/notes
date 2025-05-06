# Table Documentation: [Insights for [Company]]

## Page / Context
**Page:** [/standard#/report/manager/fuel-insights]
**Status:** Phase 1
**Table Id:** [reporting.title.fuel-insights]

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

| Column Label         | Document key                 | Type   | Sortable | Filterable | Notes                                               |
|----------------------|------------------------------|--------|----------|------------|-----------------------------------------------------|
| Group                | group                        | Text   | true     | false      | Links to group-specific insights or drilldown       |
| Weekend              | weekend_tn_count             | Number | true     | false      | Links to a modal of those fuel transactions         |
| Small                | small_tn_count               | Number | true     | false      | Links to a modal of those fuel transactions         |
| Tank Size            | tanksize_tn_count            | Number | true     | false      | Links to a modal of those fuel transactions         |
| Premium              | premium_tn_count             | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Card       | unmatched_card_vrn_tn_count  | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Vehicle    | unmatched_vrn_tn_count       | Number | true     | false      | Links to a modal of those fuel transactions         |
| Unmatched Fuel       | unmatched_fuel_type_tn_count | Number | true     | false      | Links to a modal of those fuel transactions         |
| Non Fuel             | non_fuel_tn_count            | Number | true     | false      | Links to a modal of those fuel transactions         |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
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

The table icon isn't correct
