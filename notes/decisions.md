Decisions made:
### Set Up and Structure
1. src and notebook separation
src/
    contains reusable functions or 
    functions that I end up retyping in notebooks,
    i can then park them under src as a function and call them as notebooks
notebooks/
    for narrative and showing thought processes

Process: Write in notebooks -> Move to src when repetition is observed


2. Pandas vs polars
- Pandas -> older, single threaded, 
    - eager evaluation
    + every ml library expects pandas
- Polars -> newer, multi threaded,
    + faster, memory efficient, query gets optimized before evaluation, like SQL
    - smaller ecosystem

Process: polars for data loading, feature engineering -> convert to pandas for models

## 00_data_access
1. i tested that getenv works

2. established a connection to the installed duckdb

3. installed and loaded httpfs - allows duckdb to read files over a network instead of from my local disk

4. created duckdb secret for access to the r2 db

5. Sanity Checks
    - Use `glob` (global pattern match) to list files in a directory.
    - Example: `s3/.../**/*.parquet`

        | Pattern | Matches |
        |---|---|
        | `**` | Any number of directory levels |
        | `*` | Within a single directory level |

6. Ran a DISTINCT sql command to find out that there are 3 currencies with spot and perp in the bbo.

## Running To Do:
- what does this timestamp mean?
