# Dune.com (Cheat Sheet)

This is a cheatsheet for dune.com commands and patterns (mostly notes-to-self). They are incomplete by default.

## Date and Time

### Getting year, month, day from timestamp

`year()`: Returns the year from x.
`month()`: Returns the month of the year from x.

Source: 
[dune.com](https://dune.com/docs/query/DuneSQL-reference/Functions-and-operators/datetime/?h=year#year)

Example of hacky way I needed to get `2023_09` type `varchar`:

```sql
CONCAT(CAST(year(time) as varchar), '-', cast(month(time) as varchar)) as year_month,
```
