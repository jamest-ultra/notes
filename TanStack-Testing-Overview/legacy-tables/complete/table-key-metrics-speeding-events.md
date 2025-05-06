# Table Documentation: [Speeding Events]

## Page / Context
**Page:** [/standard#/report/manager/summary/breakdown/driver/summary/speeding/events]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes — Date descending |
| **Filtering**        | None visible |
| **Search**           | No global search bar |
| **Column Visibility**| No toggle options |
| **Table Actions**    | None visible (no download, export, etc.) |
| **Tool-tip Text**    | No tooltips visible |
| **Icon Renders**     | Yes — Icon of a car with a car behind |
| **Styling**          | Fixed headers, zebra striping (alternating row colors), responsive UI |

---

## Column Definitions

| Column Label   | Document key                 | Type     | Sortable | Filterable | Notes                                |
|----------------|------------------------------|----------|----------|------------|--------------------------------------|
| DATE           | position.datetime            | Date     | Yes      | No         | routes to details                    |
| TIME           | position.datetime.time       | Text     | Yes      | No         | 24-hour format                       |
| LOCATION       | position.location            | Text     | Yes      | No         |                                      |
| MAX SPEED      | speed_mph                    | Number   | Yes      | No         | Includes "mph" suffix                |
| SPEED LIMIT    | speed_limit_mph              | Number   | Yes      | No         |                                      |
| OVER LIMIT (%) | percent_over_speed_limit_mph | Number % | Yes      | No         | Calculated percentage over limit     |

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

- Icon is different
