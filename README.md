### Selezionare gli studenti nati nel 1990 

```SQL
SELECT * 
FROM db_university.students
WHERE `date_of_birth` BETWEEN '1990-01-01' AND '1990-12-31';