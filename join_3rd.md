3. Selezionare tutti i corsi in cui insegna Fulvio Amato (id=44)

SELECT `courses`.`name` AS `course_name`, `teachers`.`id`, `teachers`.`name` AS `teacher_name`, `teachers`.`surname` AS `teacher_surname`

FROM `courses`

JOIN `course_teacher`

ON `courses`.`id` = `course_teacher`.`course_id`

JOIN `teachers`

ON `teachers`.`id` = `course_teacher`.`teacher_id`

WHERE `teachers`.`id` = 44;
