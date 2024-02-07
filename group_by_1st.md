1. Contare quanti iscritti ci sono stati ogni anno

SELECT YEAR(`enrolment_date`) AS enrolment_year, COUNT(*) AS students_enrolled 

FROM `students`

GROUP BY YEAR(`enrolment_date`)

ORDER BY YEAR(`enrolment_date`) ASC;
