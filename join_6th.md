 6. Selezionare tutti i docenti che insegnano nel Dipartimento di Matematica (54)

SELECT teachers.name, teachers.surname

FROM teachers

JOIN course_teacher ON course_teacher.teacher_id = teachers.id

JOIN courses ON course_teacher.course_id = courses.id

JOIN degrees ON courses.degree_id = degrees.id

JOIN departments ON degrees.department_id = departments.id

WHERE departments.name = 'Dipartimento di Matematica';
