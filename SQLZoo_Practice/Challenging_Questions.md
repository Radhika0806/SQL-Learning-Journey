# SQLZoo Questions I Found Challenging

## Question 1

Countries containing all vowels and no spaces.

## Question 2

Countries with three or more 'a'.

## Question 3

Capital includes country name.

## Question 4

Capital is a proper extension of country name.

## Question 5

Show country name and extension of capital.

## Question 6

Show Nobel winners whose first name is John.

```sql
SELECT winner
FROM nobel
WHERE winner LIKE 'John%';
```

## Question 7

Show Nobel winners starting with Sir.

```sql
SELECT winner, yr, subject
FROM nobel
WHERE winner LIKE 'Sir%'
ORDER BY yr DESC, winner ASC;
```
