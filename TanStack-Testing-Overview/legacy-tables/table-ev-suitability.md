# Table Documentation: [No Name (Part of the EV Suitability page)]

## Page / Context
**Page:** [/standard#/report/manager/summary/ev]
**Status:** Phase 1
**Table Id:** [Id of the table]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | Yes - Total Trips (IN Period), In Ascending |
| **Filtering**        | Global, Max Miles Per Day & Min Days Moved |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | "A summary table of EV suitable vehicles, based on and showing the distance, trips and days moved for the past 3, 6, 12 months (within the defined parameters)" |
| **Icon Renders**     | A truck icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label          | Document key | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|-----------------------|--------------|----------------------------|----------|------------|-------|
|VRN                    |              |Text                        |true      |false       |Should be able to select VRN and navigate to the vehicle details page |
|GROUP                  |              |Text                        |true      |false       |       |
|DAYS MOVED (IN PERIOD) |              |Number                      |true      |false       |       |
|MOST MILES (DAY)       |              |Number                      |true      |false       |       |
|AVERAGE MILES (DAY)    |              |Number                      |true      |false       |       |
|TOTAL MILES            |              |Number                      |true      |false       |       |
|MOST TRIPS (DAY)       |              |Number                      |true      |false       |       |
|AVERAGE TRIPS (DAY)    |              |Number                      |true      |false       |       |
|TOTAL TRIPS (IN PERIOD)|              |Number                      |true      |false       |       |

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
