# Table Documentation: [Safety Events]

## Page / Context
**Page:** [/standard#/report/manager/summary/telemetry]
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
| **Tool-tip Text**    | "Combined Telematics recorderd speeding, braking and cornering events" |
| **Icon Renders**     | Man with hard hat |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label   | Document key | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|----------------|--------------|----------------------------|----------|------------|-------|
|Name            |              |Text                        |true      |false       |       |
|Events          |              |Number                      |true      |false       |This number would change depending on the unit used |
|Per 1,000 Miles |              |Number                      |true      |false       |This should update to 1,000 Km when unit changes |

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
