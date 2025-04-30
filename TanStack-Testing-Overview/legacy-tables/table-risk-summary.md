# Table Documentation: [Risk Summary]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Local Storage |
| **Pagination**       | Client-side |
| **Default Sorting**  | No |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Triangle with exclamation mark |
| **Styling**          | Fixed headers, clean grid layout, responsive with icons for scoring levels |

---

## Column Definitions

| Column Label             | Document key             | Type     | Sortable | Filterable | Notes                                                  |
|--------------------------|--------------------------|----------|----------|------------|--------------------------------------------------------|
| GROUP NAME               |                          | Text     | Yes      | No         | Links to more detailed group reports          |
| ULTRA SCORE              |                          | Number   | Yes      | No         | Performance indicator; uses colored dot (risk level)   |
| INCIDENT SCORE           |                          | Number   | Yes      | No         | Incident-based risk; color-coded                       |
| LICENCE SCORE            |                          | Number   | Yes      | No         | Related to licence points or violations                |
| RISK ASSESSMENT SCORE    |                          | Number   | Yes      | No         |                                   |
| DRIVING SCORE            |                          | Number   | Yes      | No         | Driving behavior-based score                           |

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
