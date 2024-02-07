 5. Selezionare tutti i corsi di laurea con i relativi corsi e insegnanti

SELECT degrees.name, courses.name, teachers.name, teachers.surname

FROM degrees

JOIN courses ON courses.degree_id = degrees.id

JOIN course_techer ON course_teacher.course_id = courses.id

JOIN teachers ON course_teacher_id = teachers.id;
