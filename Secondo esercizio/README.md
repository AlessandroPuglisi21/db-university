### Contare quanti iscritti ci sono stati ogni anno

```SQL
SELECT COUNT(id), YEAR(enrolment_date) AS enrolment_year
FROM db_university.students
GROUP BY YEAR(enrolment_date);
```

### Contare gli insegnanti che hanno l'ufficio nello stesso edificio

```SQL
SELECT COUNT(id), office_address
FROM db_university.teachers
GROUP BY office_address
```
