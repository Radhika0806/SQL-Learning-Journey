# NOT LIKE

Used to exclude matching patterns.

## Example

```sql
SELECT name
FROM world
WHERE name NOT LIKE '% %';
```

Returns only single-word country names.
