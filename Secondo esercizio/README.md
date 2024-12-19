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
### Calcolare la media dei voti di ogni appello d'esame

```SQL
SELECT AVG(vote),exam_id
FROM db_university.exam_student
GROUP BY  exam_id
```

### Contare quanti corsi di laurea ci sono per ogni dipartimento

```SQL
SELECT course_id, COUNT(id) AS total_exams
FROM db_university.exams
GROUP BY course_id;
```