# Table Documentation: [No Name (Part of the EV Suitability page)]

## Page / Context
**Page:** [/standard#/report/manager/summary/ev]
**Status:** Phase 1
**Table Id:** [reporting.table.title.ev-suitability]

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

| Column Label          | Document key   | Type (Text, Number, Date…) | Sortable | Filterable | Notes |
|-----------------------|----------------|----------------------------|----------|------------|-------|
|VRN                    | licenseplate   |Text                        |true      |false       |Should be able to select VRN and navigate to the vehicle details page |
|GROUP                  | region         |Text                        |true      |false       |       |
|DAYS MOVED (IN PERIOD) | days_in_period |Number                      |true      |false       |       |
|MOST MILES (DAY)       | max_miles      |Number                      |true      |false       |       |
|AVERAGE MILES (DAY)    | average_miles  |Number                      |true      |false       |       |
|TOTAL MILES            | total_miles    |Number                      |true      |false       |       |
|MOST TRIPS (DAY)       | max_tours      |Number                      |true      |false       |       |
|AVERAGE TRIPS (DAY)    | average_tours  |Number                      |true      |false       |       |
|TOTAL TRIPS (IN PERIOD)| total_tours    |Number                      |true      |false       |       |

---

## Testing Checklist (Tan-stack Migration)

- [X] All expected columns are present
- [X] Column order and labels match legacy table
- [X] Sorting works as before
- [X] Filtering behaves as before (types, logic)
- [X] Pagination works the same way
- [X] Global and column search matches behaviour
- [X] Custom renders look/function correctly
- [X] Tool-tip text is correct
- [X] Styling and layout is consistent with legacy
- [X] Table is responsive and mobile-compatible
- [X] Loading, error, and empty states work properly
- [X] Accessibility (keyboard, ARIA roles) is preserved
- [X] Performance is acceptable for large datasets

---

## Notes / Known Issues

Add any relevant notes or known bugs here.
