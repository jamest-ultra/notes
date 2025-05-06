# Table Documentation: [Speeding - low score]

## Page / Context
**Page:** [/standard#/report/manager/summary/risk]
**Status:** Phase 1
**Table Id:** [risk_high_driving_score_entity_count]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes — Driving Score ascending |
| **Filtering**        | None visible |
| **Search**           | No global search |
| **Column Visibility**| No toggle options shown |
| **Table Actions**    | Yes — Download icon in top right corner |
| **Tool-tip Text**    | No tooltips shown |
| **Icon Renders**     | Car tilt |
| **Styling**          | Fixed headers, clean modal design, zebra striping absent |

---

## Column Definitions

| Column Label    | Document key     | Type     | Sortable | Filterable | Notes                                      |
|-----------------|------------------|----------|----------|------------|--------------------------------------------|
| DRIVER NAME     | tds_entity_name  | Text     | Yes      | No         | Clickable link to driver profile           |
| GROUP           | tds_group_name   | Text     | Yes      | No         | Represents a location or region            |
| DRIVING EVENTS  | driving_events   | Number   | Yes      | No         | Count of logged driving-related events     |
| DRIVING SCORE   | driving_score    | Number   | Yes      | No         | Score out of 10, includes red warning icon |

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
