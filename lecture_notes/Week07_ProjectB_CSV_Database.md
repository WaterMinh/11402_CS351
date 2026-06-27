# Week 07 — Project B: CSV Database and Query Engine

## Topic

Project B implementation: CSV-based mini database and query engine.

---

## Project Idea

Project B is a simple CSV-based mini database and query engine written in C++.

The goal is to load data from a CSV file, store it in memory, and allow the user to run simple SQL-like queries from the console.

---

## Implemented Features

- Load CSV file
- Parse CSV rows and columns
- Store data in memory
- Support SELECT queries
- Support WHERE conditions
- Display query results in console

---

## CSV Data

The first line of the CSV file is treated as column names.

Example:

```csv
id,name,major,grade
1,Minh,CS,90
2,Anna,CS,85
```

Each data line is parsed into fields:

```text
id = 1
name = Minh
major = CS
grade = 90
```

---

## Storage Design

The parsed data is stored in memory using C++ containers.

```cpp
vector<map<string, string>>
```

Each row is stored as a map:

```text
column name → value
```

---

## Supported Query Syntax

Select all columns:

```sql
SELECT * FROM students
```

Select specific columns:

```sql
SELECT name,grade FROM students
```

Select with WHERE condition:

```sql
SELECT name,grade FROM students WHERE major=CS
```

---

## How It Works

```text
CSV File
↓
CSV Loader
↓
CSV Parser
↓
In-Memory Storage
↓
Query Parser
↓
SELECT / WHERE Engine
↓
Console Output
```

---

## Demo Cases

I prepared four demo cases:

1. Load CSV file
2. SELECT all data
3. SELECT specific columns
4. SELECT with WHERE filtering

---

## Reflection

Project B helped me understand how a simple database system works internally. Instead of using an external database, I practiced parsing files, storing data in memory, and processing user queries manually.