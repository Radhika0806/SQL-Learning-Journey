# LENGTH Function

Returns the number of characters in a string.

```sql
LENGTH(name)
```

---

## Capital is longer than country name

```sql
SELECT capital, name
FROM world
WHERE LENGTH(capital) > LENGTH(name)
  AND capital LIKE CONCAT(name, '%');
```
