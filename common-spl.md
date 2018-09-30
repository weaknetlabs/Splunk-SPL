# Commonly Used SPL Cheet Sheet
In this cheat sheet, you will find commonly used SPL syntax and full queries that I find myself using on an almost-daily basis.

## Indexes
These queries are for all things related to Splunk> Indexes.
### Display ALL Available Indexes
To display all available indexes, do the following.

`| eventcount summarize=false index=* | dedup index | fields index`
