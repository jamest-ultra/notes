# Table Documentation: [Incidents]

## Page / Context
**Page:** [/standard#/report/manager/summary/incidents]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Incident Score, Ascending |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Warning Icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label     | Document key    | Type   | Sortable | Filterable | Notes                                                         |
|------------------|-----------------|--------|----------|------------|---------------------------------------------------------------|
| Driver           | tds_entity_name | Text   | true     | true       | Driver name, likely clickable for more details                |
| Group            | tds_group_name  | Text   | true     | true       | Assigned region/group                                         |
| Incident Score   | incident_score  | Number | true     | true       | Numeric score with a coloured indicator (e.g. risk severity)  |

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
