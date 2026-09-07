# Project Status

## Current stage
Raw collision data imported into PostgreSQL. Beginning data profiling and cleaning.

## Completed
- Installed PostgreSQL and DBeaver
- Created `uk_road_safety` database
- Created `raw` schema
- Created `raw.collisions` table
- Imported 513,801 collision records
- Verified row count with SQL
- Began exploring the dataset

## SQL concepts encountered
- `SELECT`
- `COUNT()`
- `GROUP BY`
- `ORDER BY`
- `LIMIT`
- `CASE`

## Current learning status
- `SELECT` — 🟡 Developing
- `COUNT()` — 🟡 Developing
- `GROUP BY` — 🟡 Developing
- `CASE` — 🔵 Encountered
- joins — ⚪ Not encountered
- CTEs — ⚪ Not encountered
- window functions — ⚪ Not encountered

## Next project steps
1. Inspect raw collision values
2. Identify missing and special-coded values
3. Create a cleaned `collisions` table with appropriate data types
4. Import vehicles and casualties
5. Verify table relationships
6. Begin multi-table SQL analysis

## Review queue
- Retrieve `CASE` without being told to use it
- Practise `GROUP BY` with more than one column
- Revisit data types during clean-table creation

## Session handoff
The collision CSV has been successfully loaded into `raw.collisions` with 513,801 rows. Next session should begin with a short retrieval exercise, then continue by profiling the raw collision data before creating `clean.collisions`.
