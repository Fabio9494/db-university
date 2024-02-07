4. Contare quanti corsi di laurea ci sono per ogni dipartimento

SELECT COUNT(*) as `degrees_number`, `department_id`

FROM `degrees`

GROUP BY `department_id`;
