# REPLACE Function

Replaces occurrences of one string with another.

## Syntax

```sql
REPLACE(text, old, new)
```

---

## Example

```sql
SELECT REPLACE('vessel','e','a');
```

Output:

```text
vassal
```

---

## Proper capital extension

```sql
SELECT name,
       REPLACE(capital, name, '') AS extension
FROM world
WHERE capital LIKE CONCAT(name, '_%');
```
