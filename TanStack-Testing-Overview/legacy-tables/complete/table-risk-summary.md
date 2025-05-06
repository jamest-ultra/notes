# Table Documentation: [Risk Summary]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [reporting.table.title.risk-summary]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
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

| Column Label             | Document key                  | Type     | Sortable | Filterable | Notes                                                  |
|--------------------------|-------------------------------|----------|----------|------------|--------------------------------------------------------|
| GROUP NAME               | tds_entity_name               | Text     | Yes      | No         | Links to more detailed group reports          |
| ULTRA SCORE              | risk_score                    | Number   | Yes      | No         | Performance indicator; uses colored dot (risk level)   |
| INCIDENT SCORE           | licence_score                 | Number   | Yes      | No         | Incident-based risk; color-coded                       |
| LICENCE SCORE            | incident_score                | Number   | Yes      | No         | Related to licence points or violations                |
| RISK ASSESSMENT SCORE    | licence_risk_assessment_score | Number   | Yes      | No         |                                   |
| DRIVING SCORE            | telemetry_score               | Number   | Yes      | No         | Driving behavior-based score                           |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [ ] Pagination works the same way
- [x] Global and column search matches behaviour
- [x] Custom renders look/function correctly
- [x] Tool-tip text is correct
- [x] Styling and layout is consistent with legacy
- [x] Table is responsive and mobile-compatible
- [x] Loading, error, and empty states work properly
- [x] Accessibility (keyboard, ARIA roles) is preserved
- [x] Performance is acceptable for large datasets

---

## Notes / Known Issues

Add any relevant notes or known bugs here.
