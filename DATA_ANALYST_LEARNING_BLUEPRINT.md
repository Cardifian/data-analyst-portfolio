# Data Analyst Learning + Portfolio Blueprint

## Main Goal

Build a job-ready data analyst portfolio while learning SQL and Python through real projects.

The project is the **main road**. Concepts such as `CASE`, CTEs, window functions, pandas, joins, etc. are learned through repeated use inside the projects, not as a separate long course.

We will avoid two extremes:

- **Do not stop the project** every time a new concept appears and try to master it completely.
- **Do not use a concept once and forget it.**

Instead we use a spiral:

> **Encounter → Retrieve → Apply → Combine**

---

# 1. Portfolio Roadmap

## Project 1 — UK Road Safety
**Main emphasis:** SQL, relational databases, data cleaning, joins, analytical thinking.

Skills likely to appear:
- PostgreSQL + DBeaver
- Databases, schemas, tables
- Data types
- Primary keys / foreign keys / composite keys
- Raw vs clean data layers
- `SELECT`, `WHERE`, `ORDER BY`
- `COUNT`, `SUM`, `AVG`
- `GROUP BY`, `HAVING`
- `CASE`
- joins
- CTEs
- window functions
- date/time analysis
- data-quality checks
- later: Python/pandas + visualisation

## Project 2 — NHS / Health Data
**Main emphasis:** Python + pandas, larger datasets, cleaning, trends, merging data sources.

Potential themes:
- NHS prescribing
- GLP-1 prescribing
- geographical and temporal trends
- population-normalised rates

## Project 3 — Finance / Housing
**Main emphasis:** time-series analysis, CTEs, window functions, analytical storytelling.

Potential themes:
- UK mortgage data
- house prices
- affordability
- interest rates
- arrears / lending trends

## Optional Project 4 — API / Pipeline
**Main emphasis:** Python automation and data ingestion.

Potential theme:
- UK crime API
- automated extraction → SQL → analysis

---

# 2. Learning Status System

Use these statuses for every skill:

- ⚪ **Not encountered** — we have not used it yet.
- 🔵 **Encountered** — I understand the basic idea and have seen/used it once.
- 🟡 **Developing** — I have used it several times but still need prompts, practice, or clarification.
- 🟢 **Comfortable** — I can recognise when to use it, explain the idea, and use it without being told the technique.

A skill does **not** become 🟢 just because I successfully copied or wrote it once.

To become 🟢 I should be able to:
1. Explain roughly what it does.
2. Recognise when it may be useful.
3. Write/use it without being given the exact syntax.
4. Combine it with other SQL/Python concepts.

---

# 3. Learning Spiral

## Stage A — Encounter
Learn only enough of a new concept to keep the project moving.

Example:
- `CASE` first appears.
- Learn the core idea and one useful pattern.
- Do **not** study every possible syntax variation immediately.

Typical time: **5–10 minutes**

## Stage B — Retrieve
Bring the concept back later without announcing which technique is required.

Example:
- “Create three speed categories.”
- I have to remember that `CASE` may be useful.

## Stage C — Apply
Use the same concept for a different real analytical problem.

Example:
- `CASE` for labels.
- Later `CASE` for conditional aggregation.
- Later `CASE` for missing-value handling.

## Stage D — Combine
Use it together with several other concepts.

Example:
- `CASE` + `GROUP BY` + CTE + `RANK()`.

This is the point where the concept becomes part of my analytical toolkit rather than memorised syntax.

---

# 4. Deep Topics Are Split Into Sub-Skills

Do not treat large topics as one item.

## CTEs

Progression:
- ⚪ Understand what a CTE is
- ⚪ Filter data inside a CTE
- ⚪ Aggregate inside a CTE
- ⚪ Join a CTE to another table
- ⚪ Use multiple CTEs
- ⚪ Combine CTEs with window functions

## Window Functions

Progression:
- ⚪ Understand why windows differ from `GROUP BY`
- ⚪ `SUM() OVER()`
- ⚪ `AVG() OVER()`
- ⚪ `PARTITION BY`
- ⚪ `ROW_NUMBER()`
- ⚪ `RANK()`
- ⚪ `DENSE_RANK()`
- ⚪ `LAG()`
- ⚪ `LEAD()`
- ⚪ Running totals
- ⚪ Window frames (`ROWS BETWEEN ...`) — later, only if useful

