 4. Selezionare tutti gli studenti con i dati relativi al corso di laurea a cui sono iscritti e il relativo dipartimento, in ordine alfabetico per cognome e nome

SELECT `departments`.`name` AS `departments_name`, `degrees`.`name` AS `degree_name`, `students`.`surname`, `students`.`name` AS `student_name` 

FROM `departments`

JOIN `degrees`

ON `departments`.`id` = `degrees`.`department_id`

JOIN `students`

ON `degrees`.`id` = `students`.`degree_id`

ORDER BY `students`.`surname` ASC ,`students`.`name` ASC;
