1. Selezionare tutti gli studenti iscritti al Corso di Laurea in Economia

SELECT `degrees`.`name` as `degree_name`, `students`.`name`, `students`.`surname`

FROM `degrees`

JOIN `students`

ON `degrees`.`id` = `students`.`degree_id`

WHERE `degrees`.`name`= 'Corso di Laurea in Economia';