The priority is not just syntax.

We need two types of knowledge:

### Syntax knowledge
“How do I write `RANK() OVER (...)`?”

### Selection knowledge
“This problem asks me to rank within groups, so a window function is probably appropriate.”

**Selection knowledge is more important.**

---

# 5. Core Skill Tracker Categories

## SQL Fundamentals
- `SELECT`
- aliases
- `DISTINCT`
- `WHERE`
- comparison operators
- `AND` / `OR` / `NOT`
- `IN`
- `BETWEEN`
- `LIKE`
- `ORDER BY`
- `LIMIT`

## Aggregation
- `COUNT`
- `SUM`
- `AVG`
- `MIN`
- `MAX`
- `GROUP BY`
- `HAVING`
- conditional aggregation

## Data Transformation
- `CASE`
- `NULL`
- `COALESCE`
- type conversion / casting
- date/time functions
- string functions

## Relational SQL
- primary keys
- foreign keys
- composite keys
- one-to-many relationships
- `INNER JOIN`
- `LEFT JOIN`
- join duplication
- multi-table joins

## Intermediate / Advanced Analyst SQL
- subqueries
- CTEs
- window functions
- ranking
- running totals
- previous/next row comparisons
- percent of total
- change over time

## Database / Data Engineering Basics
- database
- schema
- table
- raw layer
- clean/analytical layer
- importing CSVs
- data-quality checks
- basic indexes
- views

## Python Fundamentals
- variables
- data types
- lists
- dictionaries
- conditions
- loops
- functions

## pandas
- DataFrames
- reading files
- selecting columns
- filtering
- sorting
- `groupby`
- aggregation
- `merge`
- missing values
- cleaning
- dates
- reshaping

## Visualisation
- matplotlib
- choosing chart types
- labels/titles
- avoiding misleading charts
- communicating one clear point per chart

## Portfolio / GitHub
- Git basics
- commits
- project structure
- README
- documenting assumptions
- SQL scripts
- notebooks
- charts
- findings
- limitations

---

# 6. Session Structure

The session should not turn into a lecture.

## Beginning of Each Session — 5 to 10 minutes

### A. Recall where we are
Answer:
- What did we build last time?
- What is the next project milestone?

### B. Retrieval practice
Usually **3–5 short questions** from previously encountered material.

The questions should be mixed:
- one syntax retrieval
- one “which tool would you use?” question
- one interpretation/debugging question

Example:
- What does `GROUP BY` do?
- If you need a category based on conditions, what tool might help?
- Why might a `LEFT JOIN` increase the number of rows?

Do not spend the whole session reviewing.

### C. Check the review queue
Choose only the concepts that are due or especially important.

---

# 7. Main Part of Each Session

## Primary rule
**Project progress comes first.**

A normal session should produce something tangible:
- a table imported
- a clean table created
- a query answered
- a join completed
- a chart created
- a README section written
- a GitHub commit made

## New-concept limit
Prefer:
- **1 major new concept per session**
- up to **2–3 small supporting concepts**

If something large appears unexpectedly:
1. Learn enough to continue.
2. Add it to the review queue.
3. Return to the project.

## Concept deep-dive rule
Only deep-dive when:
- the concept is blocking progress,
- it is a high-value analyst skill,
- or repeated mistakes show that the basic model is unclear.

Typical deep-dive: **10–20 minutes**, not an entire session.

---

# 8. End of Each Session — 5 to 10 minutes

Update four things.

## A. Project progress
Example:
- ✅ Imported collision data
- ✅ Verified 513,801 rows
- ✅ Created raw schema
- ➡️ Next: inspect raw data quality

## B. Skill tracker
Example:
- `SELECT` 🟡
- `COUNT` 🟡
- `GROUP BY` 🟡
- `CASE` 🔵
- joins ⚪

## C. Review queue
Example:
- `CASE`: create categories without being prompted
- `GROUP BY`: group by two columns
- data types: revisit during clean-table creation

## D. Mistake log
Example:
- Compared a text column with numeric `1`.
- Forgot that raw columns are stored as text.
- Lesson: check the data type before debugging the comparison.

---

# 9. Retrieval Schedule

We do not need a rigid calendar, but important concepts should reappear roughly like this:

