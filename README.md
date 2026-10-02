# Join-Order-Benchmark-JOB-for-MySQL

Benchmark was downloaded from https://zenodo.org/records/19205561?utm_source=chatgpt.com.



## MySQL Load Data from csv Files

`SHOW GLOBAL VARIABLES LIKE 'local_infile';`

If it returns:

`local_infile    OFF`

enable it:

`SET GLOBAL local_infile = ON;`

-----

When creating/editing the connection:

Database → Manage Connections → your connection → Advanced

Look for the connection options and add:

`OPT_LOCAL_INFILE=1`

Then reconnect.
