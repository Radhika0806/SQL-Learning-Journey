# ORDER BY

Used to sort query results.

## ASC

```sql
ORDER BY winner ASC;
```

## DESC

```sql
ORDER BY yr DESC;
```

---

## Nobel Winners Starting With Sir

```sql
SELECT winner, yr, subject
FROM nobel
WHERE winner LIKE 'Sir%'
ORDER BY yr DESC, winner ASC;
```

---

## Chemistry and Physics Last

```sql
SELECT winner, subject
FROM nobel
WHERE yr = 1984
ORDER BY
subject IN ('Physics','Chemistry'),
subject,
winner;
```