- first encounter
- next session
- a few sessions later
- about a week later
- later inside a mixed problem
- later as an interview-style question

The exact timing can change based on performance.

If a concept is easy, review it less.
If a concept repeatedly causes difficulty, bring it back sooner.

---

# 10. Practice Style

Avoid large blocks of repetitive drills.

Prefer:
- 3–5 short retrieval questions
- real data
- mixed concepts
- gradually fewer hints
- problems where the required SQL tool is **not named**

Progression:

### Early
“Use `CASE` to create severity labels.”

### Developing
“Create readable severity labels.”

### Later
“Produce a report showing collision severity in readable categories.”

### Comfortable
“Analyse how severity patterns differ by road type.”

At the last stage I must choose the relevant SQL techniques myself.

---

# 11. Progress Must Be Visible

This project should not disappear into months of studying.

We will optimise for **visible output**.

## Every few sessions, produce something portfolio-visible:
- a completed SQL script
- a clean table
- a documented data-quality finding
- a chart
- a written insight
- a GitHub commit
- a README section

## Road Safety Project Milestones

### Milestone 1 — Database foundation
- PostgreSQL installed
- database created
- raw schema created
- collision data imported
- vehicles/casualties imported

### Milestone 2 — Clean analytical dataset
- inspect raw values
- handle missing/special codes
- convert data types
- create clean tables
- verify keys and relationships

### Milestone 3 — Core SQL analysis
- descriptive statistics
- severity patterns
- time trends
- road/weather/light conditions
- geography
- data-quality findings

### Milestone 4 — Multi-table analysis
- collisions + vehicles
- collisions + casualties
- all three tables
- driver/vehicle/casualty questions
- joins and duplication checks

### Milestone 5 — Intermediate SQL
- CTEs
- conditional aggregation
- ranking
- window functions
- trends/change calculations

### Milestone 6 — Python layer
- connect/read data
- pandas analysis
- visualisation
- selected deeper analyses

### Milestone 7 — Portfolio packaging
- clean repository
- README
- methodology
- findings
- charts
- limitations
- reproducible SQL/Python files

---

# 12. Time-Boxing / Anti-Endless-Project Rules

The first portfolio project should show meaningful progress quickly.

Rules:
1. Do not attempt every possible road-safety question.
2. Choose a small number of strong analytical questions.
3. Stop adding features once the project demonstrates the targeted skills.
4. Move unfinished “interesting ideas” into a backlog.
5. Publish an initial useful version before polishing endlessly.
6. Improve the repository incrementally through GitHub commits.

A reasonable target is to reach a **presentable first version in roughly 6–10 focused working sessions**, depending on session length and how much SQL/Python learning is needed.

It does not need to be “finished forever” before it goes on GitHub.

We can publish:
- **v0.1** database + initial SQL exploration
- **v0.2** clean data + stronger analysis
- **v0.3** joins + advanced SQL
- **v1.0** Python + polished README/findings

This lets the portfolio visibly improve over time.

---

# 13. Interview Practice

Interview practice should be integrated, not become another full course.

At appropriate points:
- explain a query in plain English
- compare two SQL approaches
- debug a broken query
- answer “when would you use X?”
- write a short query without hints
- interpret a result
- discuss limitations

Later, include short standalone SQL interview questions in retrieval sessions.

---

# 14. Current Project Position

## UK Road Safety — Current Status

Completed:
- ✅ PostgreSQL installed
- ✅ DBeaver installed
- ✅ `uk_road_safety` database created
- ✅ `raw` schema created
- ✅ `raw.collisions` table created
- ✅ collision CSV imported
- ✅ verified **513,801 rows**
- ✅ encountered `SELECT`
- ✅ encountered `COUNT`
- ✅ encountered `GROUP BY`
- 🔵 encountered `CASE`

Next:
1. Inspect raw collision data.
2. Profile unusual/missing values.
3. Build the clean collisions table with proper data types.
4. Import vehicles and casualties.
5. Continue SQL analysis.

---

# 15. Guiding Principle

The goal is not:

> “Finish a SQL curriculum.”

The goal is:

> **Become able to look at a real analytical problem, decide which SQL/Python tools are useful, use them, explain the result, and show the work in a professional portfolio.**

The portfolio gives the learning direction.
Spaced retrieval makes the learning stick.
Frequent visible outputs prevent the project from becoming endless.
