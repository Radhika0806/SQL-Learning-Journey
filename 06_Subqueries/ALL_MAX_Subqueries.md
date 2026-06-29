# ALL and MAX

## Largest Country By Area In Each Continent

```sql
SELECT continent, name, area
FROM world x
WHERE area >= ALL
(
SELECT area
FROM world y
WHERE y.continent = x.continent
AND area > 0
);
```
