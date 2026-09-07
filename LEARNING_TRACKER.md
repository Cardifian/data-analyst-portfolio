# SQL + Python Learning Tracker

This file is the **living progress tracker**. Update it at the end of each working session.

Status key:
- ⚪ Not encountered
- 🔵 Encountered
- 🟡 Developing
- 🟢 Comfortable

---

## Current Project: UK Road Safety

### Project Progress
- ✅ PostgreSQL installed
- ✅ DBeaver installed
- ✅ `uk_road_safety` database created
- ✅ `raw` schema created
- ✅ `raw.collisions` table created
- ✅ collision CSV imported
- ✅ verified 513,801 collision rows
- ➡️ Next: inspect/profile raw collision data
- ⬜ create clean collisions table
- ⬜ import vehicles
- ⬜ import casualties
- ⬜ verify keys/relationships
- ⬜ multi-table SQL analysis
- ⬜ intermediate SQL analysis
- ⬜ Python/pandas analysis
- ⬜ charts + findings
- ⬜ GitHub README + portfolio packaging

---

## SQL Skill Tracker

### Database Foundations
- Database / server distinction — 🔵
- Schemas — 🔵
- Tables — 🔵
- Data types — 🔵
- Raw vs clean data layers — 🔵
- Primary key — 🔵
- Composite key — 🔵
- Foreign key — 🔵
- One-to-many relationships — 🔵

### Query Fundamentals
- `SELECT` — 🔵
- `LIMIT` — 🔵
- aliases (`AS`) — 🔵
- `WHERE` — ⚪
- `ORDER BY` — 🔵
- `DISTINCT` — ⚪

### Aggregation
- `COUNT()` — 🔵
- `GROUP BY` — 🔵
- `SUM()` — ⚪
- `AVG()` — ⚪
- `MIN()` / `MAX()` — ⚪
- `HAVING` — ⚪
- conditional aggregation — ⚪

### Transformation
- `CASE` — 🔵
- `NULL` handling — ⚪
- `COALESCE` — ⚪
- casting / type conversion — ⚪
- date/time functions — ⚪

### Relational SQL
- `INNER JOIN` — ⚪
- `LEFT JOIN` — ⚪
- join duplication awareness — ⚪
- multi-table joins — ⚪

### Intermediate SQL
- subqueries — ⚪
- CTEs — ⚪
- window functions — ⚪

### Window Function Sub-skills
- concept vs `GROUP BY` — ⚪
- `SUM() OVER()` — ⚪
- `AVG() OVER()` — ⚪
- `PARTITION BY` — ⚪
- `ROW_NUMBER()` — ⚪
- `RANK()` — ⚪
- `DENSE_RANK()` — ⚪
- `LAG()` — ⚪
- `LEAD()` — ⚪
- running totals — ⚪

---

## Python Skill Tracker

### Python Fundamentals
- variables — ⚪
- data types — ⚪
- lists — ⚪
- dictionaries — ⚪
- conditions — ⚪
- loops — ⚪
- functions — ⚪

### pandas
- DataFrame concept — ⚪
- reading CSV/database data — ⚪
- selecting columns — ⚪
- filtering — ⚪
- sorting — ⚪
- `groupby` — ⚪
- aggregation — ⚪
- `merge` — ⚪
- missing values — ⚪
- dates — ⚪

### Visualisation
- matplotlib basics — ⚪
- chart selection — ⚪
- clear labels/titles — ⚪
- communicating findings — ⚪

---

## Review Queue

### Next retrieval
- Explain what `GROUP BY` does without looking at syntax.
- Given a categorisation problem, recognise that `CASE` may be useful.
- Explain why `collision_index + vehicle_reference` can form a composite key.

### Later
- `CASE` for ranges/categories
- `CASE` for conditional aggregation
- `GROUP BY` using more than one column
- data types during clean-table creation
- primary/foreign keys again when vehicles and casualties are imported

---

## Mistake / Confusion Log

Use this format:

**Date / concept:**  
**What happened:**  
**Why:**  
**What to remember:**

Current examples:

**Raw data types**  
What happened: Confusion about why raw columns were stored as text.  
What to remember: CSVs do not carry PostgreSQL data types. The raw layer preserves the source representation; the clean layer will deliberately convert values into analytical types.

**DBeaver database context**  
What happened: The SQL editor initially remained connected to the default `postgres` database.  
What to remember: In PostgreSQL, the SQL editor/connection must target the intended database; `SELECT current_database();` verifies it.

---

## Session Template

### Start of session
1. Where are we in the project?
2. What is today's tangible project milestone?
3. Do 3–5 retrieval questions from old concepts.
4. Check the review queue.

### During session
- Project work is the main task.
- Prefer 1 major new concept per session.
- If a concept appears, learn only enough to continue unless it blocks understanding.
- Add important concepts to the review queue instead of derailing the project.
- Gradually reduce hints and stop naming the required SQL technique in advance.

### End of session
1. Record what was built/analysed.
2. Update skill statuses.
3. Add 1–3 items to the review queue.
4. Record important mistakes/confusions.
5. Write the next project step.
6. When GitHub is set up, make a useful commit whenever there is meaningful progress.

---

## Session Log

### Session — 07 Sep 2026
**Project progress:**
- Set up PostgreSQL and DBeaver.
- Created `uk_road_safety` database.
- Created `raw` schema and `raw.collisions`.
- Imported and verified 513,801 collision rows.
- Ran initial `SELECT`, `COUNT`, and `GROUP BY` queries.

**New/encountered concepts:**
- database / schema / table
- raw data layer
- data types
- primary and composite keys
- `SELECT`
- `COUNT()`
- `GROUP BY`
- `CASE`

**Next project step:**
- Inspect and profile raw collision data before creating the clean analytical table.
