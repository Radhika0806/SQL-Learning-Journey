# LEFT Function

Returns characters from the left side of a string.

```sql
LEFT(name, 1)
```

---

## Country and capital start with same letter

```sql
SELECT name, capital
FROM world
WHERE LEFT(name,1)=LEFT(capital,1)
  AND name <> capital;
```
