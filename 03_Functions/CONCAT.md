# CONCAT Function

Combines strings together.

## Syntax

```sql
CONCAT(string1, string2)
```

---

## Capital equals Country + City

```sql
SELECT name
FROM world
WHERE capital = CONCAT(name, ' City');
```

---

## Capital contains country name

```sql
SELECT capital, name
FROM world
WHERE capital LIKE CONCAT(name, '%');
```
