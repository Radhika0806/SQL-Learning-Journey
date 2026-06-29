# XOR Operator

Returns rows where exactly one condition is true.

## Example

```sql
SELECT name, population, area
FROM world
WHERE area > 3000000
XOR population > 25000000;
```
