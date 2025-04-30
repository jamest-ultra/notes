# Table Documentation: [Key metrics]

## Page / Context
**Page:** [/standard#/report/manager/summary/breakdown]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property              | Description / Value                                                                 |
|-----------------------|--------------------------------------------------------------------------------------|
| **Data Source**       | local storage |
| **Pagination**        | Client-side |
| **Default Sorting**   | Yes — sorted by Name (ascending)                                                    |
| **Filtering**         | Toggle-based filtering by data type (Telemetry, Licence, Incident) — not per column |
| **Search**            | No |
| **Column Visibility** | No |
| **Table Actions**     | Download button (top-right) |
| **Tool-tip Text**     | "A summarised view of different scores against each group. Click on the toggle to display scores against all drivers." |
| **Icon Renders**      | Statistics graph |
| **Styling**           | Fixed header, slight row hover, no zebra striping |

---

## Column Definitions

| Column Label            | Document key | Type     | Sortable | Filterable | Notes                                                                 |
|-------------------------|--------------|----------|----------|------------|-----------------------------------------------------------------------|
| Name                    |              | Text     | true     | true       | Group or region name                                                 |
| Ultra Score             |              | Number   | true     | true       | Composite score; includes coloured dot indicator                     |
| Driving Behaviour Score |              | Number   | true     | true       | Includes count of events and per-1,000 mile rate                     |
| Total Distance (MI)     |              | Number   | true     | true       | Total miles driven                                                   |
| Licence Score           |              | Number   | true     | true       | Includes count of events and per-1,000 mile rate                     |
| Endorsements            |              | Number   | true     | true       | Number of endorsements                                               |
| Incident Score          |              | Number   | true     | true       | Includes count of incidents and per-1,000 mile rate; colour-coded    |
| Total Cost              |              | Currency | true     | true       | Total monetary cost, formatted as £GBP                               |

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
