# Table Documentation: [Incidents]

## Page / Context
**Page:** [/standard#/report/manager/summary/incidents]
**Status:** Phase 1
**Table Id:** [reporting.table.title.incidents]

---

## General Table Properties

| Property             | Description / Value |
|----------------------|---------------------|
| **Data Source**      | Rest API state |
| **Pagination**       | Client-side |
| **Default Sorting**  | No |
| **Filtering**        | No |
| **Search**           | No |
| **Column Visibility**| No |
| **Table Actions**    | Download |
| **Tool-tip Text**    | Yes/No - What does it say? |
| **Icon Renders**     | Warning Icon |
| **Styling**          | Fixed headers |

---

## Column Definitions

| Column Label     | Document key       | Type   | Sortable | Filterable | Notes                                                        |
|------------------|--------------------|--------|----------|------------|--------------------------------------------------------------|
| Claim Reference  | claim_reference_no | Text   | true     | false      | Unique identifier for the claim (UUID format)                |
| Driver Name      | tds_driver_name    | Text   | true     | false      | Full name of the driver involved                             |
| Incident Date    | odometer_dt        | Date   | true     | false      | Date when the incident occurred                              |
| VRN              | vehicle_vrn        | Text   | true     | false      | Vehicle Registration Number                                  |
| Fault Type       | fault_type         | Text   | true     | false      | Categorisation of fault (e.g., Driver, Third Party, etc.)    |
| Cost             | total_net_cost     | Number | false    | false      | Monetary cost associated with the incident (nullable)        |

---

## Testing Checklist (Tan-stack Migration)

- [x] All expected columns are present
- [x] Column order and labels match legacy table
- [x] Sorting works as before
- [x] Filtering behaves as before (types, logic)
- [x] Pagination works the same way
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

- Your now able to select licence plate
- Title has now been updated to incidents for demo instead of demo
