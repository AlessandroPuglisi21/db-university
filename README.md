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

### Selezionare tutti i corsi del primo semestre del primo anno di un qualsiasi corso di laurea (286)

```SQL
SELECT * 
FROM db_university.courses
WHERE `period` = 'I semestre' AND `year` = '1'
```

### Selezionare tutti gli appelli d'esame che avvengono nel pomeriggio (dopo le 14) del 20/06/2020 (21)

```SQL 
SELECT * 
FROM db_university.exams
WHERE `date` = '2020-06-20' AND `hour`>= '14:00:00'
```

### Da quanti dipartimenti è composta l'università? (12)

```SQL
SELECT COUNT(id) 
FROM `departments`
```

### Quanti sono gli insegnanti che non hanno un numero di telefono? (50)

```SQL
SELECT COUNT(id)
FROM `teachers`
WHERE `phone` IS NULL
``` 