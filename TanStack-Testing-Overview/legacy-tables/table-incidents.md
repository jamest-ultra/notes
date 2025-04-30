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
| **Default Sorting**  | No |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | Yes/No - What does it say? |
| **Icon Renders**     | Warning Icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label     | Document key | Type   | Sortable | Filterable | Notes                                                        |
|------------------|--------------|--------|----------|------------|--------------------------------------------------------------|
| Claim Reference  |              | Text   | true     | false      | Unique identifier for the claim (UUID format)                |
| Driver Name      |              | Text   | true     | false      | Full name of the driver involved                             |
| Incident Date    |              | Date   | true     | false      | Date when the incident occurred                              |
| VRN              |              | Text   | true     | false      | Vehicle Registration Number                                  |
| Fault Type       |              | Text   | true     | false      | Categorisation of fault (e.g., Driver, Third Party, etc.)    |
| Cost             |              | Number | false    | false      | Monetary cost associated with the incident (nullable)        |

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
