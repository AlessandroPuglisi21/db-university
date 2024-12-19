### Contare quanti iscritti ci sono stati ogni anno

```SQL
SELECT COUNT(id), YEAR(enrolment_date) AS enrolment_year
FROM db_university.students
GROUP BY YEAR(enrolment_date);
```
