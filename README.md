### Selezionare gli studenti nati nel 1990 

```SQL
SELECT * 
FROM db_university.students
WHERE `date_of_birth` BETWEEN '1990-01-01' AND '1990-12-31';
```

### Selezionare tutti i corsi che valgono più di 10 crediti (479)

```SQL
SELECT * 
FROM db_university.courses
WHERE `cfu`>= '10'
```

### Selezionare tutti gli studenti che hanno più di 30 anni

```SQL
SELECT * 
FROM db_university.students
WHERE `date_of_birth` < '1996-12-18'
```