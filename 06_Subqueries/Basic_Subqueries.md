# Basic Subqueries

## Population Greater Than Russia

```sql
SELECT name
FROM world
WHERE population >
(
SELECT population
FROM world
WHERE name='Russia'
);
```

---

## European Countries With Higher Per-Capita GDP Than UK

```sql
SELECT name
FROM world
WHERE continent='Europe'
AND gdp/population >
(
SELECT gdp/population
FROM world
WHERE name='United Kingdom'
);
```

---

## GDP Greater Than Every European Country

```sql
SELECT name
FROM world
WHERE gdp >
(
SELECT MAX(gdp)
FROM world
WHERE continent='Europe'
);
```
