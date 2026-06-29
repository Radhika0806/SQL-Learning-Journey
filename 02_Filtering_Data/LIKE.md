# LIKE Operator

LIKE is used for pattern matching.

## Wildcards

| Symbol | Meaning |
|----------|----------|
| % | Any number of characters |
| _ | Exactly one character |

---

## Countries containing "United"

```sql
SELECT name
FROM world
WHERE name LIKE 'United%';
```

---

## Countries with exactly 4 characters

```sql
SELECT name
FROM world
WHERE name LIKE '____';
```

---

## Countries having 3 or more 'a'

```sql
SELECT name
FROM world
WHERE name LIKE '%a%a%a%';
```

---

## Countries containing all vowels and having a single-word name

```sql
SELECT name
FROM world
WHERE name LIKE '%a%'
  AND name LIKE '%e%'
  AND name LIKE '%i%'
  AND name LIKE '%o%'
  AND name LIKE '%u%'
  AND name NOT LIKE '% %';
```
