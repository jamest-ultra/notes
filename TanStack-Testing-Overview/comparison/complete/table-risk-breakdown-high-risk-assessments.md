# Table Documentation: [High Risk Assessments]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [risk_high_risk_assessment_score_entity_count]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes — Risk Assessment Score ascending |
| **Filtering**        | None visible |
| **Search**           | No global search bar |
| **Column Visibility**| No toggle options shown |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No |
| **Icon Renders**     | Box with exclamation point |
| **Styling**          | Modal layout, clean and centered empty state, fixed header |

---

## Column Definitions

| Column Label            | Document key          | Type     | Sortable | Filterable | Notes                                   |
|-------------------------|-----------------------|----------|----------|------------|-----------------------------------------|
| DRIVER NAME             | driver_id             | Text     | Yes      | No         | Clickable to driver details             |
| GROUP                   | group_name            | Text     | Yes      | No         | User’s assigned group                   |
| RISK ASSESSMENT SCORE   | risk_assessment_score | Number   | Yes      | No         | scoring model                           |

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

Add any relevant notes or known bugs here.
