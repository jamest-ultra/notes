# Table Documentation: [Fuel stats - Combustion]

## Page / Context
**Page:** [/standard#/report/manager/fuel-stats]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API |
| **Pagination**       | Client-side (6 results shown) |
| **Default Sorting**  | Yes — By Licence Plate ascending |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No toggle options |
| **Table Actions**    | Yes — Download icon in top right |
| **Tool-tip Text**    | No visible tooltips |
| **Icon Renders**     | Yes — Fuel/stats icon in header |
| **Styling**          | Fixed headers, clean grid layout, numerical alignment for readability |

---

## Column Definitions

| Column Label    | Document key     | Type     | Sortable | Filterable | Notes                                        |
|-----------------|------------------|----------|----------|------------|----------------------------------------------|
| LICENCE PLATE   |                  | Text     | Yes      | No         | Vehicle registration number                  |
| TRANSACTIONS    |                  | Number   | Yes      | No         | Able to drip into the transactions           |
| LITRES          |                  | Number   | Yes      | No         | Fuel dispensed (L)                           |
| KWH             |                  | Number   | Yes      | No         | Energy equivalent (if EV hybrid)             |
| KG              |                  | Number   | Yes      | No         | Likely CO₂ equivalent weight                 |
| COST            |                  | Currency | Yes      | No         | Monetary cost — shown as “-”                 |

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
