3. Calcolare la media dei voti di ogni appello d'esame

SELECT AVG(`vote`) AS vote_average, `exam_id` 

FROM `exam_student` 

GROUP BY `exam_id`;
