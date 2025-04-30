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

| Column Label   | Document key  | Type     | Sortable | Filterable | Notes                                |
|----------------|---------------|----------|----------|------------|--------------------------------------|
| DATE           |               | Date     | Yes      | No         | routes to details |
| TIME           |               | Text     | Yes      | No         | 24-hour format                       |
| LOCATION       |               | Text     | Yes      | No         |                                      |
| MAX SPEED      |               | Number   | Yes      | No         | Includes "mph" suffix                |
| SPEED LIMIT    |               | Number   | Yes      | No         |                                      |
| OVER LIMIT (%) |               | Number % | Yes      | No         | Calculated percentage over limit     |

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
