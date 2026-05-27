This will contain all decisions i have made

### Set Up
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