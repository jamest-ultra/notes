# Table Documentation: [Driving Behaviour League]

## Page / Context
**Page:** [/standard#/report/manager/summary/telemetry]
**Status:** Phase 1
**Table Id:** [driving-behaviour-league]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Driving Behaviour Score |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Trophy |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label           | Document key    | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|------------------------|-----------------|----------------------------|----------|------------|-------|
|Name                    | tds_entity_name |Text                        |true      |false       |       |
|Driving Behaviour Score | telemetry_score |float                       |false     |false       |       |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [ ] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [x] Custom renderers look/function correctly
- [ ] Styling and layout is consistent with legacy    | Slightly off but no-one will notice
- [x] Table is responsive and mobile-compatible
- [x] Loading, error, and empty states work properly
- [x] Performance is acceptable for large datasets

---

## Notes / Known Issues

- The first column is called Group - In the legacy table it was called Name
