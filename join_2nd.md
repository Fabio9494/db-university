2. Selezionare tutti i Corsi di Laurea Magistrale del Dipartimento di Neuroscienze

SELECT `departments`.`name` AS `deparment_name`, `degrees`.`name` AS `degrees_name`, `degrees`.`level` 

FROM `departments` 

JOIN `degrees` 

ON `degrees`.`department_id`=`departments`.`id` 

WHERE `departments`.`name`= 'Dipartimento di Neuroscienze' AND `degrees`.`level` = 'magistrale';
